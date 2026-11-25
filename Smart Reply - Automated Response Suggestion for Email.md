Source: https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45189.pdf

---

Smart Reply: Automated Response Suggestion for Email

Anjuli Kannan(cid:70)

Karol Kurach(cid:70)

Sujith Ravi(cid:70)

Tobias Kaufmann(cid:70)

Andrew Tomkins

Balint Miklos

Greg Corrado

László Lukács

Marina Ganea

Peter Young

Vivek Ramavajjala

Google
{anjuli, kkurach, sravi, snufkin}@google.com

ABSTRACT
In this paper we propose and investigate a novel end-to-end
method for automatically generating short email responses,
called Smart Reply. It generates semantically diverse sug-
gestions that can be used as complete email responses with
just one tap on mobile. The system is currently used in In-
box by Gmail and is responsible for assisting with 10% of
all mobile responses.
It is designed to work at very high
throughput and process hundreds of millions of messages
daily. The system exploits state-of-the-art, large-scale deep
learning.

We describe the architecture of the system as well as the
challenges that we faced while building it, like response di-
versity and scalability. We also introduce a new method for
semantic clustering of user-generated content that requires
only a modest amount of explicitly labeled data.

Keywords
Email; LSTM; Deep Learning; Clustering; Semantics

1.

INTRODUCTION

Email is one of the most popular modes of communica-
tion on the Web. Despite the recent increase in usage of
social networks, email continues to be the primary medium
for billions of users across the world to connect and share
information [2]. With the rapid increase in email overload, it
has become increasingly challenging for users to process and
It can be especially time-
respond to incoming messages.
consuming to type email replies on a mobile device.

(cid:70)Equal contribution.

Permission to make digital or hard copies of part or all of this work for personal or
classroom use is granted without fee provided that copies are not made or distributed
for proﬁt or commercial advantage and that copies bear this notice and the full citation
on the ﬁrst page. Copyrights for third-party components of this work must be honored.
For all other uses, contact the owner/author(s).
KDD ’16, August 13–17, 2016, San Francisco, CA, USA
c(cid:13) 2016 Copyright held by the owner/author(s).

ACM ISBN 978-1-4503-4232-2/16/08..
DOI: http://dx.doi.org/XXXX.XXXX

An initial study covering several million email-reply pairs
showed that ∼25% of replies have 20 tokens or less. Thus
we raised the following question: can we assist users with
composing these short messages? More speciﬁcally, would
it be possible to suggest brief responses when appropriate,
just one tap away?

Figure 1: Example Smart Reply suggestions.

Preprocess
Email

No Smart
Reply

Trigger
response?

no

yes

Response
selection
(LSTM)

Diversity
selection

Permitted
responses
and clusters

Smart
Reply
Suggested

Figure 2: Life of a message. The ﬁgure presents the
overview of inference.

To address this problem, we leverage the sequence-to-
sequence learning framework [23], which uses long short-
term memory networks (LSTMs) [10] to predict sequences
of text. Consistent with the approach of the Neural Conver-
sation Model [24], our input sequence is an incoming mes-
sage and our output distribution is over the space of possible
replies. Training this framework on a large corpus of con-
versation data produces a fully generative model that can
produce a response to any sequence of input text. As [24]
demonstrated on a tech support chat corpus, this distribu-
tion can be used to decode coherent, plausible responses.

However, in order to deploy such a model into a product
used globally by millions, we faced several challenges not
considered in previous work:

• Response quality How to ensure that the individual
response options are always high quality in language
and content.

• Utility How to select multiple options to show a user
so as to maximize the likelihood that one is chosen.

• Scalability How to eﬃciently process millions of mes-
sages per day while remaining within the latency re-
quirements of an email delivery system.

• Privacy How to develop this system without ever in-

specting the data except aggregate statistics.

To tackle these challenges, we propose Smart Reply (Fig-
ure 1), a novel method and system for automated email
response suggestion. Smart Reply consists of the following
components, which are also shown in Figure 2:

1. Response selection: At the core of our system, an
LSTM neural network processes an incoming message,
then uses it to predict the most likely responses. LSTM
computation can be expensive, so we improve scalabil-
ity by ﬁnding only the approximate best responses. We
explain the model in detail in Section 3.

2. Response set generation: To deliver high response
quality, we only select responses from response space
which is generated oﬄine using a semi-supervised graph
learning approach. This is discussed in Section 4.

3. Diversity: After ﬁnding a set of most likely responses
from the LSTM, we would like to choose a small set to
show to the user that maximize the total utility. We
found that enforcing diverse semantic intents is critical
to making the suggestions useful. Our method for this
is described further in Section 5.

4. Triggering model: A feedforward neural network de-
cides whether or not to suggest responses. This fur-
ther improves utility by not showing suggestions when
they are unlikely to be used. We break this out into
a separate component so that we have the option to
use a computationally cheaper architecture than what
is used for the scoring model; this keeps the system
scalable. This model is described in Section 6.

The combination of these components is a novel end-to-
end method for generating short, complete responses to emails,
going beyond previous works. For response selection it ex-
ploits state-of-the-art deep learning models trained on bil-
lions of words, and for response set generation it introduces
a new semi-supervised method for semantic understanding
of user-generated content.

Moreover, since it directly addresses all four challenges
mentioned above, it has been successfully deployed in I nbox.
Currently, the Smart Reply system is responsible for assist-
ing with 10% of email replies for I nbox on mobile.

Next, we discuss the related work in Section 2, followed by
a description of our core system components in Sections 3, 4,
5, and 6. We close by showing modeling results in Section 7
and our conclusions in Section 8.

2. RELATED WORK

As we consider related work, we note that building an
automated system to suggest email responses is not a task
for which there is existing literature or benchmarks, nor is
this a standard machine learning problem to which existing
algorithms can be readily applied. However, there is work
related to two of our core components which we will review
here: predicting responses and identifying a target response
space.

Predicting full responses. Much work exists on analyz-
ing natural language dialogues in public domains such as
Twitter, but it has largely focused on social media tasks like
predicting whether or not a response is made [3], predicting
next word only [14], or curating threads [4].

Full response prediction was initially attempted in [16],
which approached the problem from the perspective of ma-
chine translation: given a Twitter post, ”translate” it into
a response using phrase-based statistical machine transla-
tion (SMT). Our approach is similar, but rather than using

SMT we use the neural network machine translation model
proposed in [23], called ”sequence-to-sequence learning”.

Sequence-to-sequence learning, which makes use of long
short-term memory networks (LSTMs) [10] to predict se-
quences of text, was originally applied to Machine Trans-
lation but has since seen success in other domains such as
image captioning [25] and speech recognition [6].

Other recent works have also applied recurrent neural net-
works (RNNs) or LSTMs to full response prediction [21],
[20], [19], [24]. In [21] the authors rely on having an SMT
system to generate n-best lists, while [19] and [24], like this
work, develop fully generative models. Our approach is most
similar to the Neural Conversation Model [24], which uses
sequence-to-sequence learning to model tech support chats
and movie subtitles.

The primary diﬀerence of our work is that it was deployed
in a production setting, which raised the challenges of re-
sponse quality, utility, scalability, and privacy. These chal-
lenges were not considered in any of these related works and
led to our novel solutions explained in the rest of this paper.
Furthermore, in this work we approach a diﬀerent domain
than [21], [20], [19], and [24], which primarily focus on social
media and movie dialogues. In both of those domains it can
be acceptable to provide a response that is merely related
or on-topic. Email, on the other hand, frequently expresses
a request or intent which must be addressed in the response.

Identifying a target response space. Our approach here
builds on the Expander graph learning approach [15], since
it scales well to both large data (vast amounts of email)
and large output sizes (many diﬀerent underlying seman-
tic intents). While Expander was originally proposed for
knowledge expansion and classiﬁcation tasks [26], our work
is the ﬁrst to use it to discover semantic intent clusters from
user-generated content.

Other graph-based semi-supervised learning techniques have

been explored in the past for more traditional classiﬁcation
problems [27, 5]. Other related works have explored tasks in-
volving semantic classiﬁcation [12] or identifying word-level
intents [17] targeted towards Web search queries and other
forums [7]. However, the problem settings and tasks them-
selves are signiﬁcantly diﬀerent from what is addressed in
our work.

Finally, we note that Smart Reply is the ﬁrst work to
address these tasks together and solve them in a single end-
to-end, deployable system.

3. SELECTING RESPONSES

The fundamental task of the Smart Reply system is to ﬁnd
the most likely response given an original message. In other
words, given original message o and the set of all possible
responses R, we would like to ﬁnd:

r∗ = argmax

P (r|o)

r∈R

3.1 LSTM model

Since we are scoring one sequence of tokens r, conditional
on another sequence of tokens o, this problem is a natural
ﬁt for sequence-to-sequence learning [23]. The model itself
is an LSTM. The input is the tokens of the original message
{o1, ..., on}, and the output is the conditional probability
distribution of the sequence of response tokens given the
input:

P (r1, ..., rm|o1, ..., on)

As in [23], this distribution can be factorized as:

P (r1, ..., rm|o1, ..., on) =

m
(cid:89)

i=1

P (ri|o1, ..., on, r1, ..., ri−1)

First, the sequence of original message tokens, including a
special end-of-message token on, are read in, such that the
LSTM’s hidden state encodes a vector representation of the
whole message. Then, given this hidden state, a softmax
output is computed and interpreted as P (r1|o1, ..., on), or
the probability distribution for the ﬁrst response token. As
response tokens are fed in, the softmax at each timestep t
is interpreted as P (rt|o1, ..., on, r1, ..., rt−1). Given the fac-
torization above, these softmaxes can be used to compute
P (r1, ..., rm|o1, ..., on).

Training Given a large corpus of messages, the training
objective is to maximize the log probability of observed re-
sponses, given their respective originals:

(cid:88)

(o,r)

log P (r1, ..., rm|o1, ..., on)

We train against this objective using stochastic gradient
descent with AdaGrad [8]. Ten epochs are run over a mes-
sage corpus which will be described in Section 7.1. Due to
the size of the corpus, training is run in a distributed fashion
using the TensorFlow library [1].

Both our input and output vocabularies consist of the
most frequent English words in our training data after pre-
processing (steps described in Section 7.1). In addition to
the standard LSTM formulation, we found that the addition
of a recurrent projection layer [18] substantially improved
both the quality of the converged model and the time to
converge. We also found that gradient clipping (with the
value of 1) was essential to stable training.

Inference At inference time we can feed in an original mes-
sage and then use the output of the softmaxes to get a prob-
ability distribution over the vocabulary at each timestep.
These distributions can be used in a variety of ways:

1. To draw a random sample from the response distribu-
tion P (r1, ..., rm|o1, ..., on). This can be done by sam-
pling one token at each timestep and feeding it back
into the model.

To ﬁnd this response, we will construct a model that can
score responses and then ﬁnd the highest scoring response.

We will next describe how the model is formulated, trained,
and used for inference. Then we will discuss the core chal-
lenges of bringing this model to produce high quality sug-
gestions on a large scale.

2. To approximate the most likely response, given the
original message. This can be done greedily by taking
the most likely token at each time step and feeding it
back in. A less greedy strategy is to use a beam search,
i.e., take the top b tokens and feed them in, then retain
the b best response preﬁxes and repeat.

Query
Hi, I thought it would be
great for us to sit down
and chat. I am free
Tuesday and Wenesday.
Can you do either of
those days?

Thanks!

–Alice

Top generated responses
I can do Tuesday.
I can do Wednesday.
How about Tuesday?
I can do Tuesday!
I can do Tuesday. What
time works for you?
I can do Wednesday!
I can do Tuesday or
Wednesday.
How about Wednesday?
I can do Wednesday. What
time works for you?
I can do either.

Table 1: Generated response examples.

3. To determine the likelihood of a speciﬁc response can-
didate. This can be done by feeding in each token of
the candidate and using the softmax output to get the
likelihood of the next candidate token.

Table 1 shows some example of generating the approxi-

mate most likely responses using a beam search.

3.2 Challenges

As described thus far, the model can generate coherent
and plausible responses given an incoming email message.
However, several key challenges arise when bringing this
model into production.

Response quality In order to surface responses to users,
we need to ensure that they are always high quality in style,
tone, diction, and content.

Given that the model is trained on a corpus of real mes-
sages, we have to account for the possibility that the most
probable response is not necessarily a high quality response.
Even a response that occurs frequently in our corpus may
not be appropriate to surface back to users. For example,
it could contain poor grammar, spelling, or mechanics (your
the best!); it could convey a familiarity that is likely to be
jarring or oﬀensive in many situations (thanks hon!); it could
be too informal to be consistent with other Inbox intelligence
features (yup, got it thx); it could convey a sentiment that
is politically incorrect, oﬀensive, or otherwise inappropriate
(Leave me alone).

While restricting the model vocabulary might address sim-
ple cases such as profanity and spelling errors, it would not
be suﬃcient to capture the wide variability with which, for
example, politically incorrect statements can be made. In-
stead, we use semi-supervised learning (described in detail
in Section 4) to construct a target response space R com-
prising only high quality responses. Then we use the model
described here to choose the best response in R, rather than
the best response from any sequence of words in its vocab-
ulary.

Utility Our user studies showed that suggestions are most
useful when they are highly speciﬁc to the original message
and express diverse intents. However, as column 1 in Table
2 shows, the raw output of the model tends to (1) favor com-
mon but unspeciﬁc responses and (2) have little diversity.

First, to improve speciﬁcity of responses, we apply some
light normalization that penalizes responses which are ap-
plicable to a broad range of incoming messages. The results
of this normalization can be seen in column 2 of Table 2.
For example, the very generic ”Yes!” has fallen out of the
top ten. Second, to increase the breadth of options shown
to the user, we enforce diversity by exploiting the semantic
structure of R, as we will discuss in Section 5. The results
of this are also shown at the bottom of Table 2.

We further improve the utility of suggestions by ﬁrst pass-
ing each message through a triggering model (described in
Section 6) that determines whether suggestions should be
generated at all. This reduces the likelihood that we show
suggestions when they would not be used anyway.

Scalability Our model needs to be deployed in a production
setting and cannot introduce latency to the process of email
delivery, so scalability is critical.

Exhaustively scoring every response candidate r ∈ R,
would require O(|R|l) LSTM steps where l is the length of
the longest response. In previous work [23], this could be
aﬀorded because computations were performed in a batch
process oﬄine. However, in the context of an email deliv-
ery pipeline, time is a much more precious resource. Fur-
thermore, given the tremendous diversity with which people
communicate and the large number of email scenarios we
would like to cover, we can assume that R is very large and
only expected to grow over time. For example, in a uniform
sample of 10 million short responses (say, responses with at
most 10 tokens), more than 40% occur only once. There-
fore, rather than performing an exhaustive scoring of every
candidate r ∈ R, we would like to eﬃciently search for the
best responses such that complexity is not a function of |R|.
Our search is conducted as follows. First, the elements of
R are organized into a trie. Then, we conduct a left-to-right
beam search, but only retain hypotheses that appear in the
trie. This search process has complexity O(bl) for beam size
b and maximum response length l. Both b and l are typically
in the range of 10-30, so this method dramatically reduces
the time to ﬁnd the top responses and is a critical element
of making this system deployable. In terms of quality, we
ﬁnd that, although this search only approximates the best
responses in R, its results are very similar to what we would
get by scoring and ranking all r ∈ R, even for small b. At
b = 128, for example, the top scoring response found by this
process matches the true top scoring response 99% of the
time. Results for various beam sizes are shown in Figure 3.
Additionally, requiring that each message ﬁrst pass through
a triggering model, as mentioned above, has the additional
beneﬁt of reducing the total amount of LSTM computation.

Privacy Note that all email data (raw data, preprocessed
data and training data) was encrypted. Engineers could only
inspect aggregated statistics on anonymized sentences that
occurred across many users and did not identify any user.
Also, only frequent words are retained. As a result, verifying
model’s quality and debugging is more complex.

Our solutions for the ﬁrst three challenges are described

further in Sections 4, 5, and 6.

1

0.8

0.6

0.4

0.2

h
c
r
a
e
s

e
v
i
t
s
u
a
h
x
e

g
n
i
h
c
t
a
m

f
o

y
c
n
e
u
q
e
r
F

0

20

40

60

80

100

120

140

Beam size

Figure 3: Eﬀectiveness of searching the response
space R. For a sample of messages we compute the fre-
quency with which the best candidate found by a beam
search over R matches the best candidate found by exhaus-
tively scoring all members of R. We compare various beam
sizes. At a beam size of 16, these two methods ﬁnd the same
best response 93% of the time.

4. RESPONSE SET GENERATION

Two of the core challenges we face when building the end
to end automated response system are response quality and
utility. Response quality comes from suggesting “high qual-
ity” responses that deliver a positive user experience. Util-
ity comes from ensuring that we don’t suggest multiple re-
sponses that capture the same intent (for example, minor
lexical variations such as “Yes, I’ll be there.” and “I will be
there.”). We can consider these two challenges jointly.

We ﬁrst need to deﬁne a target response space that com-
prises high quality messages which can be surfaced as sug-
gestions. The goal here is to generate a structured response
set that eﬀectively captures various intents conveyed by peo-
ple in natural language conversations. The target response
space should capture both variability in language and in-
tents. The result is used in two ways downstream—(a) de-
ﬁne a response space for scoring and selecting suggestions
using the model described in Section 3, and (b) promote di-
versity among chosen suggestions as discussed in Section 5.
We construct a response set using only the most frequent
anonymized sentences aggregated from the preprocessed data
(described in Section 7.1). This process yields a few million
unique sentences.

4.1 Canonicalizing email responses

The ﬁrst step is to automatically generate a set of canon-
ical responses messages that capture the variability in lan-
guage. For example, responses such as “Thanks for your kind
update.”, “Thank you for updating!”, “Thanks for the status
update.” may appear slightly diﬀerent on the surface but in
fact convey the same information. We parse each sentence
using a dependency parser and use its syntactic structure to
generate a canonicalized representation. Words (or phrases)
that are modiﬁers or unattached to head words are ignored.

4.2 Semantic intent clustering

In the next step, we want to partition all response mes-
sages into “semantic” clusters where a cluster represents a
meaningful response intent (for example, “thank you” type
of response versus “sorry” versus “cannot make it”). All mes-
sages within a cluster share the same semantic meaning but
may appear very diﬀerent. For example, “Ha ha”, “lol” and
“Oh that’s funny!” are associated with the funny cluster.

This step helps to automatically digest the entire infor-
mation present in frequent responses into a coherent set of
semantic clusters. If we were to build a semantic intent pre-
diction model for this purpose, we would need access to a
large corpus of sentences annotated with their corresponding
semantic intents. However, this is neither readily available
for our task nor at this scale. Moreover, unlike typical ma-
chine learning classiﬁcation tasks, the semantic intent space
cannot be fully deﬁned a priori. So instead, we model the
task as a semi-supervised machine learning problem and use
scalable graph algorithms [15] to automatically learn this
information from data and a few human-provided examples.

4.3 Graph construction

We start with a few manually deﬁned clusters sampled
from the top frequent messages (e.g., thanks, i love you,
sounds good). A small number of example responses are
added as “seeds” for each cluster (for example, thanks →
“Thanks!”, “Thank you.”).1

We then construct a base graph with frequent response
messages as nodes (VR). For each response message, we fur-
ther extract a set of lexical features (ngrams and skip-grams
of length up to 3) and add these as “feature” nodes (VF ) to
the same graph. Edges are created between a pair of nodes
(u, v) where u ∈ VR and v ∈ VF if v belongs to the feature
set for response u. We follow the same process and create
nodes for the manually labeled examples VL. We make an
observation that in some cases an incoming original mes-
sage could potentially be treated as a response to another
email depending on the context. For example, consider the
following (original, response) message pairs:

Let us get together soon. → When should we meet?
When should we meet? → How about Friday?

Inter-message relations as shown in the above example can
be modeled within the same framework by adding extra
edges between the corresponding message nodes in the graph.

4.4 Semi-supervised learning

The constructed graph captures relationships between sim-
ilar canonicalized responses via the feature nodes. Next, we
learn a semantic labeling for all response nodes by propa-
gating semantic intent information from the manually la-
beled examples through the graph. We treat this as a semi-
supervised learning problem and use the distributed EX-
PANDER [15] framework for optimization. The learning
framework is scalable and naturally suited for semi-supervised
graph propagation tasks such as the semantic clustering
problem described here. We minimize the following objec-
tive function for response nodes in the graph:

1In practice, we pick 100 clusters and on average 3–5 labeled
seed examples per cluster.

Figure 4: Semantic clustering of response messages.

si|| ˆCi − Ci||2 + µpp|| ˆCi − U ||2

(cid:16) (cid:88)

+ µnp

wij|| ˆCi − ˆCj||2 +

(cid:88)

wik|| ˆCi − ˆCk||2(cid:17)

j∈NF (i)

j∈NR(i)

(1)

where si is an indicator function equal to 1 if the node i is
a seed and 0 otherwise, ˆCi is the learned semantic cluster
distribution for response node i, Ci is the true label distri-
bution (i.e., for manually provided examples), NF (i) and
NR(i) represent the feature and message neighborhood of
node i, µnp is the predeﬁned penalty for neighboring nodes
with divergent label distributions, ˆCj is the learned label
distribution for feature neighbor j, wij is the weight of fea-
ture j in response i, µpp is the penalty for label distribution
deviating from the prior, a uniform distribution U .

The objective function for a feature node is alike, except
that there is no ﬁrst term, as there are no seed labels for
feature nodes:

(cid:88)

µnp

i∈N (j)

wij|| ˆCj − ˆCi||2 + µpp|| ˆCj − U ||2

(2)

The objective function is jointly optimized for all nodes

in the graph.

The output from EXPANDER is a learned distribution of
semantic labels for every node in the graph. We assign the
top scoring output label as the semantic intent for the node,
labels with low scores are ﬁltered out. Figure 4 illustrates
this process.

To discover new clusters which are not covered by the
labeled examples, we run the semi-supervised learning algo-
rithm in repeated phases. In the ﬁrst phase, we run the label
propagation algorithm for 5 iterations. We then ﬁx the clus-
ter assignment, randomly sample 100 new responses from
the remaining unlabeled nodes in the graph. The sampled
nodes are treated as potential new clusters and labeled with
their canonicalized representation. We rerun label propa-
gation with the new labeled set of clusters and repeat this
procedure until convergence (i.e., until no new clusters are
discovered and members of a cluster do not change between
iterations). The iterative propagation method thereby al-

lows us to both expand cluster membership as well as dis-
cover (up to 5X) new clusters, where each cluster has an
interpretable semantic interpretation.

4.5 Cluster Validation

Finally, we extract the top k members for each semantic
cluster, sorted by their label scores. The set of (response,
cluster label) pairs are then validated by human raters. The
raters are provided with a response Ri, a corresponding clus-
ter label C (e.g., thanks) as well as few example responses
belonging to the cluster (e.g., “Thanks!”, “Thank you.”) and
asked whether Ri belongs to C.

The result is an automatically generated and validated
set of high quality response messages labeled with semantic
intent. This is subsequently used by the response scoring
model to search for approximate best responses to an in-
coming email (described earlier in Section 3) and further
to enforce diversity among the top responses chosen (Sec-
tion 5).

5. SUGGESTION DIVERSITY

As discussed in Section 3, the LSTM ﬁrst processes an
incoming message and then selects the (approximate) best
responses from the target response set created using the
method described in Section 4. Recall that we follow this
by some light normalization to penalize responses that may
be too general to be valuable to the user. The eﬀect of this
normalization can be seen by comparing columns 1 and 2 of
Table 2. For example, the very generic ”Yes!” falls out of the
top ten responses.

Next, we need to choose a small number of options to
show the user. A straight-forward approach would be to just
choose the N top responses and present them to the user.
However, as column 2 of Table 2 shows, these responses tend
to be very similar.

The likelihood of at least one response being useful is
greatest when the response options are not redundant, so it
would be wasteful to present the user with three variations
of, say, I’ll be there. The job of the diversity component is
to select a more varied set of suggestions using two strate-
gies: omitting redundant responses and enforcing negative
or positive responses.

5.1 Omitting Redundant Responses

This strategy assumes that the user should never see two
responses of the same intent. An intent can be thought of as
a cluster of responses that have a common communication
purpose, e.g. conﬁrming, asking for time or rejecting partic-
ipation. In Smart Reply, every target response is associated
with exactly one intent. Intents are deﬁned based on auto-
matic clustering followed by human validation as discussed
in Section 4.

The actual diversity strategy is simple: the top responses
are iterated over in the order of decreasing score. Each re-
sponse is added to the list of suggestions, unless its intent
is already covered by a response on the suggestion list. The
resulting list contains only the highest-scored representative
of each intent, and these representatives are ordered by de-
creasing score.

5.2 Enforcing Negatives and Positives

We have observed that the LSTM has a strong tendency
towards producing positive responses, whereas negative re-
sponses such as I can’t make it or I don’t think so typically
receive low scores. We believe that this tendency reﬂects
the style of email conversations: positive replies may be
more common, and where negative responses are appropri-
ate, users may prefer a less direct wording.

Nevertheless, we think that it is important to oﬀer nega-
tive suggestions in order to give the user a real choice. This
policy is implemented through the following strategy:

If the top two responses (after omitting redun-
dant responses) contain at least one positive re-
sponse and none of the top three responses are
negative, the third response is replaced with a
negative one.

A positive response is one which is clearly aﬃrmative, e.g.
one that starts with Yes, Sure or Of course. In order to ﬁnd
the negative response to be included as the third sugges-
tion, a second LSTM pass is performed. In this second pass,
the search is restricted to only the negative responses in the
target set (refer Table 2 for scored negative response exam-
ples). This is necessary since the top responses produced in
the ﬁrst pass may not contain any negatives.

Even though missing negatives are more common, there
are also cases in which an incoming message triggers exclu-
sively negative responses. In this situation, we employ an
analogous strategy for enforcing a positive response.

The ﬁnal set of top scoring responses (bottom row in Ta-

ble 2) are then presented to the user as suggestions.

6. TRIGGERING

The triggering module is the entry point of the Smart
Reply system. It is responsible for ﬁltering messages that
are bad candidates for suggesting responses. This includes
emails for which short replies are not appropriate (e.g., con-
taining open-ended questions or sensitive topics), as well as
emails for which no reply is necessary at all (e.g., promo-
tional emails and auto-generated updates).

The module is applied to every incoming email just after
the preprocessing step. If the decision is negative, we ﬁnish
the execution and do not show any suggestions (see Fig-
ure 2). Currently, the system decides to produce a Smart

Sure, I’ll be there.
Yes, I can.
Yes, I can be there.
Yes, I’ll be there.
Sure, I can be there.
Yeah, I can.
Yeah, I’ll be there.
Sure, I can.
Yes. I can.
Yes, I will be there.

Unnormalized Responses Normalized Responses
Yes, I’ll be there.
Yes, I will be there.
I’ll be there.
Yes, I can.
What time?
I’ll be there!
I will be there.
Sure, I’ll be there.
Yes, I can be there.
Yes!
Normalized Negative Responses
Sorry, I won’t be able to make it tomorrow.
Unfortunately I can’t.
Sorry, I won’t be able to join you.
Sorry, I can’t make it tomorrow.
No, I can’t.
Sorry, I won’t be able to make it today.
Sorry, I can’t.
I will not be available tomorrow.
I won’t be available tomorrow.
Unfortunately, I can’t.
Final Suggestions
Sure, I’ll be there.
Yes, I can.
Sorry, I won’t be able to make it tomorrow.

Table 2: Diﬀerent response rankings for the message
“Can you join tomorrow’s meeting?”

Reply for roughly 11% of messages, so this process vastly
reduces the number of useless sugestions seen by the users.
An additional beneﬁt is to decrease the number of calls to
the more expensive LSTM inference, which translates into
smaller infrastructure cost.

There are two main requirements for the design of the
triggering component. First, it has to be good enough to
ﬁgure out cases where the response is not expected. Note
that this is a very diﬀerent goal than just scoring a set of re-
sponses. For instance, we could propose several valid replies
to a newsletter containing a sentence “Where do you want
to go today?”, but most likely all of the responses would be
useless for our users. Second, it has to be fast: it processes
hundreds of millions of messages daily, so we aim to process
each message within milliseconds.

The main part of the triggering component is a feedfor-
ward neural network which produces a probability score for
every incoming message. If the score is above some thresh-
old, we trigger and run the LSTM scoring. We have adopted
this approach because feedforward networks have repeatedly
been shown to outperform linear models such as SVM or lin-
ear regression on various NLP tasks (see for example [9]).

6.1 Data and Features

In order to label our training corpus of emails, we use as
positive examples those emails that have been responded to.
More precisely, out of the data set described in Section 7.1,
we create a training set that consists of pairs (o, y), where
o is an incoming message and y ∈ {true, f alse} is a boolean
label, which is true if the message had a response and false
otherwise. For the positive class, we consider only messages
that were replied to from a mobile device, while for negative

we use a subset of all messages. We downsample the negative
class to balance the training set. Our goal is to model P (y =
true | o), the probability that message o will have a response
on mobile.

After preprocessing (described in Section 7.1), we extract
content features (e.g. unigrams, bigrams) from the mes-
sage body, subject and headers. We also use various so-
cial signals like whether the sender is in recipient’s address
book, whether the sender is in recipient’s social network and
whether the recipient responded in the past to this sender.

6.2 Network Architecture and Training

We use a feedforward multilayer perceptron with an em-
bedding layer (for a vocabulary of roughly one million words)
and three fully connected hidden layers. We use feature
hashing to bucket rare words that are not present in the
vocabulary. The embeddings are separate for each sparse
feature type (eg. unigram, bigram) and within one feature
type, we aggregate embeddings by summing them up. Then,
all sparse feature embeddings are concatenated with each
other and with the vector of dense features (those are real
numbers and boolean values mentioned in Section 6.1).

We use the ReLu [13] activation function for non-linearity
between layers. The dropout [22] layer is applied after each
hidden layer. We train the model using AdaGrad [8] opti-
mization algorithm with logistic loss cost function. Similarly
to the LSTM, the training is run in a distributed fashion us-
ing the TensorFlow library [1].

7. EVALUATION AND RESULTS

In this section, we describe the training and test data, as
well as preprocessing steps used for all messages. Then, we
evaluate diﬀerent components of the Smart Reply system
and present overall usage statistics.

7.1 Data

To generate the training data for all Smart Reply models
from sampled accounts, we extracted all pairs of an incom-
ing message and the user’s response to that message. For
training the triggering model (see Section 6), we addition-
ally sampled a number of incoming personal messages which
the user didn’t reply to. At the beginning of Smart Reply
pipeline (Figure 2), data is preprocessed in the following
way:

Language detection The language of the message is iden-
tiﬁed and non-English messages are discarded.
Tokenization Subject and message body are broken into

words and punctuation marks.

Sentence segmentation Sentences boundaries are identi-

ﬁed in the message body.

Normalization Infrequent words and entities like personal
names, URLs, email addresses, phone numbers etc. are
replaced by special tokens.

Quotation removal Quoted original messages and forwarded

messages are removed.

Salutation/close removal Salutations like Hi John and
closes such as Best regards, Mary are removed.

After the preprocessing steps, the size of the training set
is 238 million messages, which include 153 million messages
that have no response.

7.2 Results

The most important end-to-end metric for our system is
the fraction of messages for which it was used. This is cur-
rently 10% of all mobile replies. Below we describe in more
detail evaluation stats for diﬀerent components of the sys-
tem. We evaluate all parts in isolation using both oﬄine
analysis as well as online experiments run on a subset of
accounts.

7.2.1 Triggering results

In order to evaluate the triggering model, we split the
data set described in Section 6.1 into train (80%) and test
(20%) such that all test messages are delivered after train
messages. This is to ensure that the test conditions are
similar to the ﬁnal scenario. We use a set of standard binary
classiﬁer metrics: precision, recall and the area under the
ROC curve. The AUC of the triggering model is 0.854.
We also compute the fraction of triggered messages in the
deployed system, which is 11%. We observed that it may be
beneﬁcial to slightly over-trigger, since the cost of presenting
a suggestion, even if it is not used, is quite low.

7.2.2 Response selection results

We evaluate the LSTM scoring model on three standard
metrics: Perplexity, Mean Reciprocal Rank and Precision@K.

Perplexity.

Perplexity is a measure of how well the model has ﬁt the
data: a model with lower perplexity assigns higher likelihood
to the test responses, so we expect it to be better at pre-
dicting responses. Intuitively, a perplexity equal to k means
that when the model predicts the next word, there are on
average k likely candidates. In particular, for the ideal sce-
nario of perplexity equal to 1, we always know exactly what
should be the next word. The perplexity on a set of N test
samples is computed using the following formula:

Pr = exp(−

1
W

N
(cid:88)

i=1

ln( ˆP (ri

1, ..., ri

m|oi

1, ..., oi

n)))

where W is the total number of words in all N samples, ˆP
is the learned distribution and ri, oi are the i-th response
and original message. Note that in the equation above only
response terms are factored into Pr. The perplexity of the
Smart Reply LSTM is 17.0. By comparison, an n-grams
language model with Katz backoﬀ [11] and a maximum or-
der of 5 has a perplexity of 31.4 on the same data (again,
computed only from response terms).

Response ranking.

While perplexity is a quality indicator, it does not actually
measure performance at the scoring task we are ultimately
interested in.
In particular, it does not take into account
the constraint of choosing a response in R. Therefore we
also evaluate the model on a response ranking task: for each
of N test message pairs (o, r) for which r ∈ R, we compute
s = P (r|o) and ∀i xi = P (wi|o), where wi is the i-th element
of R. Then we sort the set R = {s, x1, . . . , xN } in descending
order. Finally, we deﬁne ranki = argminj(Rj|Rj = s). Put
simply, we are ﬁnding the rank of the actual response with
respect to all elements in R.

Model
Random
Frequency
Multiclass-BOW
Smart Reply

Precision@10 Precision@20

5.58e − 4
0.321
0.345
0.483

1.12e − 3
0.368
0.425
0.579

MRR
3.64e − 4
0.155
0.197
0.267

Table 3: Response ranking

Using this value, we can compute the Mean Reciprocal

Rank:

M RR =

1
N

N
(cid:88)

i=1

1
ranki

Additionally we can compute Precision@K. For a given
value of K it is computed as the number of cases for which
target response r was within the topK responses that were
ranked by the model.

We compare the Smart Reply response selection model
to three baselines on the same ranking task. The Random
baseline ranks R randomly. The Frequency baseline ranks
them in order of their frequency in the training corpus. This
baseline captures the extent to which we can simply suggest
highly frequent responses without regard for the contents of
the original message. The Multiclass-BOW baseline ranks
R using a feedforward neural network whose input is the
original message, represented with bag of words features,
and whose output is a distribution over the elements of R
(a softmax).

As shown in Table 3, the Smart Reply LSTM signiﬁcantly
improves on the Frequency baseline, demonstrating that con-
ditioning on the original message is eﬀective; the model suc-
cessfully extracts information from the original message and
uses it to rank responses more accurately.

It also signiﬁcantly outperforms the Multiclass-BOW base-
line. There are a few possible explanations for this. First,
the recurrent architecture allows the model to learn more
sophisticated language understanding than bag of words fea-
tures. Second, when we pose this as a mulitclass prediction
problem, we can only train on messages whose response is
in R, a small fraction of our data. On the other hand, the
sequence-to-sequence framework allows us to take advantage
of all data in our corpus: the model can learn a lot about
original-response relationships even when the response does
not appear in R exactly.

Note that an added disadvantage of the multiclass formu-
lation is that it tightly couples the training of the model
to the construction of R. We expect R to grow over time,
given the incredible diversity with which people communi-
cate. While a simpler application such as chat might only
need a small number of possible responses, we ﬁnd that for
email we will need a tremendous number of possible sugges-
tions to really address users’ needs.

7.2.3 Diversity results

We justify the need for both the diversity component and
a sizable response space R by reporting statistics around
unique suggestions and clusters in Table 4. The Smart Re-
ply system generates daily 12.9k unique suggestions that
belong to 376 unique semantic clusters. Out of those, peo-
ple decide to use 4, 115, or 31.9% of, unique suggestions and
313, or 83.2% of, unique clusters. Note, however, that many
suggestions are never seen, as column 2 shows: the user may
not open an email, use the web interface instead of mobile

Figure 5: Usage distribution for top suggested re-
sponses.

Unique Clusters
Unique Suggestions

Daily Count
376
12.9k

Seen
Used
97.1% 83.2%
78% 31.9%

Table 4: Unique cluster/suggestions usage per day

or just not scroll down to the bottom of the message. Also,
only one of the three displayed suggestions will be selected
by the user. These statistics demonstrate the need to go
well beyond a simple system with 5 or 10 canned responses.
Figure 5 and Figure 6 present, respectively, the distribu-
tion of the rank for suggested responses and the distribution
of suggested clusters. The tail of the cluster distribution
is long, which explains the poor performance of Frequency
baseline described in Section 7.2.2.

We also measured how Smart Reply suggestions are used
based on their location on a screen. Recall that Smart Reply
always presents 3 suggestions, where the ﬁrst suggestion is
the top one. We observed that, out of all used suggestions,
45% were from the 1st position, 35% from the 2nd position
and 20% from the 3rd position. Since usually the third po-
sition is used for diverse responses, we conclude that the
diversity component is crucial for the system quality.

Finally, we measured the impact of enforcing a diverse set
of responses (e.g., by not showing two responses from the
same semantic cluster) on user engagement: when we com-
pletely disabled the diversity component and simply sug-
gested the three suggestions with the highest scores, the
click-through rate decreased by roughly 7.5% relative.

8. CONCLUSIONS

We presented Smart Reply, a novel end-to-end system for
automatically generating short, complete email responses.
The core of the system is a state-of-the-art deep LSTM
model that can predict full responses, given an incoming
email message. To successfully deploy this system in Inbox
by Gmail, we addressed several challenges:

• We ensure that individual response options deliver qual-
ity by selecting them from a carefully constructed re-
sponse space. The responses are identiﬁed by a novel
method for semantic clustering.

• We increase the total utility of our chosen combina-

 0.0001 0.001 0.01 0.1 0 50 100 150 200 250 300 350 400 450 500Relative usage  (% of total usage count for all suggested responses)Rank of used responses[8] J. Duchi, E. Hazad, and Y. Singer. Adaptive subgradient
methods for online learning and stochastic optimization.
JMLR, 12, 2011.

[9] Y. Goldberg. A primer on neural network models for natural

language processing. CoRR, abs/1510.00726, 2015.

[10] S. Hochreiter and J. Schmidhuber. Long short-term memory.

Neural Computation, 9(8):1735–1780, 1997.

[11] S. M. Katz. Estimation of probabilities from sparse data for the

language model component of a speech recogniser. IEEE
Transactions on Acoustics, Speech, and Signal Processing,
35:400–401, 1987.

[12] X. Li. Understanding the semantic structure of noun phrase
queries. In Proceedings of the 48th Annual Meeting of the
Association for Computational Linguistics (ACL), pages
1337–1345, Uppsala, Sweden, July 2010. Association for
Computational Linguistics.

[13] V. Nair and G. E. Hinton. Rectiﬁed linear units improve

restricted boltzmann machines. In Proceedings of the 27th
International Conference on Machine Learning (ICML-10),
pages 807–814, 2010.

[14] B. Pang and S. Ravi. Revisiting the predictability of language:
Response completion in social media. In Proceedings of the
2012 Joint Conference on Empirical Methods in Natural
Language Processing and Computational Natural Language
Learning, pages 1489–1499, Jeju Island, Korea, July 2012.
Association for Computational Linguistics.

[15] S. Ravi and Q. Diao. Large scale distributed semi-supervised

learning using streaming approximation. In Proceedings of the
19th International Conference on Artiﬁcial Intelligence and
Statistics (AISTATS), 2016.

[16] A. Ritter, C. Cherry, and W. B. Dolan. Data-driven response
generation in social media. In Proceedings of the 2011
Conference on Empirical Methods in Natural Language
Processing, Edinburgh, UK, July 2011. Association for
Computational Linguistics.

[17] R. Saha Roy, R. Katare, N. Ganguly, S. Laxman, and

M. Choudhury. Discovering and understanding word level user
intent in web search queries. Web Semant., 30(C):22–38, Jan.
2015.

[18] H. Sak, A. Senior, and F. Beaufays. Long short-term memory
recurrent neural network architectures for large scale acoustic
modeling. In Proceedings of the Annual Conference of
International Speech Communication Association
(INTERSPEECH), 2014.

[19] I. V. Serban, A. Sordoni, Y. Bengio, A. Courville, and

J. Pineau. Hierarchical neural network generative models for
movie dialogues. In arXiv preprint arXiv:1507.04808, 2015.

[20] L. Shang, Z. Lu, and H. Li. Neural responding machine for

short-text conversation. In In Proceedings of ACL-IJCNLP,
2015.

[21] A. Sordoni, M. Galley, M. Auli, C. Brockett, Y. Ji, M. Mitchell,
J.-Y. Nie, J. Gao, and B. Dolan. A neural network approach to
context-sensitive generation of conversation responses. In In
Proceedings of NAACL-HLT, 2015.

[22] N. Srivastava, G. Hinton, A. Krizhevsky, I. Sutskever, and

R. Salakhutdinov. Dropout: A simple way to prevent neural
networks from overﬁtting. Journal of Machine Learning
Research, 15:1929–1958, 2014.

[23] I. Sutskever, O. Vinyals, and Q. V. Le. Sequence to sequence

learning with neural networks. Advances in Neural
Information Processing Systems (NIPS), 2014.

[24] O. Vinyals and Q. V. Le. A neural conversation model. In

ICML Deep Learning Workshop, 2015.

[25] O. Vinyals, A. Toshev, S. Bengio, and D. Erhan. Show and tell:
A neural image caption generator. In Proceedings of IEEE
Conference on Computer Vision and Pattern Recognition
(CVPR), 2015.

[26] J. B. Wendt, M. Bendersky, L. Garcia-Pueyo, V. Josifovski,
B. Miklos, I. Krka, A. Saikia, J. Yang, M.-A. Cartright, and
S. Ravi. Hierarchical label propagation and discovery for
machine generated email. In Proceedings of the International
Conference on Web Search and Data Mining (WSDM)
(2016), 2016.

[27] X. Zhu, Z. Ghahramani, and J. Laﬀerty. Semi-supervised
learning using gaussian ﬁelds and harmonic functions. In
Proceedings of the International Conference on Machine
Learning (ICML), pages 912–919, 2003.

Figure 6: Usage distribution for semantic clusters
corresponding to top suggested responses.

tion of suggestions by enforcing diversity among them,
and ﬁltering traﬃc for which suggestions would not be
useful.

• We build a scalable system by eﬃciently searching the

target response space.

Our clearest metric of success is the fact that 10% of mo-
bile replies in Inbox are now composed with assistance from
the Smart Reply system. Furthermore, we have designed the
system in such a way that it is easily extendable to address
additional user needs; for instance, the architecture of our
core response scoring model is language agnostic, therefore
accommodates extension to other languages in addition to
English.

9. ACKNOWLEDGMENTS

The authors would like to thank Oriol Vinyals and Ilya
Sutskever for many helpful discussions and insights, as well
as Prabhakar Raghavan for his guidance and support.

10. REFERENCES
[1] M. Abadi, A. Agarwal, P. Barham, and et al. Tensorﬂow:

Large-scale machine learning on heterogeneous systems. 2015.

[2] I. G. P. Aﬀairs. Interconnected world: Communication & social

networking. Press Release, March 2012. http:
//www.ipsos-na.com/news-polls/pressrelease.aspx?id=5564.
[3] Y. Artzi, P. Pantel, and M. Gamon. Predicting responses to

microblog posts. In Proceedings of the 2012 Conference of the
North American Chapter of the Association for
Computational Linguistics: Human Language Technologies,
pages 602–606, Montr´eal, Canada, June 2012. Association for
Computational Linguistics.

[4] L. Backstrom, J. Kleinberg, L. Lee, and

C. Danescu-Niculescu-Mizil. Characterizing and curating
conversation threads: Expansion, focus, volume, re-entry. In
Proceedings of the Sixth ACM International Conference on
Web Search and Data Mining, WSDM ’13, pages 13–22, 2013.

[5] Y. Bengio, O. Delalleau, and N. Le Roux. Label propagation
and quadratic criterion. In O. Chapelle, B. Sch¨olkopf, and
A. Zien, editors, Semi-Supervised Learning, pages 193–216.
MIT Press, 2006.

[6] W. Chan, N. Jaitly, Q. V. Le, and O. Vinyals. Listen, attend,

and spell. arXiv:1508.01211, abs/1508.01211, 2015.
[7] Z. Chen, B. Liu, M. Hsu, M. Castellanos, and R. Ghosh.

Identifying intention posts in discussion forums. In Proceedings
of the 2013 Conference of the North American Chapter of the
Association for Computational Linguistics: Human Language
Technologies, pages 1041–1050, Atlanta, Georgia, June 2013.
Association for Computational Linguistics.

 0.01 0.1thankswill dono i did ntsounds goodthanks for the updatei got itgreat thankssee youhere you golove itlooks goodyes i amno problemthanks for the helpok thanksi ll be therethat s finegreatnotedthanks for emailRelative usage(% of total usage count for semantic clusters)
