Source: https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45908.pdf

---

Template Induction over Unstructured Email Corpora

Julia Proskurnia† Marc-Allen Cartright‡

Lluís Garcia-Pueyo‡

Ivo Krka‡

James B. Wendt‡

†EPFL

Tobias Kaufmann‡

Balint Miklos‡

‡Google, Inc.

†iuliia.proskurnia@epﬂ.ch
‡{mcartright, lgpueyo, krka, jwendt, snufkin, bal}@google.com

ABSTRACT
Unsupervised template induction over email data is a central
component in applications such as information extraction,
document classiﬁcation, and auto-reply. The beneﬁts of au-
tomatically generating such templates are known for struc-
tured data, e.g. machine generated HTML emails. However
much less work has been done in performing the same task
over unstructured email data.

We propose a technique for inducing high quality tem-
plates from plain text emails at scale based on the suﬃx
array data structure. We evaluate this method against an
industry-standard approach for ﬁnding similar content based
on shingling, running both algorithms over two corpora: a
synthetically created email corpus for a high level of exper-
imental control, as well as user-generated emails from the
well-known Enron email corpus. Our experimental results
show that the proposed method is more robust to variations
in cluster quality than the baseline and templates contain
more text from the emails, which would beneﬁt extraction
tasks by identifying transient parts of the emails.

Our study indicates templates induced using suﬃx ar-
rays contain approximately half as much noise (measured
as entropy) as templates induced using shingling. Further-
more, the suﬃx array approach is substantially more scal-
able, proving to be an order of magnitude faster than shin-
gling even for modestly-sized training clusters.

Public corpus analysis shows that email clusters contain
on average 4 segments of common phrases, where each of
the segments contains on average 9 words, thus showing that
templatization could help users reduce the email writing ef-
fort by an average of 35 words per email in an assistance or
auto-reply related task.

Keywords
Human-generated email; structural template; ﬁxed phrase
extraction; templatization; suﬃx array generalization; EN-
RON corpus.

2017 International World Wide Web Conference Committee (IW3C2),

c
(cid:13)
published under Creative Commons CC-BY-NC-ND 2.0 License.
WWW 2017, April 3–7, 2017, Perth, Australia.
ACM 978-1-4503-4913-0/17/04.
http://dx.doi.org/10.1145/3038912.3052631

1.

INTRODUCTION

Template induction, the technique of generating a skele-
ton of repeated content based on previously seen examples,
has seen substantial success for structured content such as
web pages, where metadata such as the underlying DOM1
provides multiple presentational and structural signals that
can be exploited algorithmically. These structures can be
useful for tasks such as automatic labeling, plagiarism de-
tection, duplicate detection, and structured information ex-
traction. Despite the success of template induction for struc-
tured data, we have found little prior research for the same
task, but for data that is not explicitly structured (i.e. plain
text). This duality has diﬃcult implications for a domain
such as email. Despite often having some amount of struc-
ture, emails almost always contain some signiﬁcant portion
of freeﬂowing plain text that have, to date, not yet been
suﬃciently modeled in induced structured templates.

In this paper, we develop a template induction algorithm
that focuses on the plain text content. We use email as the
target domain, as we envision two potentially high-impact
applications of templates generated for plain text content:
1) structured information extraction, where particular im-
portant pieces of information in the email are extracted; 2)
email autocompletion, where the system suggests content
to add during the composition of an email, based on the
already present content the user has added; and 3) facilita-
tion of the spam detection and ﬁltering. Although the po-
tential beneﬁts of templatizing users emails are considerable
(email autocompletion etc), targeting email documents pro-
vides nontrivial challenges in addition to the lack of explicit
structure. Unlike the public domain for web pages, email
documents are virtually always considered private, making
it diﬃcult to obtain training data. This is a sharp contrast
to the freely observable and highly-structured web domain.
Consequently, there are vastly fewer suitable datasets avail-
able for this kind of investigation, and we were unable to ﬁnd
any direct prior research on this topic. Given this setting,
the primary task becomes one of establishing that template
induction can be eﬀective for the unstructured content. We
look to further reduce the email response cost to users by
investigating the usefulness of a template suggestion mech-
anism that is initiated when composing emails from a set of
automatically constructed templates.

A template creation method consists of two parts: First,
clustering similar messages. Second, for each cluster, deter-
mining the parts which are considered “ﬁxed” and storing

.

1http://wikipedia.org/wiki/Document Object Model

the information in a standard representation, which is the
produced template. In this paper, we focus on the latter.

To determine the ﬁxed regions, we use an implementation
of the suﬃx array data structure [24], which is eﬃcient in
space and time complexity, and can be easily parallelized.
We show that the quality of produced templates created
with our approach is consistently better than the baseline
regardless of the quality of the clusters and with better la-
tency performance. The results of the public corpora analy-
sis determine that text suggestion would aﬀect a signiﬁcant
number of users and would save them a signiﬁcant volume
of writing in an autocompletion task. In addition, we show
that the portion of emails detected as ﬁxed-text is larger
than for the baseline, which would allow an automated in-
formation extraction system to focus on fewer parts of the
emails when extracting transient information.

To determine the eﬀectiveness of using a suﬃx array to
generate templates, we compare it against a standard base-
line approach for template creation. We test both methods
on a synthetically generated corpus as well as a publicly
available corpus of emails from the Enron Corporation2.
The results of these experiments indicate that the suﬃx ar-
ray serves as a superior approach to correctly identifying an
optimal number and span of ﬁxed regions.
The main contributions of this work are:

•

•

•

•

An extensive analysis of the feasibility of email templa-
tization for emails sent by a given user or bulk sender;
A scalable technique that results in high quality tem-
plates regardless of the clustering quality;
A novel application of the generalized suﬃx array al-
gorithm to detect common phrases over similar emails;
and
An evaluation of the eﬃciency and quality of both the
suﬃx array and baseline approaches.

The rest of the paper is organized as follows. Section 2 dis-
cusses prior work in the area of email template creation. Sec-
tion 3 describes the template creation task in detail as well
as our suﬃx-array based approach to generating templates
from pre-formed clusters. Section 4 describes the experi-
mental setup for comparative analysis, and concludes with
the results of those experiments. Finally, Section 5 presents
further applications and potential future work based on the
results of this study.

2. RELATED WORK

In this section we discuss state of the art techniques re-
lated to this work. Speciﬁcally, we cover methods for email
content mining (e.g. spam classiﬁcation, labeling, and thread-
ing), template induction (for web and for emails), and auto-
completion systems.

2.1 Email Content Mining

Most email content mining techniques are originally de-
rived from more established web information extraction meth-
ods, such as template or wrapper induction [5, 11, 15, 16,
22].
In addition to information extraction, email content
mining techniques also span document classiﬁcation tasks,
such as spam ﬁltering, automatic labeling, as well as docu-
ment clustering for email threading.

Spam classiﬁcation. The popularity and necessity of
email as a communication medium has also made email a

2https://www.cs.cmu.edu/˜./enron/

popular target for spam attacks. Simple manual spam ﬁl-
tering rules have given way in the last decade to more com-
plex and eﬀective machine learning systems that now serve
as the defacto defenders tasked with detecting and removing
spam messages from inboxes [4, 21, 26]. More recently, these
binary classiﬁcation have expanded beyond textual classiﬁ-
cation to include much richer feature sets, collaborative ﬁl-
tering techniques, and peer-to-peer and social networking
ontology-based semantic spam detection techniques [7, 8].

Label classiﬁcation and ranking. The expansion of
email as one of the primary communication media in both
personal and commercial use has led to the notion of email
overload, in which users become overwhelmed when the rate
of incoming messages in their inbox outpaces the rate at
which they can process those messages [9]. Automatic email
foldering has been proposed to alleviate this problem [6, 14,
19]. However, these works present methods for email orga-
nization based on the underlying context of each message
rather than occurrences of speciﬁc strings.

In many of these scenarios, sparsity of labeled data re-
mains a hindrance to accurate and robust model develop-
ment. Kiritchenko and Matwin deal with the sparsity is-
sue by using a co-training algorithm to build weak classi-
ﬁers, then label unlabeled examples, and add the most conﬁ-
dent predictions to the labeled set [13]. Somewhat similarly,
Wendt et al. utilize a graph-based label propagation algo-
rithm to label unlabeled emails from a small set of labeled
emails, but do so at the template level to improve scalability
in very large mail provider systems [25].

Possibly one of the most popular and widely known au-
tomatic email organization systems is Google’s Gmail prior-
ity inbox, which distinguishes between important and non-
important emails by predicting the probability that the user
will interact with the email (e.g. open, respond) within some
time window from delivery [1].

Threading. Email threading is another solution to the
email overload problem that assists in inbox organization
and can furthermore reduce the user’s perceived inbox load
by clustering emails from the same conversation together
[18]. Current threading techniques cluster messages together
by header information, such as sender, subject, and sub-
ject preﬁxes (e.g.
‘Re:’, ‘Fwd:’). Personal correspondence
emails are generally threaded very accurately using this tech-
nique, however, many commercial emails, such as purchase
receipts, tracking numbers, and shipment conﬁrmations are
often split into multiple threads due to their diﬀerent subject
lines despite arriving from the same sender domain and be-
longing to the same semantic thread. Ailon et al. presented
techniques to thread such commercial emails through lever-
aging email templates and learning temporal causal rela-
tionships between emails from similar senders [2]. Similarly,
Wang et al. attempt to recover implicit threading struc-
tures by sorting messages by time and construct a graph of
conversations of the same topic, however their analysis is
limited to newsgroup style conversations [23].

2.2 Template Induction

Web data is generally formatted in a human-readable for-
mat which a machine renders might not necessarily under-
stand. Web extraction techniques have been proposed to
solve this issue of extracting information structured for hu-
man consumption from data.

Figure 1: An overview of the clustering and template induction.

The web is comprised of over a trillion documents in the
public domain [3], many of which are dynamically created
and generated using templates. Hence, web information ex-
traction is a well explored topic and is often closely coupled
with template induction techniques. Since many emails uti-
lize HTML markup and it is estimated that nearly 60% of
emails are created from templates (e.g. B2C emails) [2],
it is natural to also apply similar web-based techniques for
template induction and information extraction on emails.
However, emails are among the most sensitive data on the
Internet. Hence, little research has been presented on email
template induction due to privacy constraints, although re-
cent work has proposed methods for enforcing anonymity in
web mail auditing [10].

While there is very little published work on using struc-
tural templates for processing commercial email data, tem-
plates have been used for annotating semantic types within
the DOM trees of emails [27] and used in hierarchical clas-
siﬁcation of emails [25]. To our knowledge, no techniques
have yet been published that propose template induction
for plain text email content.

[17] summarizes the short messages about same events
into their shorter representaton. However, it has two ma-
jor drawbacks that are not suited for the email use case.
First, clustering of the messages relies on the edit distance
which does not scale well over average size emails and might
produce clusters where all words are diﬀerent. Second, the
method requires strong preprocessing.

2.3 Assisted Email Composition

SmartReply is the ﬁrst email-speciﬁc machine-learned tool
designed to assist the user in composing email. The tool is
built on recurrent neural networks (one to encode the in-
coming email and the other to predict possible responses)
that automatically suggests replies to email messages [12].
The work presented here aims to provide assistance that is
learned speciﬁcally from an individual email sender, whereas
SmartReply provides canned responses meant to satisfy as
many users as possible. In a assisted email composition con-
text SmartReply would infer intent, while our work would
detect content that was written before by the same sender.

3. METHODOLOGY

The design of the template induction system is shown in
Figure 1. We ﬁrst describe the preprocessing and clustering
steps which generate the input for the template induction
algorithms. We then present two approaches for the ﬁxed
phrase extraction, as well as template induction algorithm.

3.1 Preprocessing

During the preprocessing phase, we perform necessary en-
richment and ﬁltering of the raw input emails to make them
suitable for use as experimental input for comparison.

For each email in the raw corpus, we determine if the mes-
sage is a reply (its subject begins with the pattern re:) or
a forward (its subject begins with the pattern fwd:) of a
prior email. All other emails are treated as original mes-
sages. Any non-original message is analyzed, and if all of
the content of the message is simply a quote of the original
message, the email is ﬁltered out. Of the remaining emails,
all messages determined to be non-English (or consisting pri-
marily of non-English content) are additionally ﬁltered out.
Each of the remaining emails is then tokenized and each pro-
duced token is a structure that carries the original form of
the token as well as its lemma, using the WordNet database
for lemmatization [20].

3.2 Clustering

After normalization and ﬁltering, we then cluster similar
emails as follows. Given the task at hand, a natural basis
for similarity is to ﬁrst group all emails sent from the same
email address together. Each of these initial groups is then
further processed to produce the ﬁnal set of email clusters,
which are then passed as input to the template generation
algorithms.

Formally, let Di and Dj be two emails in our corpus, rep-
resented as term count vectors. We deﬁne the distance be-
tween two emails:

δ(Di, Dj) =

(cid:13)
(cid:13)
(cid:13)
(cid:13)

Di
Di

(cid:107)

(cid:107)

1 −

(cid:107)

(cid:13)
(cid:13)
(cid:13)
(cid:13)2

Dj
Dj

1
(cid:107)

(1)

δ

≤

≤

which we use as a measure when constructing the ﬁnal set
√2
of clusters. Note that based on this deﬁnition, 0
(√2 indicates orthogonal document vectors). A maximal
distance indicates that two documents have disjoint vocab-
ularies, while minimal distance indicates that, at the very
least, the token frequency histograms of the two documents
are identical. This measure does not account for token or-
dering diﬀerences; we assume that statistical similarity is
suﬃcient when considering documents from a single sender.
We use the distance deﬁned in Equation 1 and a given dis-
tance threshold θ
range(δ) to partition each input sender-
based group into smaller clusters based on email distances.
Using these deﬁnitions, we present Algorithm 1, which re-
ceives an input cluster Cin (e.g. every email sent by a given
user or bulk sender), and a threshold θ to produce a set of
output clusters Cout

The InitializeCluster function adds a new cluster to
the output set Cout, and places D in the new cluster as
the “representative” of that cluster. The Rep function re-
turns the assigned representative email of a given cluster,
e.g., the ﬁrst email added to the cluster. While we could
drop this assumption and attempt to ﬁnd the best represen-
tative email for the entire cluster, performing this operation
reduces to an instance of the set cover problem, which is

3.

∈

3The large volume of emails in a real-world scenario makes
the usage of complex clustering techniques not scalable. Al-
though cluster creation is not the focus of this work, we
observed that Algorithm 1 and k-means clustering did not
show any signiﬁcant diﬀerences in the quality of the result-
ing clusters, however, the method in Algorithm 1 showed a
signiﬁcant gain in speed.

Fixed phrase extractionFilteringNormalizationInput Documents(Outbox)ClusteringEmailClustersFixed PhrasesTemplatesTemplate constructionAlgorithm 1 Creating distance-based clusters.

Algorithm 2 Baseline method for ﬁnding ﬁxed text.

∈

{}
Cin
if Cout = =

ProcessClusters(Cin, θ)
1 Cout =
2 for D
3
4
5
6
7
8
9 return Cout

InitializeCluster(Cout, D)

∅
else Cbest = argminC∈Cout

if SIM (D, Rep(Cbest)) > θ

δ(D, Rep(C))

Cbest = Cbest

D

else InitializeCluster(Cout, D)

∪ {

}

known to be NP-complete. Although we may be able to
ﬁnd the optimal representative for some smaller-scale sets,
such an approach would not scale to real-world collections.
Therefore we use the pre-selected representative to keep the
problem tractable.

Line 1 initializes an empty result, where the main itera-
tion over the input cluster emails occurs on lines 2–8. We
initialize the ﬁrst output cluster with the ﬁrst email in line 4.
For each subsequent email, we calculate the distance of the
email from all the representatives. If the best score is greater
than θ, the email is added to the cluster with the best score;
otherwise it creates a new cluster, with the email set as the
representative (lines 5–8). When all emails are processed,
the resulting set of clusters is returned in line 9. Each of the
ﬁnal clusters represents a “template” of an email - each email
in the cluster is a minor variant of a mostly static template.

3.3 Baseline Phrase Extraction

We now describe the two methods we compare when con-
In both cases, we assume the input
ducting experiments.
documents have already been clustered based on our selected
distance metric. The task is to determine the parts of con-
tent that are frequent enough in the cluster to consider them
“ﬁxed”, which we can subsequently use to construct a tem-
plate representing the clustered emails.

We adopt a greedy version of a longest common subse-
quence algorithm as a baseline approach. To identify ﬁxed
phrases for the templatization task, our baseline algorithm
operates sequentially on emails of a given cluster. Pseu-
docode of the algorithm is presented in Algorithm 2. We
1.0 as a threshold for determining
deﬁne the input 0
if a token is ﬁxed. Additionally, let ti be the ith token in an
email vector i.e., D = t0 . . . t|D|−1. A token will be classiﬁed
C
as ﬁxed if it is present in γ
documents. Given a cluster
C
Cout from the clustering step, and a value for γ, the
algorithm will return a set of terms considered as ﬁxed for
the given cluster.

∗ |

≤

≤

∈

γ

|

On line 1, we iterate over C to calculate the document
frequencies of the unique tokens in C, and store the tabu-
lated data in df . Line 2 initializes the acc variable, which
acts as an accumulator for the frequency counts of observed
phrases. Lines 3–11 loop over every email in C, ﬁlling acc
with candidate phrases. The function InsertInc inserts the
entry if it does not exist, or increments the count of the
existing entry. Lines 5–11 construct the candidate phrases
by iterating over the token sequences from the current D.
The phrase (line 4) variable tracks the “current” candidate

C

{}
∈

phrase = []
for i = 0 to
if df [ti]

D
1
| −
|
C
γ
∗ |
≥
Append(phrase, ti)

BaselineExtractPhrases(C, γ)
1 df = DocumentFrequencies(C)
2 acc =
3 for D
4
5
6
7
8
9
10
11
12
13
14 RemoveInfrequent(acc, γ
15 return Keys(acc)

InsertInc(acc, phrase, 1)

phrase
|

phrase
|

phrase = []

else

> 0

> 0

∗ |

C

if

if

)

|

|

|

|

InsertInc(acc, phrase, 1)

∗ |

|

phrase. If a token has a high enough document frequency, it
is appended to the current phrase (lines 6–7). Otherwise if
the current phrase is non-empty, its count is incremented in
acc, and the phrase list is reset to empty (lines 9–11). The
ﬁnal step on line 14 involves iterating over the entries in the
acc variable, and removing any candidate phrases that are
below the γ

threshold.

C

One of the major advantages of this approach is that the
space and time complexity constraints of the algorithm are
both linear with respect to the input size. Both aspects of
the algorithm are
max is the length
of the longest email in C. Constructing df requires a scan
over each email in C, while the execution of Algorithm 2
is a linear scan over the emails in C.
In terms of space
complexity, the greedy construction of the candidate phrase
table makes the space requirements be linear as well.

max), where

(
|

D

D

O

C

||

|

|

|

3.3.1 Limitations

While Algorithm 2 is straightforward in its execution, it
suﬀers from the assumption that frequent tokens tend to co-
occur with each other. Only the longest identiﬁed phrases
will be computed for the given emails; any subphrases that
may also pass the frequency threshold, but are not in the
same order or consecutive, will not be included in the out-
put set of ﬁxed phrases unless they occur as unique phrases
elsewhere in the emails. For example, if the current tracked
phrase is “Hi your order is here”, the potentially higher-
frequency phrase “your order is here” will not be added as
a resulting ﬁxed phrase simply because it occurs as a sub-
phrase. Let us consider the following two clusters with 5
emails each, with 5 words in each document:
C1 : (A B C D E),(A B C D F),(A B C D G),(A B Q C D)
C2 : (A B C D E),(E A B C D),(A X C Y E),(A K C L E)
= 2 for this example. For the ﬁrst cluster
C1, the resulting ﬁxed phrase would be A B C D, since
it is greedily constructed and passes the frequency checks.
However, because A B C D was greedily constructed with
the ﬁrst three emails, the more useful ﬁxed phrase pair A
B and C D are not considered, resulting in a template with
suboptimal coverage over its constituent emails. For the

Let γ

∗ |

C

|

second cluster C2, the resulting ﬁxed phrases would be A, C
and E, while more optimal A B C D and E are not emitted.

3.4 Sufﬁx Array Based Approach

In order to overcome the limitations discussed in the previ-
ous section, we introduce an algorithm to perform template
induction based on a suﬃx array. Since the performance and
precision of the extracted phrases play an important role in
template extraction and user proﬁling, we examine both the
quality and scalability characteristics of this approach.

Our approach uses two main data structures to compute
ﬁxed phrases. The ﬁrst is a suﬃx array (SA), which is the
lexicographically sorted array of all suﬃxes of the input doc-
uments, i.e., pointers to the original positions. SA typically
operate over the character space of the input, however in or-
der to ensure that we produce valid ﬁxed phrases, we need
the SA to operate on the token space. Therefore, when con-
structing the SA, we only permit suﬃxes to be added at
standard token separators such as whitespace and punctu-
ation. The second data structure is an array of the longest
common preﬁx (LCP), which is produced while computing
the SA. Entries in the LCP correspond to the number of
common characters in the preﬁxes between two consecutive
suﬃxes in the SA.

∈

Algorithm 3 provides a sketch of the ﬁxed phrase selection
N to be a thresh-
process using SA and LCP. We deﬁne µ
old for the minimum number of shared characters allowed
between two suﬃxes, and provide it as an input argument.
In line 1, we initialize an accumulator acc, and we construct
the SA and LCP structures. In this instance, acc has the
added functionality of maintaining the insertion order of the
entries, which will be needed in Algorithm 3. Practically
speaking, this can be achieved by internally maintaining
both a table and list to accomodate both access patterns.

The main loop of the algorithm (lines 3–15) iterates over
the contents of the SA, using each iteration to examine a
particular suﬃx and then decide whether to track it as a
candidate ﬁxed phrase. On line 4 we only admit suﬃxes
that have a high enough overlap with the previous value;
all admitted suﬃxes then have their counts incremented on
line 54. The Phrase function extracts the actual phrase
from the input by its position (SA) and length (LCP).

The next action depends on the delta of the “current”
LCP ; when there is a decrease in the LCP , we know that
the currently tracked phrase has ended, and we need to check
its frequency (lines 6–11). The completed phrase’s count is
updated (lines 7–11). The PrevLarger function emits all
previously inserted acc entries as long as the corresponding
LCP values are higher than the current value. Similarly,
the PrevSmaller function emits contiguous prior entries
with lower corresponding LCP values. If the frequency of
the recovered phrases is below the γ
, then the phrase is
dropped from acc. Alternatively, if the LCP increases, this
indicates that a new phrase has started, and we need to in-
crement (or insert) it and all contained subphrases (lines 12–
15). In the case where the LCP delta is zero, no additional
action is taken. After the loop completes, the remaining
keys in acc are returned as the ﬁxed phrases (line 16).

∗ |

C

|

4 Since all the documents are treaded as a single string dur-
ing the SA construction, we maintain an additional data
structure D that contains indexes of beginnings of the doc-
uments. Thus, ids of the documents are obtained with SA.

Algorithm 3 Fixed phrase extraction based on SA, LCP.

; SA, LCP = BuildSuffixArray(C)

InsertInc(acc, Phrase(SA[i], LCP [i
if LCP [i] < LCP [i

1]

1

{}

SA
|

| −
if LCP [i] > µ

ExtractPhrases(C, γ, µ)
1 acc =
2 InsertInc(acc, Phrase(SA[0], LCP [0]), 1)
3 for i = 1 to
4
5
6
7
8
9
10
11
12
13
14
15
16 return Keys(acc)

elseif LCP [i] > LCP [i

if acc[phrase] < γ

∗ |

∈

InsertInc(acc, phrase, 1)

−
c = acc[Phrase(SA[i], LCP [i
InsertInc(acc, Phrase(SA[i], LCP [i]), c)
PrevLarger(acc, LCP [i])
for phrase
C

1])]

−

∈

−
InsertInc(acc, Phrase(SA[i], LCP [i]))
for phrase

PrevSmaller(acc, LCP [i])

RemoveKey(acc, phrase)
1]

1]), 1)

−

|

“ A B ” : 4

ID LCP SA
9
1
9
2
5
3
0
4
7
5
7
6
3
7
0
8
9
...
. . .
. . .

1 A B C D E...
11 A B C D F...
21 A B C D G...
31 A B Q C D...
3
B C D E ...
13 B C D F ...
23 B C D G...
33 B Q C D
47 C D
. . .
. . .

Table 1: LCP, SA and
actual suﬃxes ordered
lexicographically.
Sen-
tence starts with space.

“ A B C D ” : 3

“ B C D ” : 3

Let us again consider the simple example from the end
of Section 3.3.1. Table 1 provides a view of the contents
of the SA and LCP after constructing them over the exam-
ple emails. Recall that the SA is an array with pointers to
the suﬃxes’ positions in the original input, (e.g., 1, 11, 21,
and so on), and the LCP stores the number of shared char-
acters between two consecutive suﬃxes. For the course of
the example, we make the following assumptions: the clus-
ter contains only the suﬃxes present in Table 1, each suﬃx
comes from a diﬀerent document 5 , and γ

= 3.

C

We start with the ﬁrst suﬃx “A B C D ”, which belongs to
the ﬁrst document. The suﬃx has an overlap of 9 characters
with the next suﬃx (i.e., there are at least two documents
that have a repeated phrase of length 9 including spaces)
and thus we insert the phrase into acc with count 1 (line 5).
As we progress in the example, we see the decrease of the
LCP between IDs 3 and 4 which is valid, i.e., number of
remaining overlapping characters passes µ. A negative LCP
delta indicates that the suﬃx has shortened, and the current
phrase has ended. In this case, its accumulated frequency
is checked, the phrase passes, and it is emitted. We observe
that the LCP value drops to 5 characters, thus the count
of the corresponding suﬃx should include the frequency of
the previous larger phrases, and acc is updated accordingly
(line 7-8). As a result, “A B ” is added to acc with count

∗ |

|

5In the algrithm 3 we proceed ensure that phrase increment
only happen for phrases in diﬀerent document.

3. When the LCP increases, the frequency of the current
tracked phrase should continue to accumulate and longer
phrases should be added to acc with count 1 (lines 12–15).
Following this example to its termination, we would produce
A B C D, A B, C D for the ﬁrst cluster and A B C D, E for
the second one, which prove to be more optimal selections
than those produced by Algorithm 2.

p / l

/ 2001 is now available

Template 1 : The report name :
published as of
for view on the website .
Template 2 : We have received the executed
Letter Agreement date
00
amending the ... . Copy will be distributed .
Template 3 : Please , put it on my

/ 2

. Vince

,

|

|

(

||

C

C

O

D

The computation complexity consists of two factors: suf-
ﬁx array construction and ﬁxed phrase extraction loop. The
former is
max) complexity. The latter is propor-
tional to the input size, or more preciesly, proportional to
the number of words in the input. Overall, the complexity
is

O
The algorithm also has modest space demands, since it
only requires the following input: the suﬃx array and the
longest common preﬁx array, both of which are proportional
to the input size and store only pointers to the original input.
During operation, the only data structure maintained is the
output argument, the ﬁnal set of ﬁxed phrases.

max).

(
|

D

||

|

The algorithm aﬀords several opportunities for paralleliza-
tion. For example, each part of the suﬃx array starts with
a diﬀerent letter, and can be processed independently. Ad-
ditionally, instead of partially rescanning the suﬃx array
when there is a change in the current LCP value, a new
process/thread can be spawned that will be responsible for
updating the occurrences of the bigger phrase.

3.5 Constructing a Template from Phrases

We now describe the process of building a template based
on the induced ﬁxed phrases. We design the template itself
to be an ordered list of ﬁxed and non-ﬁxed phrases. We de-
ﬁne the coverage of a given template/email pair to be the
fraction of characters of the email that can be aligned with
the ﬁxed text present in the template. It is an important
measure since it describes an email comression, i.e., number
of characters that might be saved while typing or while rep-
resenting an email through the ﬁxed and non-ﬁxed regions
etc.

The main task is to align the ﬁxed phrases with the follow-
ing optimization criterion: choose a set of non-overlapping
phrases that maximize the coverage over the email. Funda-
mentally the process of template building involves dynamic
programming to align the ﬁxed phrases of the template onto
the email.6

When the alignments of the phrases to the email are found,
the email is transformed into the sequence of the matched
ﬁxed phrases separated by the parts of the template which
were not mapped to a ﬁxed phrase, and are presumed to
contain variable content. For example, if we have 2 ﬁxed
phrases: “hi”, “how are you” and the email is “hi John, how
are you”, we would like to generate the template “hi
how are you”. Example templates generated using our tech-
niques on the Enron corpus are presented in Table 2.

Overall, the quality of the templates is hard to evalu-
ate and can be either performed by humans or automati-
cally. Human evaluation is rather expensive and error prone.
Therefore, we rely on the coverage metric as a reﬂectino of
the cluster edit distance.

6A more detailed description is omitted due to complexity
and limits on space.

Table 2: Examples of the templates created based on SA.

correspond to the non-ﬁxed regions of the templates.

4. EXPERIMENTS

In this section we describe the experimental setup, data
sources and insights we have obtained from both the baseline
and suﬃx array based approaches. We perform two main ex-
periments to analyze the quality of the templates produced
by the two presented methods. We conduct the same exper-
iment with two separate corpora: a synthetically generated
corpus and a real email corpus from the Enron Corporation.
We continue to use the coverage over emails for quality as-
sessment, and we introduce the template entropy measure,
which is the proportion of ﬁxed phrases that a template
contains. More ﬁxed phrases in the template indicate more
variable content separating it, thus introducing more uncer-
tainty which we aim to minimize. Using these measures and
given an induced template, our goal is to maximize cover-
age and minimize template entropy. To test the robustness
of the proposed approach we have performed multiple runs
varying clustering threshold θ and ﬁxed phrase document
frequency γ.

4.1 Synthetic Corpus

Since the algorithm could be run over all user’s emails,
it is important to know how sensitive the template creation
algorithms are to cluster quality. We test both methods
against clusters of varying quality, so in order to perform
these tests while minimizing confounding factors from the
input, we use a synthetically generated corpus of emails,
which is constructed as follows. We automatically gener-
ated 3 independent sets of 100 emails each. For each set we
create 10 clusters with 10 emails each. For a given cluster,
we selected a set of predeﬁned “ﬁxed” phrases that we then
separated in each email by randomly generated text that
acted as the “non-ﬁxed” portion of the email. For example,
in a cluster with two predeﬁned ﬁxed phrases, we randomly
chose phrases to put before, between and after the ﬁxed
phrases for each email in the cluster.

To ensure that uniform email size did not confound our re-
sults, we create another synthetic set where the cluster sizes
are distributed normally instead of uniformly. Table 3 pro-
vides details on the generated corpora. The average coverage
per template of cluster sizes is about 80%, and the average
template entropy is 3. The randomly generated emails had
an average size of 260B, which is in the 92nd percentile of
email sizes in the public corpus.

We characterize the templatization performance by vary-
ing two parameters that are speciﬁed prior to processing as
described in Section 3: the clustering threshold θ and the
ﬁxed phrase document frequency γ. We found that with
θ
0.6 all synthetic emails were grouped into one cluster,
while for θ = 0.7, 0.8, 0.9 average cluster sizes were 20, 11,
6 respectively. Since generation of the ﬁxed and variable

≤

Figure 2: Average template coverage and entropy for two synthetically generated corpuses, i.e., equally and normally distributed
cluster sizes. We present the coverage by varying clustering threshold θ and ﬁxed phrase frequency γ. Suﬃx Array based approaches
consistently show higher coverage (portion of the email marked as ﬁxed) with lower Template Entropy (number of ﬁxed-phrases per
template). Template coverage of a cluster is computed for each email and averaged for the whole cluster.

Metric
Cluster size

Syn1
U

N

Syn2
U

N

Syn3
U

N

Mean
U

N

Coverage (%)
Entropy
Characters

75
3
178

85
2.7
246

82
4
148

79
4
162

79
2.7
249

82
3.2
177

79
3.2
192

82
3.3
195

Table 3: Average characteristics of the generated synthetic cor-
pus. U and N correspond to the uniform and normal distribution
of the cluster sizes.

parts in the synthetic emails is performed randomly, multi-
ple clusters may share similar ﬁxed and variable parts, which
might result in over- or under-clustering. θ = 0.8 showed
the closest cluster distribution to the expected results. The
results are shown on Figure 2 using our two selected mea-
sures. The higher the clustering threshold is set, the more
template coverage converges towards a steady value for both
methods. Similar behavior is shown for the template en-
tropy; as cluster quality increases, templates are built over
more homogeneous sets of emails and therefore have a more
compact structure.

We can see the consistent improvement over the baseline
approach both in terms of email coverage and template en-
tropy. As shown on the synthetic corpus results Table 3,
the expected coverage and entropy are 79% and 3.2 respec-
tively for the ﬁrst batch of generated emails. We can see
that by varying both θ and γ, the suﬃx array based ap-
proach maintains dominance across all metrics. This consis-
tently improved performance stems from the fact that the
suﬃx array provides a higher quality set of candidate ﬁxed
phrases to use in template construction. Overall, having
more phrases is beneﬁcial when it comes to user proﬁling
and better template construction even if the higher number
of phrases requires an increase in extraction time.

4.2 Enron Corpus

For the second series of experiments we used the publicly
released email corpus from the Enron Corporation. The
corpus contains a large database of over 600,000 emails gen-
erated by over 150 users, mostly from senior management
of Enron. For the experiment we extracted all of the sent
emails of the corpus users. This resulted in over 125,000
emails with more than 300 distinct email addresses7.

We preprocessed the corpus as described in Section 3.
Multiple statistics are collected during clustering, such as
user outbox (sent mail) counts, cluster quality, and so on.
We do this in order to provide a sense as to whether the
clusters formed would be suitable for template induction.
By exposing an explicit notion of the quality of the clusters,
we avoid the possibility of an unknown feature acting as a
confounding factor when evaluating the induced templates.
To measure quality of the clusters themselves, we use a
variant of the “edit distance” (ED) measure. For an output
cluster C

Cout, we calculate the ED of the cluster as:

∈

ED(C) =

1
chars(C)

(cid:88)

D∈C

CharED(Rep(C), D)

(2)

where chars(C) is the sum of the character lengths of all
member emails in C. We rely on this metric to emphasize
the compression of the outbox and thus typing reduction of
the repetitive parts. When a cluster has a body edit distance
of less than 20% of its average content length and contains
at least 5 emails, we call that cluster a “high-quality” (HQ)
cluster. Based on this analysis and deﬁnition we obtain the
following corpus statistics shown in Table 4.

We break down the user sent mail volume into deciles to
get a sense of how many users could be characterized as
“high-volume” senders, as shown in Table 4. Only active
users that fall into the 40th percentile and higher by their

7We treat multiple corporate accounts of a user as separate
entities since each account is used for a distinct purpose.

0.00.20.40.60.81.0Coverageθ=0.6θ=0.7BaseUniformSAUniformBaseNormalSANormalθ=0.8θ=0.90.50.70.905101520253035Entropy0.50.70.90.50.70.90.50.70.9γUser deciles Number of

0
20
30
40
50
60
70
80
90
Aggregates

users

79
19
28
31
32
32
31
33
31
316

Total
outbox size

Average
outbox size

Average email
length

Average cluster size
for θ = 0.8

High quality clusters
for θ = 0.8

79
50
310
1,372
2,885
5,886
10,809
23,377
80,336
125104

1
2.63
11.07
44.26
90.16
183.94
348.68
708.39
2,591.48
442

284.81
372.21
1,352.31
589.07
641.81
483.96
618.29
409.21
570.87
591

1
1.97
3.22
5.15
5.63
4.8
6.16
4.56
7.84
4.48

Table 4: Description of the Enron sent mail corpus.

0
0
0
2
2
7
11
53
102
177

∼

sent mail volume are capable of producing templates that
are of suitable quality, and as the decile increases, the num-
ber of HQ clusters grow superlinearly. The data in the table
suggests that a user would need at least
40 emails to pro-
duce any useful templates. Given the increasing prevalence
of email for communication, this suggests that templatiza-
tion could be useful for virtually every current user of email.
The ﬁrst two deciles did not have more than one email
sent which is shown in the 4th column. Interestingly, the
average size of a sent email is signiﬁcantly greater in the
third decile compared to others. This observation is driven
by the data, i.e., users with a relatively low outbox size (
11
emails on average) tend to send mainly long annual reports.
Moreover, the average size of the user outbox correlates with
the tendency to write similar emails.

∼

We also investigated whether the average edit distance in
a cluster behaved as a function of the cluster size, as shown
in Figure 3.
Indeed, the greater the size of the produced
cluster, the lower the chance to observe a small edit distance
within the cluster. The two exceptions to this observation
occur at cluster sizes 10 and 100, which consist of annual
reports (within a cluster) that only vary in the month men-
tioned in the email.

Figure 4: Correlation between average body edit distance and
average subject edit distance within cluster and fraction of dis-
tinct receivers (1 - all receivers are distinct) respectively.

positive correlation of 0.91 between θ and the number of
clusters produced, while the synthetic data has a moderate
positive correlation of 0.62. More proliﬁc users (top deciles)
tend to write more similar emails as described in Table 4.
We tested the variations of the SA approach when limiting
the size of the accepted ﬁxed phrase (2, 3 words).

Figure 3: The average ED as cluster size increases for θ = 0.8

Using the edit distance as deﬁned, we ﬁnd that the edit
distance for the bodies and subjects of the emails in a given
cluster have a Pearson correlation coeﬃcient of 0.31. As
the edit distance increases for the subjects, the body edit
distance tends to increase as well. The trends for subject vs.
body are presented in Figure 4. Such information could be
used in email clustering and cluster ﬁltering, or for eﬃciency
gains when performing clustering at large scale.

Similarly to the synthetic corpus experiments we performed
template induction for the baseline and SA based approaches.
As a result of clustering with θ = 0.8 we obtained over 25,000
clusters. As expected, the higher the cluster threshold, the
more clusters are produced. In particular, we observe strong

Figure 5: Average template coverage and entropy for γ = 0.8
and θ = 0.8 over Enron corpus all and high quality clusters.

As can be seen from Figure 5, the suﬃx array based ap-
proach performs better than the baseline alternative in terms
of coverage and entropy. We show only one pair of values for
θ and γ here, but we observed similar behaviour for other
values of these parameters. By varying the constraints on
the phrase quality, we show that it is possible to balance
between the coverage and the entropy of the template. For

17th(2emails)23th(3emails)33th(4emails)35th(5emails)39th(6emails)41th(8emails)42th(10emails)43th(12emails)44th(15emails)46th(26emails)49th(153emails)over917emailsPercentilesofclustersizes10−410−310−210−1100Averageeditdistance10−210−1100101102Subjecteditdistance148121620Averagebodyeditdistancepercentiles10−1100Fractionofdistinctreceivers0.00.10.20.30.40.50.60.70.8CoverageAllclustersHQclusters02468101214EntropyBaseSASA(keeponlyphraseswithaminof2words)SA(keeponlyphraseswithaminof3words)example, the most restrictive results (SA with phrases with
a min of 3 words) have the least template coverage. How-
ever, this signiﬁcantly reduces the number of ﬁxed regions in
the template. Overall, average entropy for various setups of
our approach is
4, while maintaining the coverage within
60%. Considering an average email length of 600 characters
and average word size to be
35 word
reduction in typing in an autocompletion setting for users
with induced templates.

10, we obtain a

∼

∼

∼

Our ﬁndings indicate that using SA for template induction
oﬀers better performance than the baseline both in terms of
email coverage and template entropy. As can be seen in
3 for
Figure 2, where expected performance is
coverage and entropy respectively, the SA based ﬁxed phrase
extraction shows better results for both metrics no matter
the quality of the cluster. Similar behavior is observed for
the Enron corpus and shown in Figure 5.

80% and

∼

∼

4.3 Scalability Analysis

To test the performance characteristics of both approaches
we performed ﬁxed phrase extraction over various cluster
sizes. Even though this work focuses on the template extrac-
tion for a single user account the size of the outbox should
not be neglected, since it could reach millions of emails. We
kept each email size to be almost identical in size (approx. 1
KB each8). We varied the cluster size from 2 KB to 33 MB
with the corresponding number of emails from 2 to 33,000.
Figure 6 shows the execution time taken to create templates
as the size of the input cluster increases. When the clus-
ters are relatively small, the methods are equivalent in ef-
ﬁciency. However, the growth trends depicted in Figure 6
clearly show that the baseline approach takes longer to com-
plete than the SA approach as the cluster size scales up. The
baseline approach proves to be sensitive to both the number
of emails in the cluster and email size variations within the
cluster. The SA is agnostic to these variations due to the
fact that the input is treated as a blob of information for
which the SA is built and valid phrases are added to the
result.

Additionally, one can easily see that the growth of the
baseline is also superlinear - the baseline requires less than
200 seconds for 5K emails and 400 seconds for 15K emails,
but requires over 1600 seconds for 30K emails. While the
earlier segment has a slope of approximately 2/3 (2x time for
3x input), the next segment is closer to a slope of 2 (4x time
for 2x input). This suggests that the slope will continue to
grow as the input size increases. The SA approach shows a
slight slope increase as well, but it is multiplicalely less than
the baseline, making the SA approach more scalable.

5. CONCLUSIONS AND FUTURE WORK

We have demonstrated the feasibility of performing high-
quality plain text template induction using proposed highly
scalable solution. The experiments, perfomed on both a
synthethic and organic email corpora, illustrate the eﬃcacy
of using suﬃx arrays to induce templates, even in the face
of input clusters of varying quality.

We continued our investigation by then comparing two
template induction algorithms. We have shown both in the-
ory and in practice that using a suﬃx array is more eﬀective

81 KB is a upper bound on the 95% of the emails send in
our corpus.

Figure 6: A comparison of the increase in extraction size as the
average cluster size increases.

than an out-of-the-box shingling baseline for template in-
duction. The results of our investigation show that plain
text documents can be templatized more eﬃciently using
suﬃx arrays: the baseline showed superlinear growth, while
the suﬃx array’s growth is multiplicatively slower. Addi-
tionally, the templates induced using the suﬃx array encode
more useful information than the greedy approach: across
our experiments the suﬃx array templates provided con-
sistently better coverage than the greedily-built templates.
Our ancillary experiments suggested that if used for email
autocompletion, the generated templates could on average
save 35 words of typing when composing emails. Overall
the presented work is salient for numerous applications, in-
cluding optimizing the production of content, extracting in-
formation from machine-generated content (imagine if the
“user” sending the email is an algorithm written by an on-
line seller), and proﬁling composition behaviors of users. We
only considered forming templates for individual users or
bulk senders, however we would like to further explore 1)
accross user clustering to induce templates; 2) applications
of the created templates. This could allow an even higher
email compression and carry insights into the composition
behaviors of users at an aggregate level.

Our initial implementation relies on a simple selection the
representative document of a cluster, but we would like to
further explore alternative methods to ﬁnd a “near-best”
representation of a given cluster. Although we have shown
that suﬃx array templates are more robust to cluster quality
than greedily built templates, the clustering method aﬀects
the number of clusters produced, potentially creating many
more clusters than there should be.

Finally, although we discussed and analyzed the eﬃciency
of using the suﬃx array for template induction, our collec-
tion sizes are not real-world scale, and did not fully push
the limits of our implementation. To be truly web-scale,
our approach would need to work on billions of input docu-
ments, which will most likely present several eﬃciency chal-
lenges worth investigating. Both the clustering and induc-
tion phases could be improved by developing parallelized
versions of both algorithms.

6. REFERENCES
[1] D. Aberdeen, O. Pacovsky, and A. Slater. The learning
behind gmail priority inbox. In NIPS Workshop on
Learning on Cores, Clusters and Clouds, 2010.

050001000015000200002500030000ClustersizeinKBytes02004006008001000120014001600ExtractiontimeinsecondsSufﬁxarraybasedBaseline[2] N. Ailon, Z. S. Karnin, E. Liberty, and Y. Maarek.
Threading machine generated email. In Proc. of the
6th ACM International Conference on Web Search
and Data Mining, pages 405–414, 2013.

[3] J. Alpert and N. Hajaj. We knew the web was big.

The Oﬃcial Google Blog, 21, July 25 2008.

[4] I. Androutsopoulos, J. Koutsias, K. V. Chandrinos,

and C. D. Spyropoulos. An experimental comparison
of naive bayesian and keyword-based anti-spam
ﬁltering with personal e-mail messages. In Proc. of the
23rd Annual International ACM SIGIR Conference on
Research and Development in Information Retrieval,
pages 160–167, 2000.

[5] A. Arasu and H. Garcia-Molina. Extracting structured
data from web pages. In Proc. of the ACM SIGMOD
International Conference on Management of Data,
pages 337–348, 2003.

[6] R. Bekkerman. Automatic categorization of email into
folders: Benchmark experiments on Enron and SRI
corpora. Computer Science Department Faculty
Publication Series, University of Massachusetts,
Amherst, (218), 2004.

[7] E. Blanzieri and A. Bryl. A survey of learning-based

techniques of email spam ﬁltering. Artiﬁcial
Intelligence Review, 29(1):63–92, 2008.

[8] G. Caruana and M. Li. A survey of emerging

approaches to spam ﬁltering. ACM Computing
Surveys, 44(2):1–27, 2012.

[9] L. A. Dabbish and R. E. Kraut. Email overload at
work: An analysis of factors associated with email
strain. In Proc. of the 20th Conference on Computer
Supported Cooperative Work, pages 431–440, 2006.

[10] D. Di Castro, L. Lewin-Eytan, Y. Maarek, R. Wolﬀ,

and E. Zohar. Enforcing k-anonymity in web mail
auditing. In Proc. of the 9th International Conference
on Web Search and Data Mining, to appear, 2016.
[11] C. Hachenberg and T. Gottron. Locality sensitive

hashing for scalable structural classiﬁcation and
clustering of web documents. In Proc. of the 22nd
ACM International Conference on Information &
Knowledge Management, pages 359–368, 2013.
[12] A. Kannan, K. Kurach, S. Ravi, T. Kaufmann,
A. Tomkins, B. Miklos, G. Corrado, L. Luk´acs,
M. Ganea, P. Young, and V. Ramavajjala. Smart
reply: Automated response suggestion for email.
CoRR, abs/1606.04870, 2016.

[13] S. Kiritchenko and S. Matwin. Email classiﬁcation
with co-training. In Proc. of the Conference of the
Center for Advanced Studies on Collaborative
Research, pages 301–312, 2011.

[14] A. Kulkarni and T. Pedersen. Name discrimination

and email clustering using unsupervised clustering and
labeling of similar contexts. In Proc. of the 2nd Indian

International Conference on Artiﬁcial Intelligence,
pages 703–722, 2005.

[15] N. Kushmerick. Wrapper induction for information

extraction. PhD thesis, University of Washington,
1997.

[16] A. H. Laender, B. A. Ribeiro-Neto, A. S. da Silva, and
J. S. Teixeira. A brief survey of web data extraction
tools. ACM Sigmod, 31(2):84–93, 2002.
[17] J. Leskovec, L. Backstrom, and J. Kleinberg.

Meme-tracking and the dynamics of the news cycle. In
Proc. of the 15th ACM SIGKDD International
Conference on Knowledge Discovery and Data Mining,
KDD ’09, pages 497–506. ACM, 2009.

[18] D. D. Lewis and K. A. Knowles. Threading electronic
mail: A preliminary study. Information Processing &
Management, 33(2):209–217, 1997.

[19] H. Li, D. Shen, B. Zhang, Z. Chen, and Q. Yang.

Adding semantics to email clustering. In Proc. of the
6th International Conference on Data Mining, pages
938–942, 2006.

[20] G. A. Miller. WordNet: A lexical database for English.
Communications of the ACM, 38(11):39–41, 1995.
[21] P. Pantel and D. Lin. Spamcop: A spam classiﬁcation

& organization program. In Proc. of the AAAI
Workshop on Learning for Text Categorization, pages
95–98, 1998.

[22] S. Sarawagi. Automation in information extraction
and integration. In Tutorial of the 28th Internationl
Conference on Very Large Databases, 2002.

[23] Y.-C. Wang, M. Joshi, W. W. Cohen, and C. P. Ros´e.
Recovering implicit thread structure in newsgroup
style conversations. In Proc. of the 2nd International
Conference on Weblogs and Social Media, pages
152–160, 2008.

[24] P. Weiner. Linear pattern matching algorithms. In

Proc. of the 14th Annual Symposium on Switching and
Automata Theory, pages 1–11, 1973.

[25] J. B. Wendt, M. Bendersky, L. Garcia-Pueyo,

V. Josifovski, B. Miklos, I. Krka, A. Saikia, J. Yang,
M.-A. Cartright, and S. Ravi. Hierarchical label
propagation and discovery for machine generated
email. In Proc. of the 9th International Conference on
Web Search and Data Mining, 2016.

[26] L. Zhang, J. Zhu, and T. Yao. An evaluation of
statistical spam ﬁltering techniques. ACM
Transactions on Asian Language Information
Processing, 3(4):243–269, 2004.

[27] W. Zhang, A. Ahmed, J. Yang, V. Josifovski, and

A. J. Smola. Annotating needles in the haystack
without looking: Product information extraction from
emails. In Proc. of the 21th ACM SIGKDD
International Conference on Knowledge Discovery and
Data Mining, pages 2257–2266, 2015.
