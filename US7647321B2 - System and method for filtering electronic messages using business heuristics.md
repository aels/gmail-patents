Source: https://patents.google.com/patent/US7647321B2/en

---

# US7647321B2 - System and method for filtering electronic messages using business heuristics - Google Patents

System and method for filtering electronic messages using business heuristics

[Download PDF](https://patentimages.storage.googleapis.com/73/0e/23/5529c4d0a446e3/US7647321.pdf)

## Info

Publication number
:   US7647321B2

US7647321B2
US10/832,407
US83240704A
US7647321B2
US 7647321 B2
US7647321 B2
US 7647321B2

US 83240704 A
US83240704 A
US 83240704A
US 7647321 B2
US7647321 B2
US 7647321B2

Authority
:   US
:   United States

Prior art keywords
:   electronic message
:   business
:   intended recipient
:   threshold
:   message

Prior art date
:   2004-04-26

Legal status (The legal status is an assumption and is not a legal conclusion. Google has not performed a legal analysis and makes no representation as to the accuracy of the status listed.)
:   Expired - Lifetime, expires 2026-08-22

Application number
:   US10/832,407

Other versions
:   [US20050240617A1
    (en](/patent/US20050240617A1/en)

Inventor
:   Peter K. Lund
:   Scott M. Petry
:   Jason H. Titus

Current Assignee (The listed assignees may be inaccurate. Google has not performed a legal analysis and makes no representation or warranty as to the accuracy of the list.)
:   Google LLC

Original Assignee
:   Google LLC

Priority date (The priority date is an assumption and is not a legal conclusion. Google has not performed a legal analysis and makes no representation as to the accuracy of the date listed.)
:   2004-04-26

Filing date
:   2004-04-26

Publication date
:   2010-01-12
:   2004-04-26
    Application filed by Google LLC
    filed
    Critical
    Google LLC
:   2004-04-26
    Assigned to POSTINI INC.
    reassignment
    POSTINI INC.
    ASSIGNMENT OF ASSIGNORS INTEREST (SEE DOCUMENT FOR DETAILS).
    Assignors: LUND, PETER K., PETRY, SCOTT M., TITUS, JASON H.
:   2004-04-26
    Priority to US10/832,407
    priority
    Critical
    patent/US7647321B2/en
:   2005-03-29
    Priority to KR1020067024774A
    priority
    patent/KR101208943B1/en
:   2005-03-29
    Priority to JP2007510738A
    priority
    patent/JP4960222B2/en
:   2005-03-29
    Priority to CNA200580013218XA
    priority
    patent/CN1977263A/en
:   2005-03-29
    Priority to CA2564232A
    priority
    patent/CA2564232C/en
:   2005-03-29
    Priority to AU2005241402A
    priority
    patent/AU2005241402B2/en
:   2005-03-29
    Priority to PCT/US2005/010276
    priority
    patent/WO2005109234A2/en
:   2005-03-29
    Priority to EP05733019A
    priority
    patent/EP1763789A4/en
:   2005-10-27
    Publication of US20050240617A1
    publication
    Critical
    patent/US20050240617A1/en
:   2009-04-30
    Assigned to GOOGLE INC.
    reassignment
    GOOGLE INC.
    ASSIGNMENT OF ASSIGNORS INTEREST (SEE DOCUMENT FOR DETAILS).
    Assignors: POSTINI, INC.
:   2009-12-09
    Priority to US12/634,436
    priority
    patent/US8321432B2/en
:   2010-01-12
    Publication of US7647321B2
    publication
    Critical
    patent/US7647321B2/en
:   2010-01-12
    Application granted
    granted
    Critical
:   2017-10-02
    Assigned to GOOGLE LLC
    reassignment
    GOOGLE LLC
    CHANGE OF NAME
    Assignors: GOOGLE INC.
:   2026-08-22
    Adjusted expiration
    legal-status
    Critical
:   Status
    Expired - Lifetime
    legal-status
    Critical
    Current

## Links

* [USPTO](https://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO1&Sect2=HITOFF&p=1&u=/netahtml/PTO/srchnum.html&r=1&f=G&l=50&d=PALL&s1=7647321.PN.)
* [USPTO PatentCenter](https://patentcenter.uspto.gov/applications/10832407)
* [USPTO Assignment](https://assignment.uspto.gov/patent/index.html#/patent/search/resultFilter?searchInput=7647321)
* [Espacenet](https://worldwide.espacenet.com/publicationDetails/biblio?CC=US&NR=7647321B2&KC=B2&FT=D)
* [Global Dossier](https://globaldossier.uspto.gov/result/application/US/10832407/1)
* [Discuss](https://patents.stackexchange.com/questions/tagged/US7647321)

## Images

* ![](https://patentimages.storage.googleapis.com/ee/70/94/45dde5b27362bf/US07647321-20100112-D00000.png)
* ![](https://patentimages.storage.googleapis.com/cd/35/f6/df8e8a28f15621/US07647321-20100112-D00001.png)
* ![](https://patentimages.storage.googleapis.com/2d/fa/3c/136f108d9fea53/US07647321-20100112-D00002.png)
* ![](https://patentimages.storage.googleapis.com/f1/ea/14/d68b9abc7afc84/US07647321-20100112-D00003.png)
* ![](https://patentimages.storage.googleapis.com/99/e4/ff/2a098c191cf325/US07647321-20100112-D00004.png)

## Classifications

* + G—PHYSICS
  + G06—COMPUTING OR CALCULATING; COUNTING
  + G06Q—INFORMATION AND COMMUNICATION TECHNOLOGY [ICT] SPECIALLY ADAPTED FOR ADMINISTRATIVE, COMMERCIAL, FINANCIAL, MANAGERIAL OR SUPERVISORY PURPOSES; SYSTEMS OR METHODS SPECIALLY ADAPTED FOR ADMINISTRATIVE, COMMERCIAL, FINANCIAL, MANAGERIAL OR SUPERVISORY PURPOSES, NOT OTHERWISE PROVIDED FOR
  + G06Q50/00—Information and communication technology [ICT] specially adapted for implementation of business processes of specific business sectors, e.g. utilities or tourism
  + G06Q50/60—Business processes related to postal services
* + G—PHYSICS
  + G06—COMPUTING OR CALCULATING; COUNTING
  + G06Q—INFORMATION AND COMMUNICATION TECHNOLOGY [ICT] SPECIALLY ADAPTED FOR ADMINISTRATIVE, COMMERCIAL, FINANCIAL, MANAGERIAL OR SUPERVISORY PURPOSES; SYSTEMS OR METHODS SPECIALLY ADAPTED FOR ADMINISTRATIVE, COMMERCIAL, FINANCIAL, MANAGERIAL OR SUPERVISORY PURPOSES, NOT OTHERWISE PROVIDED FOR
  + G06Q10/00—Administration; Management
  + G06Q10/10—Office automation; Time management
  + G06Q10/107—Computer-aided management of electronic mailing [e-mailing]
* + G—PHYSICS
  + G06—COMPUTING OR CALCULATING; COUNTING
  + G06Q—INFORMATION AND COMMUNICATION TECHNOLOGY [ICT] SPECIALLY ADAPTED FOR ADMINISTRATIVE, COMMERCIAL, FINANCIAL, MANAGERIAL OR SUPERVISORY PURPOSES; SYSTEMS OR METHODS SPECIALLY ADAPTED FOR ADMINISTRATIVE, COMMERCIAL, FINANCIAL, MANAGERIAL OR SUPERVISORY PURPOSES, NOT OTHERWISE PROVIDED FOR
  + G06Q50/00—Information and communication technology [ICT] specially adapted for implementation of business processes of specific business sectors, e.g. utilities or tourism
  + G06Q50/10—Services
* + H—ELECTRICITY
  + H04—ELECTRIC COMMUNICATION TECHNIQUE
  + H04L—TRANSMISSION OF DIGITAL INFORMATION, e.g. TELEGRAPHIC COMMUNICATION
  + H04L51/00—User-to-user messaging in packet-switching networks, transmitted according to store-and-forward or real-time protocols, e.g. e-mail
  + H04L51/21—Monitoring or handling of messages
  + H04L51/212—Monitoring or handling of messages using filtering or selective blocking

## Definitions

* Disclosed embodiments herein
  relate generally to the filtering of electronic messages (e-mail), and more particularly to systems and method for filtering electronic messages using business heuristics.
* E-mail management
  is commonly handled by ISPs that have user/subscribers, or by company servers located at facilities where the e-mail users are employed.
* a part of e-mail management
  comprises filtering for spam or virus control, but when such e-mail management is performed at the ISP or at the company server location, valuable communication bandwidth and computing resources are expended on routing, analyzing, and other handling of spurious e-mail traffic.
* Present e-mail management systems
  are further characterized by a lack of real-time monitoring, feedback, and updating of rules regarding e-mail traffic or SMTP connection situations. Thus, management and monitoring of e-mail traffic situations is commonly handled through human intervention.
* the method
  further includes assigning a spam-score to the electronic message based on a likelihood that the electronic message is not unwanted by the intended recipient, blocking delivery of the electronic message to the intended recipient when the spam-score does not cross an overall threshold, and delivering the electronic message to the intended recipient based on the adjusted likelihood when the electronic message is determined to be associated with the desirable business.
* a related system for filtering an electronic message using business heuristics
  includes a message handler configured to receive the electronic message, and a heuristics module associated with the message handler and configured to determine whether the electronic message is associated with a desirable business.
* the message handler
  is further configured to adjust the likelihood that the electronic message will be delivered to the intended recipient if the electronic message is determined to be associated with the desirable business.
* such a system
  also includes a software module associated with the message handler and configured to assign a spam-score to the electronic message based on a likelihood that the electronic message is not unwanted by an intended recipient of the electronic message, where the message handler is further configured to block delivery of the electronic message to the intended recipient when the spam-score does not cross an overall threshold.
* FIG. 1
  illustrates one embodiment of a prior art system for the delivery of e-mail messages through the Internet or other computer network
* FIG. 2
  illustrates a block diagram of an embodiment in which an active Electronic Message Management System is provided between the Internet and receiving mail server;
* FIG. 3
  illustrates a more detailed diagram including a block diagram of the EMS shown in FIG. 2 ;
* FIG. 4
  illustrates one embodiment of a screen shot for setting multiple thresholds for filtering unwanted e-mail messages
* FIG. 5
  illustrates a more detailed view of the block diagram of the EMS discussed with reference to FIG. 3 ;
* FIG. 6
  illustrates one embodiment of a screen shot for setting business-specific thresholds, in addition to the base thresholds described above, in accordance with the disclosed principles
* FIG. 7
  illustrates a flow diagram of an exemplary process for the disclosed business heuristics-based filtering technique.
* Sending mail servers 102 a, 102 b
  (having associated source Internet protocol (IP) addresses) and receiving mail servers 102 c, 102 d (having associated destination IP addresses), or other message gateways, allow electronic messages, such as electronic mails (or “e-mails”) to be delivered to and from sending client machines 104 a - 104 d to receiving client machines 104 e - 104 h, or other devices such as cell phones, pagers, and/or hand-held computers.
* IP
  Internet protocol
* e-mails
  electronic mails
* the transmission direction of the e-mails
  may also be reversed, where the sending machines and servers become the receiving machines and servers and vice versa.
* E-mail messages
  are typically composed by an application running on a client machine 104 .
* the user
  uploads the completed message to a mail server 102 .
* the mail server 102
  in one embodiment is owned by an Internet Service Provider (ISP) or by a private corporation for whom the user works.
* ISP
  Internet Service Provider
* the user client machine 104
  connects to the mail server 102 via dial-up, digital subscriber loop (DSL), cable Internet, or by other appropriate means.
* DSL
  digital subscriber loop
* RFC 822 obsoleted by RFC2822
  which are a standard and a proposed standard, respectively, promulgated by Internet Engineering Task Force (“IETF”).
* RFC821
  obsoleted by RFC 2821, which are also a standard and a proposed standard, respectively, of the IETF. These standards can be found at ⁇ www.ietf.org>.
* the present disclosure
  hereby incorporates by reference the subject matter of the RFC 821 and RFC 822 standards and the RFC 2821 and RFC2822 proposed standards. If the proposed standards are updated from the versions published in April 2001, it is the subject matter of the April 2001 versions of these proposed standards that is hereby incorporated by reference.
* the RFC 821 and RFC 2821 documents
  describe a Simple Mail Transport Protocol (“SMTP”), which is the protocol by which e-mail messages have typically been transported over the Internet.
* SMTP
  Simple Mail Transport Protocol
* MTAs
  Mail Transfer Agents
* MUAs
  Mail User Agents
* UUAs
  Mail User Agents
* the SMTP mail transport protocol
  uses domain names to route messages from a sender to a receiver of e-mail.
* a distributed database of TCP/IP addresses corresponding to particular domain names
  is maintained across the Internet 101 in Domain Name Servers (“DNSs”) 108 .
* DNSs
  Domain Name Servers
* the source mail servers 102 a, 102 b
  would generally take the address specified by the sending user and inquire of a DNS server 108 the IP address to be assigned to the particular addressed domain name.
* an “address”
  is a character string that identifies a user to whom mail will be sent, a user or source that is sending mail, or a location into which mail will be deposited.
* emailbox
  refers to that depository.
* the two terms
  are typically used interchangeably unless the distinction between the location in which mail is placed (the mailbox) and a reference to it (the address) is important.
* An address
  normally consists of user and domain specifications; however, addresses may have different forms depending on usage and type of address.
* the standard mailbox naming convention
  is defined to be “local-part@domain”; contemporary usage permits a much broader set of applications than simple “user names”.
* the local part of the address
  is typically interpreted and assigned semantics only by the host specified in the domain part of the address.
* the standard IP address
  is typically a specific string of numbers identifying a source or destination server.
* a DNS lookup
  is performed to resolve the domain name.
* the email 110
  is then sent from the source mail server 102 a, 102 b via the Internet 101 to the identified domain.
* FIG. 2
  illustrated is a block diagram 200 of an embodiment in which an active Electronic Message (e.g., E-Mail) Management System (EMS) 203 is provided between Internet 101 and receiving mail server 202 .
* the EMS 203 of the present invention
  is “active” and automated since it is constantly managing attempted transmissions of electronic messages without the need for human intervention at various steps of the management process. In this sense, an EMS 203 according to the principles disclosed herein is automated, and configured to manage message delivery in real-time.
* the EMS 203
  is able to interpret conditions, analyze patterns, and manage the delivery of data to the receiving server 202 by performing processing steps as each of the SMTP connection between the sender and recipient are processed.
* Traditional e-mail servers
  will typically accept the message data and write the message to disk prior to performing analysis.
* the EMS 203
  is able to perform management steps at each stage of the SMTP transaction in order to minimize impact on the destination server 202 , while providing security and management. So that mail intended for the mail server 202 , and thus the receiving client's terminal 204 , is routed through the EMS 203 , the numerical IP address in the DNS 108 that is associated with the domain name of the targeted mail server 202 is updated to reflect the numerical address of the EMS 203 .
* the domain name of the mail server 202
  is ⁇ anywhere.com> and the numerical IP addresses for the mail server 202 and EMS 203 were “1234.5678.9876.5432” and “9876.5432.1234.5768,” respectively. Then the records in the distributed DNS database 108 for ⁇ anywhere.com> would be updated to reflect the EMS's numerical address “9876.5432.1234.5768,” rather than “1234.5678.9876.5432.”
* the EMS 203
  can be located anywhere on the Internet 101 . It can also be located either outside or within the mail server's 202 associated firewall 210 , as shown by the optional positioning of the 20 firewall 210 at position “A” (outside the firewall) or at position “B” (inside the firewall). Alternatively, the EMS 203 could possibly run on the same physical machine as the mail server 202 .
* FIG. 3
  illustrated is a more detailed diagram including a block diagram 300 of the EMS 203 shown in FIG. 2 .
* An administrative console
  (not illustrated) may be located on the same particular server machine as the actual EMS system 203 for providing an administrative access tool to assist in configuring how the EMS 203 processes incoming electronic messages.
* the connections between the EMS 203 and the mail servers 102 a, 102 c
  may be made through Internet or SMTP connections.
* the EMS 203
  could exist inside or outside a particular firewall with or without one of the mail servers 102 a, 102 c.
* the system shown in FIG. 3
  handles e-mail from a “sending” mail server 102 a.
* the designation of one mail server as a “sender” and the other as a “receiver”
  is arbitrary. Practically speaking, both mail servers 102 a, 102 c will generally act as both sender and receiver of electronic messages from and to the mail servers' 102 a, 102 c sending and receiving clients 104 a, 104 e.
* at least one of the mail servers' 102 a, 102 c domain names
  will be associated with the EMS 203 in the DNS distributed database and its servers 108 .
* the console
  receives information from the EMS 203 regarding the types of electronic messages which are coming in for particular users or groups of users, such as information regarding the suspected viruses and spam e-mails, directory harvest attacks, or unwanted content or delivery attempts that have been sent to the user or users.
* the EMS 203
  is shown in FIG. 3 as including several interconnected message handling software modules for processing electronic messages.
* message handling software modules
  for processing electronic messages.
* connection management module
  or simply a connection manager 322 .
* the connection manager 322
  is responsible for setting up and monitoring incoming SMTP connections from UAs/mail servers 102 a (or Mail Transfer Agents).
* the connection manager 322
  is the entry point to the EMS 203 , and it monitors the incoming SMTP connection attempts and e-mail messages. Specialized processes found, for example, in software daemons, interact with data collected from the incoming messages and/or connection attempts to recognize patterns of messages within the traffic of messages that can be acted upon. More specifically, the connection manager 322 , an e-mail handler 326 , plug-in applications 332 , and a delivery management module (or simply a delivery manager 324 ), are all employed to process incoming electronic messages.
* the e-mail handler 326
  takes an incoming e-mail message and can “scrape” or extract information from the message as it is going by, i.e., without imposing a delay on the delivery of the message.
* the e-mail handler 326
  is also able to conditionally deliver messages via the delivery manager 324 , either on its own accord or according to instructions.
* the e-mail handler 326
  is conceptually connected to a Multipurpose Internet Mail Extensions (MIME) decoder 328 and to an application interface 330 .
* the application interface 330
  provides an interface between the e-mail handler 326 and the plug-in applications 332 mentioned above.
* patterns in the data
  may be determined so that message processing information, typically in the form of disposition instructions, may be created. If one of the applications 332 , such as a spam detection application, returns a value for a message (i.e., a “spam score”) based on the likelihood that the message is not spam, the e-mail handler 326 can configure the delivery of the message to route it to a quarantine website.
* a spam detection application
  returns a value for a message (i.e., a “spam score”) based on the likelihood that the message is not spam.
* the decisions on which electronic messages are passed, diverted, deferred, etc.
  are made in part based on the metadata generated from the universe of incoming messages, and based on the way the EMS 203 has been configured and the applications 332 selected for processing the messages.
* the delivery manager 324
  may be instructed to dispose of the message appropriately.
* FIG. 4
  illustrated is one embodiment of a screen shot 400 for setting multiple thresholds for filtering unwanted e-mail message. More specifically, the screen shot 400 illustrates the opportunity to adjust the settings on an overall threshold for incoming e-mails: “Bulk E-mail”. In addition, the screen 400 allows for adjusting the settings in base thresholds based on specific categories: “Sexually Explicit”, “Get Rich Quick”, “Special Offers”, and “Racially Insensitive”. Once a user has made his desired selections and adjustments, the changes may be saved by clicking the “Save Changes” button on the screen. In addition, if the adjustments are not to be kept, the user may simply cancel the changes by clicking the illustrated “Cancel” button.
* the overall threshold
  “Bulk E-mail”, is employed for establishing an overall tolerance for filtering incoming e-mail messages.
* e-mail filtering processes
  typically assign a spam score to all incoming e-mails that indicates the likelihood that the e-mail is not spam (i.e., that the e-mail is not necessarily unwanted by the intended recipient).
* the process
  may alternatively be configured where the spam score is based on the likelihood that the e-mail is spam.
* the basis for assigning such spam scores
  differs for each specific filtering process based on the criteria each process is configured to examine.
* a spam score
  may be affected by a source IP address of the e-mail (e.g., a known “spammer”) or if it is determined to be part of a mass e-mailing attempt, such as a directory harvest attack.
* a source IP address of the e-mail
  e.g., a known “spammer”
* a mass e-mailing attempt
  such as a directory harvest attack.
* the level of tolerance for such filtering
  may be adjusted using on-screen selection within a range from “Lenient” to “Aggressive”. As may be expected, as this overall setting is increased towards the “Aggressive” side, more incoming e-mail messages are likely to be filtered out.
* each user of the filtering process
  may adjust his individual overall threshold.
* the remaining four base thresholds
  typically employ content-based filtering processes.
* Such content-based filtering processes
  may be embodied in the application modules 332 discussed with reference to FIG. 3 .
* users
  may individually adjust the tolerance in each of these four base thresholds depending on their personal tolerance for receiving unwanted e-mail that should have been filtered, or, alternatively, the improper filtering of e-mail that should have been allowed to pass through to the intended recipient's inbox.
* these base thresholds
  also provide the option of shutting off each particular filter threshold, as illustrated in the screen shot 400 .
* the EMS
  still includes the connection manager 322 , which is responsible for setting up and monitoring incoming SMTP connections from mail servers and monitoring incoming SMTP connection attempts and e-mail messages.
* the EMS
  still also includes the e-mail handler 326 , the MIME decoder, the delivery manager 324 , and the plug-in applications 332 , which communicate with the e-mail handler 326 via the application interface 330 .
* an incoming electronic message
  is first received by the connection manager 322 .
* the connection manager 322
  is typically configured to work in conjunction with the e-mail handler 326 to determine the source IP address of the sender of the message.
* a business heuristics-based (hereinafter, simply heuristics) module
  in the form of a business heuristics-based source IP address module 332 a assists in processing the message.
* the heuristics source IP module 332 a
  may be included in the EMS as one of several software application plug-ins.
* the heuristics source IP module 332 a
  is configured to access a source IP address database 334 in order to compare the previously determined source IP address of the incoming message to those stored in the database 334 .
* the heuristics source IP module 332 a
  may also be configured to compare the destination IP address of an outgoing message to those stored in the database 334 .
* the “source IP address”
  includes both the IP address of a sender of the message into the EMS system, as well as the IP address of a user of the EMS system who is sending the message.
* an overall message filtering threshold established by the user
  may be adjusted to increase the likelihood that the message will be delivered to the intended recipient, rather than being filtered out as unwanted spam. Such a threshold adjustment is discussed in greater detail below.
* another business heuristics module
  in the form of a heuristics-based content module 332 b, has also been added among the multiple applications 332 associated with the EMS.
* the heuristics content module 332 b
  may be comprised of software configured to analyze the content of incoming (or outgoing) electronic messages to determine the presence of content related to predetermined industries. For example, as a message is received by the EMS, the heuristics content module 332 b works with the e-mail handler 326 to search/extract content within the message based on instruction code provided by the heuristics content module 332 b.
* both the heuristics IP address module 332 a and the heuristics content module 332 b
  may be employed to determine if the message is somehow associated with a desirable business.
* being “associated with a business”
  means determining that any part of the message, including the source or destination IP address, the subject line, the message text, or any attachments, is in some way related to that business or to a job within that business.
* the source or destination IP address on the message
  belongs to a company or other organization known to be in or related to that business, or a part of the message may include content that is typically employed by companies or other organizations known to be in or related to that business, regardless if the sender or intended recipient is actually employed or volunteers in that line of business.
* the disclosed heuristics process
  may apply to messages between two persons that are not associated with a specific business or profession, but the message includes content (or an IP address) that is determined to be associated with a designated type or field of business.
* content
  or an IP address
* Another example of being “associated with an business”
  includes content found to be associated with professional associations of professions related to the business. For instance, a lawyer working at a financial company may still employ and benefit from legal-based heuristics filtering even though he is working at a financial company or other non-legal entity, and not strictly in the legal industry.
* the adjustment to the overall threshold
  may vary based on the amount of business-based content detected in the incoming message, as well as the threshold setting for the heuristics content module 332 b made by either the intended recipient, the administrator, or even both.
* the heuristics content module 332 b and the heuristics source IP module 332 a
  are not limited to the exact embodiments and connections illustrated in FIG. 5 .
* persons who are ordinarily skilled in the pertinent field of technology/art
  will understand variations that may be made to those components and/or their corresponding connections to other components, without departing from the scope of the principles of filtering based on heuristics disclosed herein. Adjustments made based on either module 332 a, 332 b are discussed in greater detail below.
* FIG. 6
  illustrated is one embodiment of a screen shot 600 for setting business-specific thresholds, in accordance with the disclosed heuristics principles. Specifically, adjustment of two business-based thresholds: “Legal” and “Financial,” are illustrated. Of course, any number and/or type of business thresholds may be provided and employed with the disclosed filtering process. Also as before, once any adjustments have been made, the changes may be saved by clicking the “Save Changes” button or on the screen, or cancelled by clicking the illustrated “Cancel” button.
* the business-based thresholds
  are provided to influence whether e-mail messages satisfy the settings of the prior base thresholds such that they are delivered to the intended recipient. More specifically, the business thresholds generally allow e-mail messages that would normally be filtered out to pass through to the intended recipient based on business heuristics. The objective of this heuristics approach to e-mail filtering is to eliminate the problem of false positives that can become an issue when using generalized spam-filtering technology. As such, the likelihood that e-mail messages will be filtered out based on the settings of the base thresholds may be reduced based on the settings of the business thresholds. Moreover, in preferred embodiments, the screen shot 600 allowing the business threshold adjustments is only available to administrators of the e-mail filtering service. In such embodiments, a user interface may be provided to intended recipients of the messages that simply allows the user to turn heuristics filtering of messages on or off. Of course, in other embodiments the intended recipients of the incoming messages are provided access to the threshold adjustment bars.
* TH eff
  TH base ⁇ TH ind (1)
* TH eff
  the resulting effective threshold calculated by multiplying TH base , which is the cumulative base threshold, and TH ind , which is the business threshold.
* the result
  is a base threshold TH base .
* the business threshold TH ind
  based on its setting(s), adjusts the base threshold TH base to make it more lenient in certain business-based situations, thus increasing the likelihood of allowing a message through to the intended recipient that would previously have been filtered out.
* the business threshold TH ind
  may be adjusted to an extreme setting, which would virtually be determinative of the passage of an incoming message that would otherwise have been blocked from reaching the intended recipient. Determining the effective threshold is discussed in greater detail below.
* FIG. 7
  With continued reference to the screen shot 400 of FIG. 4 and the screen shot 600 of FIG. 6 , illustrated is a flow diagram of an exemplary process for the disclosed business heuristics-based filtering technique.
* the exemplary process of FIG. 7
  will be described with reference to a specific example. It should be understood, however, that this description should not be interpreted as a limitation to the implementation of the principles described herein, including, but not limited to, the technique for assigning values and scores to the various thresholds.
* the process of FIG. 7
  begins at a Start block 710 , wherein the disclosed e-mail filtering process is initiated.
* an incoming electronic message
  i.e., an e-mail
* the filtering process
  e.g., typically embodied in software
* the filtering process
  may be at a geographically distinct location from the intended recipient of the e-mail, or it may be located within the recipient's on-site e-mail server.
* a spam score
  is assigned to the incoming e-mail message, as mentioned above.
* the spam score given to the e-mail
  is typically based on several different criteria, and is used to indicate a likelihood that the message is not spam.
* the source IP address and/or domain of the sender
  may be considered, as well as the domain of the destination IP addresses and the content of the subject line and/or body of the e-mail.
* characteristics associated with the message
  may also be considered, such as whether the message is part of a mass mailing, whether the message is part of a directory harvest attack, whether the sender of the message is linked with prior spam mailings, etc.
* the spam score
  ranges from 0 or 100, where 0 indicates a certainty that the e-mail is spam, while a score of 100 indicates a certainty that the e-mail is not spam.
* the spam score assigned to each message passing therethrough
  is typically not changed throughout the filtering process, and is instead simply compared to various thresholds to determine whether the spam score falls below the threshold and should therefore be filtered from delivery to the intended recipient.
* other embodiments
  may also adjust the spam score, either alone or with an adjustment of the threshold.
* membership in a particular category associated with the base thresholds
  is determined.
* the subject line and/or body (or any associated part) of the e-mail
  may be scanned to look for indicators that the e-mail falls under one of the content-driven base thresholds: sexually Explicit, Get Rich Quick, Special Offers, or Racially Insensitive.
* the assigned spam score
  is used to generally determine whether the e-mail will be filtered out, membership in one of the enumerated categories increases the likelihood that the e-mail will be so filtered.
* each of the variable settings for these four categories
  may represent a multiplier used to increase the chance that the spam score will not surpass a new (adjusted) threshold, and therefore the message be filtered out. For example, if the user has an original overall threshold of 40, and an incoming e-mail includes sexually explicit material but has only been assigned a spam score of 50, without detecting membership in an offending category the e-mail will be passed through to the user since its spam score exceeds the threshold value.
* the settings for the content-driven base thresholds
  which create multipliers as described above, indicate a user's tolerance for false positives in filtering e-mails when the e-mails are determined to fall into the content-based (i.e., offending) categories. More specifically, in the example set forth above, the user is essentially stating that he is willing to tolerate 10 times the number of false positives (with the exemplary multiplier of 10) if the content of the e-mail is determined to contain sexually explicit material.
* the e-mail
  may still be filtered out based on its membership in the offending category (i.e., having offending content), as influenced by a high level set by the user for each category.
* the source IP address of the message
  is associated with any of the particular industries at issue, typically by employing software plug-ins, as described above.
* a list of “approved senders”
  contains a list of specific source IP addresses of potential message senders so that messages from those senders are more likely to be delivered to the user's inbox based on their affiliation with an “approved” source IP address.
* a database
  may be maintained that includes substantially all of the known IP addresses for all law firms in the United States. Thus, this database may be searched to determine if the source IP address for the incoming message corresponds to an address in this database.
* the user's thresholds
  will be adjusted on this basis, in a manner similar to that discussed above with reference to block 740 . Similar embodiments are envisioned for source IP addresses found to be associated with the financial business, such as from a bank or even between a sender and recipient that are not associated with the financial business but the content of the message is still found to be associated with the financial business (e.g., through terminology or the like).
* the database of source IP addresses
  is typically generated and kept by the administrating organization that is administering message filtering as disclosed herein, where that list is typically kept hidden from the users and competitors alike.
* filtering systems and processes as disclosed herein
  are broad enough to encompass embodiments where the intended recipient of the message may edit or even entirely create the list.
* the thresholds for filtering while employing such a list
  may be variable at the adjustment of the administrator or the user. Of course, such thresholds may also be adjusted to levels where an incoming message is almost always delivered if the sender's IP address is found to be included on the database list.
* this adjustment to the user's overall threshold
  is typically made based on IP addresses, not on domain name as found in conventional filtering techniques.
* domain name-based approaches
  typically include a list of “approved senders”, and when the domain name for the message sender matches a domain in the list, the message is simply allowed to pass through to the intended recipient.
* such approaches
  are not effective against senders of unwanted messages that employ “spoofing” techniques to send messages. In such situations, the unwanted message would still include a domain name that has been “approved” for sending messages.
* the disclosed technique
  employs the source IP address (typically four multi-digit numbers separated by periods) of message senders to help determine whether the sent message should be filtered out.
* One embodiment of such an approach
  may include the matching of the source IP address with IP addresses of known valid senders stored in a database, but the disclosed technique is not so limited.
* more than a mere source IP address “look-up” in the database
  takes place.
* other factors
  may be taken into account, such as the comparison of the sending IP address with that of the intended recipient to determine if both are members of the same business. If it is so determined, than the likelihood that the message is spam is less, and so the recipient's overall threshold may be adjusted (e.g., lowered) to reflect this likelihood.
* various comparisons
  may be made with the source IP address using such business-based viewpoints to determine whether the user's overall threshold should be adjusted to increase the likelihood that the message will be allowed to pass through.
* other determinations
  may include viewing past message traffic or connection attempts by the sending IP address (with or without consideration of any destination IP addresses) to determine if there is a pattern in such traffic/attempts that is typically associated with senders of spam rather than valid message senders.
* Other examples
  include comparing prior message traffic between the source IP address and other intended recipients within the business, or where the source IP address is assigned as related to a particular business through an external verification processes.
* a system and process as disclosed herein
  may include any such approaches, while remaining within the scope of the present disclosure and any claims issuing therefrom.
* the threshold adjustment
  based on whether there is business content in the e-mail that corresponds to one of the pre-selected industries.
* Plug-in applications
  may also be used to analyze the content of the e-mail looking for key terms or phrases that are typically associated with the industries. For example, if several instances of “legalese” are detected in the content of the e-mail and it is determined that the e-mail is sufficiently associated with the legal business, the user's threshold may be adjusted for comparison with the message's assigned spam score to accomplish the disclosed filtering process.
* the multiplier associated with the specific threshold
  may be set low enough such that the message is delivered to the intended recipient, even if the message would have been filtered out based on its spam score (or for other reasons) had no business content been found.
* a database
  may be used to store key terms and phrases associated with the business to accomplish the business content determination, and the disclosed technique is not limited to industries in which the intended recipient works.
* a process conducted in accordance with the principles disclosed herein
  may include blocks 750 and 760 in any order, or may even be conducted simultaneously, without departing from the scope of this disclosure.
* block 780
  filtering of the e-mail is conducted based on a comparison of its assigned spam score to the current overall threshold value. If at block 740 it was determined that the content of the e-mail did not warrant membership in any of the offending categories, then the filtering is done using the original overall threshold. To this end, if the spam score does not exceed the original threshold, then delivery of the e-mail to the intended recipient is blocked. However, if membership in one of the offending categories was determined, then the filtering is based on a comparison between the assigned spam score and the adjusted overall thresholds.
* category membership
  may result in the overall threshold value being increased (depending on the setting established by the user or system administrator), so as to decrease the likelihood that the e-mail will be allowed to the reach the user.
* the spam score
  does not exceed the adjusted overall threshold value, then delivery of the e-mail to the intended recipient is blocked. Conversely, in either case, if the spam score should exceed either the original or adjusted overall thresholds, then the e-mail will be delivered to the user.
* the process
  instead moves to block 790 .
* the e-mail
  is filtered based on a comparison of its assigned spam score to the effective threshold value, as adjusted in accordance with blocks 750 and 760 .
* the effective threshold
  is determined as described above, where the overall threshold is typically decreased depending on the settings established by the user and/or the system administrator.
* the business threshold values
  include multipliers of the original overall threshold.
* the multipliers for the business threshold values
  may all be less than 1.
* multiplying the overall threshold value with such a fractional multiplier
  decreases that overall threshold value, which increases the chance that the message will be allowed through the filtering process and be delivered to the intended recipient.
* the disclosed approach
  allows the threshold to be adjusted based on the content of the e-mail (or perhaps the source IP address), if associated with, for example, the legal industry.
* the use of the business threshold multipliers
  allows a user to essentially state that less false positives will be tolerated if an association to the selected industries in the business thresholds is determine to exist.
* the overall threshold
  will typically be decreased in this embodiment by the multiplier corresponding to the setting established in the “Legal” business threshold.
* the amount of the multiplier
  (and thus the amount of adjustment to the overall threshold) may be established, in one embodiment, by the intended recipient by an adjustment in the settings for separate thresholds for each business.
* a similar result
  may be attained if the source IP address or domain is found to be associated with the legal industry. For example, assuming that the domain used by a prestigious law firm has been identified in the source (or destination) IP address contained in the e-mail. In this example, while the e-mail may contain racial slurs therein, the likelihood that a prestigious law firm (whose source domain has been identified in the e-mail and matched to a database of approved senders) is sending out (or being sent) racially insensitive e-mail as spam is very remote. Unfortunately, however, the classification of the e-mail as “Racially Insensitive” based on its content will greatly decrease the chance for the e-mail to pass through the filtering process.
* the overall threshold
  although adjusted due to category membership, may then be decreased based on determined business association to create a more lenient effective threshold, and thus increase the chance that this particular e-mail will reach the intended recipient.
* the process
  may simply be configured to definitively deliver the incoming message to the intended recipient if the source IP address of the message has been determined to be associated with one of the predetermined industries, although approval is based on association with a predetermined business, in accordance with the disclosed principles.

## Landscapes

* Engineering & Computer Science
  (AREA)
* Business, Economics & Management
  (AREA)
* Human Resources & Organizations
  (AREA)
* Strategic Management
  (AREA)
* Entrepreneurship & Innovation
  (AREA)
* Tourism & Hospitality
  (AREA)
* Marketing
  (AREA)
* Physics & Mathematics
  (AREA)
* Theoretical Computer Science
  (AREA)
* Economics
  (AREA)
* General Physics & Mathematics
  (AREA)
* General Business, Economics & Management
  (AREA)
* Operations Research
  (AREA)
* Computer Networks & Wireless Communication
  (AREA)
* Quality & Reliability
  (AREA)
* Data Mining & Analysis
  (AREA)
* Signal Processing
  (AREA)
* Computer Hardware Design
  (AREA)
* Health & Medical Sciences
  (AREA)
* General Health & Medical Sciences
  (AREA)
* Primary Health Care
  (AREA)
* Information Transfer Between Computers
  (AREA)
* Data Exchanges In Wide-Area Networks
  (AREA)

## Abstract

Disclosed are systems and methods for use in filtering electronic messages using business heuristics. In one aspect, a method includes determining whether the electronic message is associated with a desirable business, and adjusting the likelihood of delivering the electronic message to an intended recipient of the message if the electronic message is determined to be associated with the desirable business. In a more specific embodiment, the method further includes assigning a spam-score to the electronic message based on a likelihood that the electronic message is not unwanted by the intended recipient, blocking delivery of the electronic message to the intended recipient when the spam-score does not cross an overall threshold, and delivering the electronic message to the intended recipient based on the adjusted likelihood when the electronic message is determined to be associated with the desirable business.

## Description

CROSS-REFERENCE TO RELATED APPLICATION

This Application is related to co-pending patent application Ser. No. 10/370,118, filed Feb. 19, 2003, and entitled “E-Mail Management Services”, which is commonly assigned with the present disclosure and incorporated herein by reference in its entirety for all purposes.

TECHNICAL FIELD

Disclosed embodiments herein relate generally to the filtering of electronic messages (e-mail), and more particularly to systems and method for filtering electronic messages using business heuristics.

BACKGROUND

E-mail management is commonly handled by ISPs that have user/subscribers, or by company servers located at facilities where the e-mail users are employed. A part of e-mail management comprises filtering for spam or virus control, but when such e-mail management is performed at the ISP or at the company server location, valuable communication bandwidth and computing resources are expended on routing, analyzing, and other handling of spurious e-mail traffic. Present e-mail management systems are further characterized by a lack of real-time monitoring, feedback, and updating of rules regarding e-mail traffic or SMTP connection situations. Thus, management and monitoring of e-mail traffic situations is commonly handled through human intervention.

Even if these concerns are addressed in modern e-mail management systems, the techniques typically employed to filter out unwanted spam messages is relatively ineffective as a whole. Specifically, as conventional techniques developed, so too did techniques employed by the senders of spam messages to circumvent many of even the most aggressive approaches. Making matters worse, even in situations where filtering techniques are successful in preventing unwanted messages from reaching their intended recipients, many otherwise valid messages are also blocked from delivery. Among the problems plaguing conventional systems employed for blocking unwanted messages is the phenomenon “spoofing” e-mail addresses to trick filtering system into believing the message is being sent by a valid sender. As a result, even filtering systems that employ “approved senders” configured by users are still ineffective against such attacks. Moreover, as mentioned above, if conventional systems are upgraded with available tools to assist in preventing such attacks, the end result typically is that many valid messages are prevented from reaching the user, which results in losses in both time and costs.

BRIEF SUMMARY

Disclosed are systems and methods for use in filtering electronic messages using business heuristics. As used herein, the term “business” is not intended to be limited to a business organization or to any one capitalist endeavor, but rather includes any and all organizations and any and all endeavors including professional, industrial, service-oriented, charitable, self-serving, etc. In one aspect, a method includes determining whether the electronic message is associated with a desirable business, and adjusting the likelihood of delivering the electronic message to an intended recipient of the message if the electronic message is determined to be associated with the desirable business. In a more specific embodiment, the method further includes assigning a spam-score to the electronic message based on a likelihood that the electronic message is not unwanted by the intended recipient, blocking delivery of the electronic message to the intended recipient when the spam-score does not cross an overall threshold, and delivering the electronic message to the intended recipient based on the adjusted likelihood when the electronic message is determined to be associated with the desirable business.

In another aspect, a related system for filtering an electronic message using business heuristics is also disclosed. In one embodiment, the system includes a message handler configured to receive the electronic message, and a heuristics module associated with the message handler and configured to determine whether the electronic message is associated with a desirable business. In such an embodiment, the message handler is further configured to adjust the likelihood that the electronic message will be delivered to the intended recipient if the electronic message is determined to be associated with the desirable business. In a more specific embodiment, such a system also includes a software module associated with the message handler and configured to assign a spam-score to the electronic message based on a likelihood that the electronic message is not unwanted by an intended recipient of the electronic message, where the message handler is further configured to block delivery of the electronic message to the intended recipient when the spam-score does not cross an overall threshold.

BRIEF DESCRIPTION OF THE DRAWINGS

Reference is now made to the following detailed description of the preferred embodiments, taken in conjunction with the accompanying drawings. It is emphasized that various features may not be drawn to scale. In fact, the dimensions of various features may be arbitrarily increased or reduced for clarity of discussion. Reference is now made to the following descriptions taken in conjunction with the accompanying drawings, in which:

FIG. 1 illustrates one embodiment of a prior art system for the delivery of e-mail messages through the Internet or other computer network;

FIG. 2 illustrates a block diagram of an embodiment in which an active Electronic Message Management System is provided between the Internet and receiving mail server;

FIG. 3 illustrates a more detailed diagram including a block diagram of the EMS shown in FIG. 2;

FIG. 4 illustrates one embodiment of a screen shot for setting multiple thresholds for filtering unwanted e-mail messages;

FIG. 5 illustrates a more detailed view of the block diagram of the EMS discussed with reference to FIG. 3;

FIG. 6 illustrates one embodiment of a screen shot for setting business-specific thresholds, in addition to the base thresholds described above, in accordance with the disclosed principles;

FIG. 7 illustrates a flow diagram of an exemplary process for the disclosed business heuristics-based filtering technique.

DETAILED DESCRIPTION OF PREFERRED EMBODIMENTS

Referring initially to FIG. 1, illustrated is one embodiment of a prior art system **100** for the delivery of e-mail messages through the Internet **101** or other computer network. Sending  mail servers  **102** *a,*  **102** *b* (having associated source Internet protocol (IP) addresses) and receiving  mail servers  **102** *c,*  **102** *d* (having associated destination IP addresses), or other message gateways, allow electronic messages, such as electronic mails (or “e-mails”) to be delivered to and from sending client machines **104** *a*-**104** *d* to receiving client machines **104** *e*-**104** *h,* or other devices such as cell phones, pagers, and/or hand-held computers. In accordance with conventional systems, the transmission direction of the e-mails may also be reversed, where the sending machines and servers become the receiving machines and servers and vice versa.

E-mail messages are typically composed by an application running on a client machine **104**. When composition of the message is completed, the user uploads the completed message to a mail server **102**. The mail server **102** in one embodiment is owned by an Internet Service Provider (ISP) or by a private corporation for whom the user works. The user client machine **104** connects to the mail server **102** via dial-up, digital subscriber loop (DSL), cable Internet, or by other appropriate means. One standard for e-mail formats is described by RFC 822 obsoleted by RFC2822, which are a standard and a proposed standard, respectively, promulgated by Internet Engineering Task Force (“IETF”). The protocol by which e-mail messages are transmitted from sending mail server **102** to receiving mail server **102** are described by RFC821, obsoleted by RFC 2821, which are also a standard and a proposed standard, respectively, of the IETF. These standards can be found at <www.ietf.org>. The present disclosure hereby incorporates by reference the subject matter of the RFC 821 and RFC 822 standards and the RFC 2821 and RFC2822 proposed standards. If the proposed standards are updated from the versions published in April 2001, it is the subject matter of the April 2001 versions of these proposed standards that is hereby incorporated by reference. The RFC 821 and RFC 2821 documents describe a Simple Mail Transport Protocol (“SMTP”), which is the protocol by which e-mail messages have typically been transported over the Internet.

SMTP servers and SMTP clients (SMTP clients are network computers, not to be confused with the client machines **104**) provide a mail transport service, and therefore act as Mail Transfer Agents (“MTAs”). Mail User Agents (“MUAs” or “UAs”) are normally thought of as the sources and targets of mail. At the source, an MUA might be the  source mail server  **102** *a,*  **102** *b* that collects mail to be transmitted from a user and hands it off to an MTA within the network **101**. The final (“delivery”) MTA would be thought of as handing the mail off to an MUA, which might be the  destination mail server  **102** *c,*  **102** *d* that holds a user's mail in the user's inbox.

The SMTP mail transport protocol uses domain names to route messages from a sender to a receiver of e-mail. A distributed database of TCP/IP addresses corresponding to particular domain names is maintained across the Internet **101** in Domain Name Servers (“DNSs”) **108**. Thus, to route an e-mail to its destination, the  source mail servers  **102** *a,*  **102** *b* would generally take the address specified by the sending user and inquire of a DNS server **108** the IP address to be assigned to the particular addressed domain name. As used in this specification, an “address” is a character string that identifies a user to whom mail will be sent, a user or source that is sending mail, or a location into which mail will be deposited. The term “mailbox” refers to that depository. The two terms are typically used interchangeably unless the distinction between the location in which mail is placed (the mailbox) and a reference to it (the address) is important. An address normally consists of user and domain specifications; however, addresses may have different forms depending on usage and type of address. The standard mailbox naming convention is defined to be “local-part@domain”; contemporary usage permits a much broader set of applications than simple “user names”. The local part of the address is typically interpreted and assigned semantics only by the host specified in the domain part of the address. In contrast, the standard IP address is typically a specific string of numbers identifying a source or destination server.

Once the  source mail server  **102** *a,*  **102** *b* lexically identifies a domain to which email will be delivered for processing, a DNS lookup, through a DNS server **108**, is performed to resolve the domain name. The email **110** is then sent from the  source mail server  **102** *a,*  **102** *b* via the Internet **101** to the identified domain.

Turning now to FIG. 2, illustrated is a block diagram **200** of an embodiment in which an active Electronic Message (e.g., E-Mail) Management System (EMS) **203** is provided between Internet **101** and receiving mail server **202**. The EMS **203** of the present invention is “active” and automated since it is constantly managing attempted transmissions of electronic messages without the need for human intervention at various steps of the management process. In this sense, an EMS **203** according to the principles disclosed herein is automated, and configured to manage message delivery in real-time.

The EMS **203** is able to interpret conditions, analyze patterns, and manage the delivery of data to the receiving server **202** by performing processing steps as each of the SMTP connection between the sender and recipient are processed. Traditional e-mail servers will typically accept the message data and write the message to disk prior to performing analysis. The EMS **203** is able to perform management steps at each stage of the SMTP transaction in order to minimize impact on the destination server **202**, while providing security and management. So that mail intended for the mail server **202**, and thus the receiving client's terminal **204**, is routed through the EMS **203**, the numerical IP address in the DNS **108** that is associated with the domain name of the targeted mail server **202** is updated to reflect the numerical address of the EMS **203**. For example, suppose the domain name of the mail server **202** is <anywhere.com> and the numerical IP addresses for the mail server **202** and EMS **203** were “1234.5678.9876.5432” and “9876.5432.1234.5768,” respectively. Then the records in the distributed DNS database **108** for <anywhere.com> would be updated to reflect the EMS's numerical address “9876.5432.1234.5768,” rather than “1234.5678.9876.5432.”

Although this figure shows the EMS **203** as being physically adjacent to the mail server **202**, such placement is only for illustration purposes. The EMS **203** can be located anywhere on the Internet **101**. It can also be located either outside or within the mail server's **202** associated firewall **210**, as shown by the optional positioning of the 20 firewall **210** at position “A” (outside the firewall) or at position “B” (inside the firewall). Alternatively, the EMS **203** could possibly run on the same physical machine as the mail server **202**.

Looking now at FIG. 3, illustrated is a more detailed diagram including a block diagram **300** of the EMS **203** shown in FIG. 2. An administrative console (not illustrated) may be located on the same particular server machine as the actual EMS system **203** for providing an administrative access tool to assist in configuring how the EMS **203** processes incoming electronic messages. The connections between the EMS **203** and the  mail servers  **102** *a,*  **102** *c* may be made through Internet or SMTP connections. As previously mentioned, the EMS **203** could exist inside or outside a particular firewall with or without one of the  mail servers  **102** *a,*  **102** *c.*

Generally, the system shown in FIG. 3 handles e-mail from a “sending” mail server **102** *a.* The designation of one mail server as a “sender” and the other as a “receiver” is arbitrary. Practically speaking, both  mail servers  **102** *a,*  **102** *c* will generally act as both sender and receiver of electronic messages from and to the mail servers' **102** *a,*  **102** *c* sending and receiving  clients  **104** *a,*  **104** *e.* In the embodiment shown, at least one of the mail servers' **102** *a,*  **102** *c* domain names will be associated with the EMS **203** in the DNS distributed database and its servers **108**. In embodiments employing the administrative console, the console receives information from the EMS **203** regarding the types of electronic messages which are coming in for particular users or groups of users, such as information regarding the suspected viruses and spam e-mails, directory harvest attacks, or unwanted content or delivery attempts that have been sent to the user or users.

The EMS **203** is shown in FIG. 3 as including several interconnected message handling software modules for processing electronic messages. For a more detailed discussion, reference is made to co-pending patent application Ser. No. 10/370,118, filed Feb. 19, 2003, and entitled “E-Mail Management Services”, which is commonly assigned with the present disclosure and incorporated herein by reference in its entirety for all purposes. The layout of these various software modules is not indicative of any particular physical structure in the machine running these software modules. One module illustrated is a connection management module, or simply a connection manager **322**. The connection manager **322** is responsible for setting up and monitoring incoming SMTP connections from UAs/mail servers **102** *a* (or Mail Transfer Agents). The connection manager **322** is the entry point to the EMS **203**, and it monitors the incoming SMTP connection attempts and e-mail messages. Specialized processes found, for example, in software daemons, interact with data collected from the incoming messages and/or connection attempts to recognize patterns of messages within the traffic of messages that can be acted upon. More specifically, the connection manager **322**, an e-mail handler **326**, plug-in applications **332**, and a delivery management module (or simply a delivery manager **324**), are all employed to process incoming electronic messages.

The e-mail handler **326** takes an incoming e-mail message and can “scrape” or extract information from the message as it is going by, i.e., without imposing a delay on the delivery of the message. The e-mail handler **326** is also able to conditionally deliver messages via the delivery manager **324**, either on its own accord or according to instructions. The e-mail handler **326** is conceptually connected to a Multipurpose Internet Mail Extensions (MIME) decoder **328** and to an application interface **330**. The application interface **330** provides an interface between the e-mail handler **326** and the plug-in applications **332** mentioned above. Following a configuration established by rules stored, for example, in an associated database, patterns in the data may be determined so that message processing information, typically in the form of disposition instructions, may be created. If one of the applications **332**, such as a spam detection application, returns a value for a message (i.e., a “spam score”) based on the likelihood that the message is not spam, the e-mail handler **326** can configure the delivery of the message to route it to a quarantine website.

The decisions on which electronic messages are passed, diverted, deferred, etc. are made in part based on the metadata generated from the universe of incoming messages, and based on the way the EMS **203** has been configured and the applications **332** selected for processing the messages. Depending on the condition preventing transmission of the message to the intended recipient, even if a connection by the connection manager **322** is accepted, the delivery manager **324** may be instructed to dispose of the message appropriately.

Turning briefly now to FIG. 4, illustrated is one embodiment of a screen shot **400** for setting multiple thresholds for filtering unwanted e-mail message. More specifically, the screen shot **400** illustrates the opportunity to adjust the settings on an overall threshold for incoming e-mails: “Bulk E-mail”. In addition, the screen **400** allows for adjusting the settings in base thresholds based on specific categories: “Sexually Explicit”, “Get Rich Quick”, “Special Offers”, and “Racially Insensitive”. Once a user has made his desired selections and adjustments, the changes may be saved by clicking the “Save Changes” button on the screen. In addition, if the adjustments are not to be kept, the user may simply cancel the changes by clicking the illustrated “Cancel” button.

The overall threshold, “Bulk E-mail”, is employed for establishing an overall tolerance for filtering incoming e-mail messages. Specifically, e-mail filtering processes typically assign a spam score to all incoming e-mails that indicates the likelihood that the e-mail is not spam (i.e., that the e-mail is not necessarily unwanted by the intended recipient). Of course, the process may alternatively be configured where the spam score is based on the likelihood that the e-mail is spam. The basis for assigning such spam scores differs for each specific filtering process based on the criteria each process is configured to examine. For example, a spam score may be affected by a source IP address of the e-mail (e.g., a known “spammer”) or if it is determined to be part of a mass e-mailing attempt, such as a directory harvest attack. As a result, if the spam score assigned to an incoming e-mail does not exceed the preset overall tolerance setting, then the e-mail will be filtered and not reach the intended recipient. As illustrated, the level of tolerance for such filtering may be adjusted using on-screen selection within a range from “Lenient” to “Aggressive”. As may be expected, as this overall setting is increased towards the “Aggressive” side, more incoming e-mail messages are likely to be filtered out. However, as the number of filtered messages increases with the change in tolerance, so too does the chance for “false positives” in the screening process, where valid and desirable e-mail messages are improperly identified as spam and filtered. As a result, each user of the filtering process may adjust his individual overall threshold.

Also capable of being adjusted are the four base thresholds identified above. However, where the “Bulk E-mail” threshold is typically applied against incoming messages based on source or destination IP addresses, the remaining four base thresholds typically employ content-based filtering processes. Such content-based filtering processes may be embodied in the application modules **332** discussed with reference to FIG. 3. As before, users may individually adjust the tolerance in each of these four base thresholds depending on their personal tolerance for receiving unwanted e-mail that should have been filtered, or, alternatively, the improper filtering of e-mail that should have been allowed to pass through to the intended recipient's inbox. Furthermore, these base thresholds also provide the option of shutting off each particular filter threshold, as illustrated in the screen shot **400**.

Referring now to FIG. 5, illustrated is a more detailed view of the block diagram **300** of the EMS discussed with reference to FIG. 3. As before, the EMS still includes the connection manager **322**, which is responsible for setting up and monitoring incoming SMTP connections from mail servers and monitoring incoming SMTP connection attempts and e-mail messages. The EMS still also includes the e-mail handler **326**, the MIME decoder, the delivery manager **324**, and the plug-in applications **332**, which communicate with the e-mail handler **326** via the application interface **330**.

In the illustrated embodiment, an incoming electronic message is first received by the connection manager **322**. The connection manager **322** is typically configured to work in conjunction with the e-mail handler **326** to determine the source IP address of the sender of the message. Once the source IP address of the sender has been determined, a business heuristics-based (hereinafter, simply heuristics) module in the form of a business heuristics-based source IP address module **332** *a* assists in processing the message. The heuristics source IP module **332** *a* may be included in the EMS as one of several software application plug-ins. More specifically, the heuristics source IP module **332** *a* is configured to access a source IP address database **334** in order to compare the previously determined source IP address of the incoming message to those stored in the database **334**. Of course, the heuristics source IP module **332** *a* may also be configured to compare the destination IP address of an outgoing message to those stored in the database **334**. Thus, as used herein, the “source IP address” includes both the IP address of a sender of the message into the EMS system, as well as the IP address of a user of the EMS system who is sending the message. Once compared, if the source IP address of the message is determined to be related to the pre-selected field or type of business (e.g., the legal industry), then an overall message filtering threshold established by the user (or perhaps the administrator of the message filtering system) may be adjusted to increase the likelihood that the message will be delivered to the intended recipient, rather than being filtered out as unwanted spam. Such a threshold adjustment is discussed in greater detail below.

Also in this embodiment, another business heuristics module, in the form of a heuristics-based content module **332** *b,* has also been added among the multiple applications **332** associated with the EMS. As also discussed in greater detail below, the heuristics content module **332** *b* may be comprised of software configured to analyze the content of incoming (or outgoing) electronic messages to determine the presence of content related to predetermined industries. For example, as a message is received by the EMS, the heuristics content module **332** *b* works with the e-mail handler **326** to search/extract content within the message based on instruction code provided by the heuristics content module **332** *b.* As with heuristics filtering based on the IP address of the message, if content related to the pre-selected business is detected, then an overall message filtering threshold established by the user (and/or the administrator) may be adjusted to increase the likelihood that the message will be delivered to the intended recipient rather than being filtered out. Thus, both the heuristics IP address module **332** *a* and the heuristics content module **332** *b* may be employed to determine if the message is somehow associated with a desirable business.

As used herein, being “associated with a business” means determining that any part of the message, including the source or destination IP address, the subject line, the message text, or any attachments, is in some way related to that business or to a job within that business. For example, the source or destination IP address on the message belongs to a company or other organization known to be in or related to that business, or a part of the message may include content that is typically employed by companies or other organizations known to be in or related to that business, regardless if the sender or intended recipient is actually employed or volunteers in that line of business. As such, the disclosed heuristics process may apply to messages between two persons that are not associated with a specific business or profession, but the message includes content (or an IP address) that is determined to be associated with a designated type or field of business. Another example of being “associated with an business” includes content found to be associated with professional associations of professions related to the business. For instance, a lawyer working at a financial company may still employ and benefit from legal-based heuristics filtering even though he is working at a financial company or other non-legal entity, and not strictly in the legal industry.

In one specific embodiment, the adjustment to the overall threshold may vary based on the amount of business-based content detected in the incoming message, as well as the threshold setting for the heuristics content module **332** *b* made by either the intended recipient, the administrator, or even both. Of course, the heuristics content module **332** *b* and the heuristics source IP module **332** *a* are not limited to the exact embodiments and connections illustrated in FIG. 5. As such, persons who are ordinarily skilled in the pertinent field of technology/art will understand variations that may be made to those components and/or their corresponding connections to other components, without departing from the scope of the principles of filtering based on heuristics disclosed herein. Adjustments made based on either  module  **332** *a,*  **332** *b* are discussed in greater detail below.

Looking now at FIG. 6, illustrated is one embodiment of a screen shot **600** for setting business-specific thresholds, in accordance with the disclosed heuristics principles. Specifically, adjustment of two business-based thresholds: “Legal” and “Financial,” are illustrated. Of course, any number and/or type of business thresholds may be provided and employed with the disclosed filtering process. Also as before, once any adjustments have been made, the changes may be saved by clicking the “Save Changes” button or on the screen, or cancelled by clicking the illustrated “Cancel” button.

The business-based thresholds are provided to influence whether e-mail messages satisfy the settings of the prior base thresholds such that they are delivered to the intended recipient. More specifically, the business thresholds generally allow e-mail messages that would normally be filtered out to pass through to the intended recipient based on business heuristics. The objective of this heuristics approach to e-mail filtering is to eliminate the problem of false positives that can become an issue when using generalized spam-filtering technology. As such, the likelihood that e-mail messages will be filtered out based on the settings of the base thresholds may be reduced based on the settings of the business thresholds. Moreover, in preferred embodiments, the screen shot **600** allowing the business threshold adjustments is only available to administrators of the e-mail filtering service. In such embodiments, a user interface may be provided to intended recipients of the messages that simply allows the user to turn heuristics filtering of messages on or off. Of course, in other embodiments the intended recipients of the incoming messages are provided access to the threshold adjustment bars.

Also illustrated in FIG. 6 is the variability of the tolerance of the business thresholds. In the illustrated embodiment, as the tolerance adjustment moves from “No Extra Importance” to “Extra Importance”, the likelihood that a filtered e-mail message will be allowed to pass through to the intended recipient increases. Of course, other titles for the variable range of threshold settings may also be employed. By adjusting such threshold settings, an “effective threshold” is generated based on the settings of the original base thresholds, as modified by the settings of the business thresholds. Equation (1) sets forth an example of this relationship:

*TH* eff *=TH* base *·TH* ind  (1)

where THeff is the resulting effective threshold calculated by multiplying THbase, which is the cumulative base threshold, and THind, which is the business threshold. Stated another way, as the original overall threshold is adjusted using the setting of one of the base thresholds, the result is a base threshold THbase. Then, the business threshold THind, based on its setting(s), adjusts the base threshold THbase to make it more lenient in certain business-based situations, thus increasing the likelihood of allowing a message through to the intended recipient that would previously have been filtered out. In some embodiments, the business threshold THind may be adjusted to an extreme setting, which would virtually be determinative of the passage of an incoming message that would otherwise have been blocked from reaching the intended recipient. Determining the effective threshold is discussed in greater detail below.

Turning now to FIG. 7, with continued reference to the screen shot **400** of FIG. 4 and the screen shot **600** of FIG. 6, illustrated is a flow diagram of an exemplary process for the disclosed business heuristics-based filtering technique. To more clearly understand the function of the disclosed approach, the exemplary process of FIG. 7 will be described with reference to a specific example. It should be understood, however, that this description should not be interpreted as a limitation to the implementation of the principles described herein, including, but not limited to, the technique for assigning values and scores to the various thresholds. The process of FIG. 7 begins at a Start block **710**, wherein the disclosed e-mail filtering process is initiated.

At block **720**, an incoming electronic message (i.e., an e-mail) is intercepted by the filtering process. The filtering process (e.g., typically embodied in software) may be at a geographically distinct location from the intended recipient of the e-mail, or it may be located within the recipient's on-site e-mail server. At block **730**, a spam score is assigned to the incoming e-mail message, as mentioned above. The spam score given to the e-mail is typically based on several different criteria, and is used to indicate a likelihood that the message is not spam. For example, the source IP address and/or domain of the sender may be considered, as well as the domain of the destination IP addresses and the content of the subject line and/or body of the e-mail. Also, characteristics associated with the message may also be considered, such as whether the message is part of a mass mailing, whether the message is part of a directory harvest attack, whether the sender of the message is linked with prior spam mailings, etc. A detailed discussion of this part of the process is found in the co-pending patent application cross-referenced above. In this specific example, the spam score ranges from 0 or 100, where 0 indicates a certainty that the e-mail is spam, while a score of 100 indicates a certainty that the e-mail is not spam. In addition, the spam score assigned to each message passing therethrough is typically not changed throughout the filtering process, and is instead simply compared to various thresholds to determine whether the spam score falls below the threshold and should therefore be filtered from delivery to the intended recipient. Of course, other embodiments may also adjust the spam score, either alone or with an adjustment of the threshold.

On the other side of the process, at block **740**, membership in a particular category associated with the base thresholds is determined. Looking back at FIG. 4, the subject line and/or body (or any associated part) of the e-mail may be scanned to look for indicators that the e-mail falls under one of the content-driven base thresholds: Sexually Explicit, Get Rich Quick, Special Offers, or Racially Insensitive. Where the assigned spam score is used to generally determine whether the e-mail will be filtered out, membership in one of the enumerated categories increases the likelihood that the e-mail will be so filtered. In a specific embodiment, each of the variable settings for these four categories may represent a multiplier used to increase the chance that the spam score will not surpass a new (adjusted) threshold, and therefore the message be filtered out. For example, if the user has an original overall threshold of 40, and an incoming e-mail includes sexually explicit material but has only been assigned a spam score of 50, without detecting membership in an offending category the e-mail will be passed through to the user since its spam score exceeds the threshold value. However, if the user's setting for a category into which the e-mail falls is high, for example, a 10 multiplier, such a setting will cause the user's original overall tolerance to be increased by the multiplier if the e-mail is determined to contain the offending content. Thus, where the spam score originally fell above the overall threshold, the same spam score for this particular e-mail is now less than the newly adjusted threshold. Therefore, the e-mail will be filtered from delivery.

In effect, the settings for the content-driven base thresholds, which create multipliers as described above, indicate a user's tolerance for false positives in filtering e-mails when the e-mails are determined to fall into the content-based (i.e., offending) categories. More specifically, in the example set forth above, the user is essentially stating that he is willing to tolerate 10 times the number of false positives (with the exemplary multiplier of 10) if the content of the e-mail is determined to contain sexually explicit material. To this end, even if the e-mail receives a very high spam score, indicating a virtual certainty that it is not spam, the e-mail may still be filtered out based on its membership in the offending category (i.e., having offending content), as influenced by a high level set by the user for each category.

Moving on to block **750**, it is determined whether the source IP address of the message is associated with any of the particular industries at issue, typically by employing software plug-ins, as described above. Such a list of “approved senders” contains a list of specific source IP addresses of potential message senders so that messages from those senders are more likely to be delivered to the user's inbox based on their affiliation with an “approved” source IP address. For example, a database may be maintained that includes substantially all of the known IP addresses for all law firms in the United States. Thus, this database may be searched to determine if the source IP address for the incoming message corresponds to an address in this database. If it is determined that the source IP address is present in the database, then the user's thresholds will be adjusted on this basis, in a manner similar to that discussed above with reference to block **740**. Similar embodiments are envisioned for source IP addresses found to be associated with the financial business, such as from a bank or even between a sender and recipient that are not associated with the financial business but the content of the message is still found to be associated with the financial business (e.g., through terminology or the like).

The database of source IP addresses is typically generated and kept by the administrating organization that is administering message filtering as disclosed herein, where that list is typically kept hidden from the users and competitors alike. However, filtering systems and processes as disclosed herein are broad enough to encompass embodiments where the intended recipient of the message may edit or even entirely create the list. Additionally, the thresholds for filtering while employing such a list may be variable at the adjustment of the administrator or the user. Of course, such thresholds may also be adjusted to levels where an incoming message is almost always delivered if the sender's IP address is found to be included on the database list.

Moreover, this adjustment to the user's overall threshold is typically made based on IP addresses, not on domain name as found in conventional filtering techniques. Specifically, domain name-based approaches typically include a list of “approved senders”, and when the domain name for the message sender matches a domain in the list, the message is simply allowed to pass through to the intended recipient. However, such approaches are not effective against senders of unwanted messages that employ “spoofing” techniques to send messages. In such situations, the unwanted message would still include a domain name that has been “approved” for sending messages. Instead, the disclosed technique employs the source IP address (typically four multi-digit numbers separated by periods) of message senders to help determine whether the sent message should be filtered out. One embodiment of such an approach may include the matching of the source IP address with IP addresses of known valid senders stored in a database, but the disclosed technique is not so limited.

In some embodiments, more than a mere source IP address “look-up” in the database takes place. In such embodiments, other factors may be taken into account, such as the comparison of the sending IP address with that of the intended recipient to determine if both are members of the same business. If it is so determined, than the likelihood that the message is spam is less, and so the recipient's overall threshold may be adjusted (e.g., lowered) to reflect this likelihood. In these and other embodiments, various comparisons may be made with the source IP address using such business-based viewpoints to determine whether the user's overall threshold should be adjusted to increase the likelihood that the message will be allowed to pass through. For example, other determinations may include viewing past message traffic or connection attempts by the sending IP address (with or without consideration of any destination IP addresses) to determine if there is a pattern in such traffic/attempts that is typically associated with senders of spam rather than valid message senders. Other examples include comparing prior message traffic between the source IP address and other intended recipients within the business, or where the source IP address is assigned as related to a particular business through an external verification processes. Of course, a system and process as disclosed herein may include any such approaches, while remaining within the scope of the present disclosure and any claims issuing therefrom.

Next, at block **760**, it is determined whether content in the e-mail message is associated with specific predetermined industries. More specifically, this determination is made considering the threshold adjustment based on whether there is business content in the e-mail that corresponds to one of the pre-selected industries. Plug-in applications (see FIG. 3) may also be used to analyze the content of the e-mail looking for key terms or phrases that are typically associated with the industries. For example, if several instances of “legalese” are detected in the content of the e-mail and it is determined that the e-mail is sufficiently associated with the legal business, the user's threshold may be adjusted for comparison with the message's assigned spam score to accomplish the disclosed filtering process. As a result, if sufficient business content is detected in the message, the multiplier associated with the specific threshold may be set low enough such that the message is delivered to the intended recipient, even if the message would have been filtered out based on its spam score (or for other reasons) had no business content been found. As with the source IP addresses, a database may be used to store key terms and phrases associated with the business to accomplish the business content determination, and the disclosed technique is not limited to industries in which the intended recipient works. Moreover, a process conducted in accordance with the principles disclosed herein may include  blocks  **750** and **760** in any order, or may even be conducted simultaneously, without departing from the scope of this disclosure.

If no business association is found in the e-mail content, then the process moves on to block **780**. At this block, filtering of the e-mail is conducted based on a comparison of its assigned spam score to the current overall threshold value. If at block **740** it was determined that the content of the e-mail did not warrant membership in any of the offending categories, then the filtering is done using the original overall threshold. To this end, if the spam score does not exceed the original threshold, then delivery of the e-mail to the intended recipient is blocked. However, if membership in one of the offending categories was determined, then the filtering is based on a comparison between the assigned spam score and the adjusted overall thresholds. Specifically, as mentioned above, category membership may result in the overall threshold value being increased (depending on the setting established by the user or system administrator), so as to decrease the likelihood that the e-mail will be allowed to the reach the user. Thus, if the spam score does not exceed the adjusted overall threshold value, then delivery of the e-mail to the intended recipient is blocked. Conversely, in either case, if the spam score should exceed either the original or adjusted overall thresholds, then the e-mail will be delivered to the user.

If it was determined at block **760** that there is an association with any of the selected industries, whether based on the business-related source IP address (block **750**) and/or the business-based content determination, the process instead moves to block **790**. At this block, the e-mail is filtered based on a comparison of its assigned spam score to the effective threshold value, as adjusted in accordance with  blocks  **750** and **760**. The effective threshold is determined as described above, where the overall threshold is typically decreased depending on the settings established by the user and/or the system administrator. Like the base threshold values, the business threshold values include multipliers of the original overall threshold. However, where the base threshold values were multipliers greater than 1 (in order to increase the overall threshold and increase the chance of filtering out the message in this embodiment), the multipliers for the business threshold values may all be less than 1. Thus, in such embodiments, multiplying the overall threshold value with such a fractional multiplier decreases that overall threshold value, which increases the chance that the message will be allowed through the filtering process and be delivered to the intended recipient.

The increase in the likelihood of passing through is true regardless of whether the original overall threshold or an adjusted overall threshold is used. This advantage of the disclosed approach is particularly beneficial when an e-mail has been categorized into one of the offending categories, but yet is actually an important and desired e-mail for the intended recipient to have. In a specific example, an e-mail that is determined to include a number of racial slurs therein will likely be categorized under the “Racially Insensitive” base threshold. Moreover, since the recipient has set this base threshold at the maximum, in this example, there is even a less likely chance that the e-mail will reach the intended recipient.

However, if the e-mail actually includes legal documents pertaining to a suit based on the use of those racial slurs, then the e-mail would be filtered out improperly. To prevent such a false positive, the disclosed approach allows the threshold to be adjusted based on the content of the e-mail (or perhaps the source IP address), if associated with, for example, the legal industry. In essence, the use of the business threshold multipliers allows a user to essentially state that less false positives will be tolerated if an association to the selected industries in the business thresholds is determine to exist. Thus, if the e-mail did contain such legal content, then the overall threshold will typically be decreased in this embodiment by the multiplier corresponding to the setting established in the “Legal” business threshold. As a result, the likelihood that the e-mail will be allowed to reach the recipient is therefore increased. Additionally, the amount of the multiplier (and thus the amount of adjustment to the overall threshold) may be established, in one embodiment, by the intended recipient by an adjustment in the settings for separate thresholds for each business.

A similar result may be attained if the source IP address or domain is found to be associated with the legal industry. For example, assuming that the domain used by a prestigious law firm has been identified in the source (or destination) IP address contained in the e-mail. In this example, while the e-mail may contain racial slurs therein, the likelihood that a prestigious law firm (whose source domain has been identified in the e-mail and matched to a database of approved senders) is sending out (or being sent) racially insensitive e-mail as spam is very remote. Unfortunately, however, the classification of the e-mail as “Racially Insensitive” based on its content will greatly decrease the chance for the e-mail to pass through the filtering process. By employing the disclosed technique, however, the overall threshold, although adjusted due to category membership, may then be decreased based on determined business association to create a more lenient effective threshold, and thus increase the chance that this particular e-mail will reach the intended recipient. Of course, in some embodiments, the process may simply be configured to definitively deliver the incoming message to the intended recipient if the source IP address of the message has been determined to be associated with one of the predetermined industries, although approval is based on association with a predetermined business, in accordance with the disclosed principles.

While various embodiments of systems and methods for filtering electronic messages according to the business heuristics-based principles disclosed herein have been disclosed, it should be understood that they have been presented by way of example only, and not limitation. Thus, the breadth and scope of the invention(s) should not be limited by any of the above-described exemplary embodiments, but should be defined only in accordance with the following claims and their equivalents. Moreover, the above advantages and features are effected in described embodiments, but shall not limit the application of the claims to processes and structures accomplishing any or all of the above advantages.

Additionally, the section headings herein are provided for consistency with the suggestions under 37 CFR 1.77 or otherwise to provide organizational cues. These headings shall not limit or characterize the invention(s) set out in any claims that may issue from this disclosure. Specifically and by way of example, although the headings refer to a “Technical Field,” the claims should not be limited by the language chosen under this heading to describe the so-called technical field. Further, a description of a technology in the “Background” is not to be construed as an admission that technology is prior art to any invention(s) in this disclosure. Neither is the “Brief Summary” to be considered as a characterization of the invention(s) set forth in the claims found herein. Furthermore, any reference in this disclosure to “invention” in the singular should not be used to argue that there is only a single point of novelty claimed in this disclosure. Multiple inventions may be set forth according to the limitations of the multiple claims associated with this disclosure, and the claims accordingly define the invention(s), and their equivalents, that are protected thereby. In all instances, the scope of the claims shall be considered on their own merits in light of the specification, but should not be constrained by the headings set forth herein.

## Claims (40)

1. A method of filtering an electronic message using business heuristics, the method comprising:

receiving an electronic message at a message management server operating on a computer network;

examining, using a message handler associated with the management server, the electronic message for characteristics indicative of its desirability or undesirability to an intended recipient of the electronic message;

establishing, with the message handler and based on the examination, a likelihood that delivery of the electronic message to the intended recipient should be blocked;

determining whether the electronic message is associated with a desirable business using one or more heuristics modules associated with the message handler; and

automatically decreasing, with the message handler, the likelihood that delivery of the electronic message to the intended recipient should be blocked if the electronic message is determined to be associated with the desirable business.

2. A method according to claim 1, wherein establishing a likelihood that delivery of the electronic message to the intended recipient should be blocked comprises assigning a spam-score to the electronic message based on the examination, and wherein decreasing the likelihood that delivery of the electronic message should be blocked comprises adjusting the spam-score, the method further comprising blocking or delivering the electronic message to the intended recipient according to a comparison of the adjusted spam-score to an overall threshold.

3. A method according to claim 2, wherein blocking or delivering the electronic message further comprises blocking delivery of the electronic message to the intended recipient when the adjusted spam-score does not exceed the overall threshold.

4. A method according to claim 1, wherein establishing a likelihood that delivery of the electronic message to the intended recipient should be blocked comprises assigning a spam-score to the electronic message based on the examination, and wherein decreasing the likelihood that delivery of the electronic message should be blocked comprises adjusting an overall threshold, the method further comprising blocking or delivering the electronic message to the intended recipient according to a comparison of the spam-score to the adjusted overall threshold.

5. A method according to claim 1, wherein the determining comprises determining whether the source of the electronic message is associated with the desirable business, the adjusting further comprising adjusting the likelihood of blocking delivery of the electronic message to the intended recipient if the source of the electronic message is determined to be associated with the desirable business.

6. A method according to claim 5, wherein the decreasing the likelihood that delivery of the electronic message should be blocked further comprises decreasing an overall threshold to accomplish delivery of the message if the source of the electronic message is determined to be associated with the desirable business.

7. A method according to claim 5, wherein the source comprises an Internet Protocol (IP) address of a sending server of the electronic message.

8. A method according to claim 7, wherein determining whether the source is related to the desirable business comprises one or more of comparing the IP address of the source to at least one of an IP address of the intended recipient, comparing prior connection attempts by the source IP address to the intended recipient, comparing prior message traffic between the source IP address and the intended recipient, comparing prior message traffic between the source IP address and other intended recipients within the business, or determining if the source IP address is assigned to be related to a particular business through external verification processes.

9. A method according to claim 1, wherein determining comprises determining the presence of business content in the electronic message likely to be used by the desirable business, the decreasing further comprising decreasing the likelihood that delivery of the electronic message to the intended recipient should be blocked if the business content is determined to be present in the electronic message.

10. A method according to claim 9, wherein establishing a likelihood that delivery of the electronic message to the intended recipient should be blocked comprises assigning a spam-score to the electronic message based on the examination, the method further comprising:

creating an effective threshold by adjusting an overall threshold based on the presence of the business content, and

blocking delivery of the electronic message to the intended recipient if the spam-score does not cross the effective threshold.

11. A method according to claim 9, further comprising establishing a business threshold to govern the determining of the presence of business content.

12. A method according to claim 11, further comprising creating an effective threshold by adjusting an overall threshold by an amount proportional to an amount of the business threshold.

13. A method according to claim 11, wherein the amount of the business threshold is established by an administrator of the method of filtering for the intended recipient.

14. A method according to claim 10, further comprising determining the presence of offending content in the electronic message corresponding to at least one base threshold, the presence of the offending content adjusting the overall threshold prior to creating the effective threshold.

15. A method according to claim 14, wherein the amount of the at least one base threshold is established by the intended recipient of the electronic message.

16. A method according to claim 14, wherein the at least one base threshold is a content-based tolerance of electronic messages associated with categories selected from the group consisting of sexually explicit content, get-rich-quick content, special-offers content, and racially insensitive content.

17. A method according to claim 14, further comprising adjusting the overall threshold by an amount proportional to an amount of the at least one base threshold.

18. A method according to claim 10, wherein the overall threshold is established by the intended recipient of the electronic message.

19. A method according to claim 1, wherein the desirable business is selected from the group consisting of the legal profession and financial professions.

20. A method according to claim 1, wherein the intended recipient is associated with the desirable business.

21. A computer-readable storage medium containing a set of instructions executable by a computer for performing the process of:

examining an electronic message for characteristics indicative of its desirability or undesirability to an intended recipient of the electronic message;

calculating, based on the examination, a likelihood that delivery of the electronic message to the intended recipient should be blocked;

determining whether the electronic message is associated with a desirable business; and

automatically decreasing the calculated likelihood that delivery of the electronic message to the intended recipient should be blocked if the electronic message is determined to be associated with the desirable business.

22. A computer-readable storage medium according to claim 21, wherein establishing a likelihood that delivery of the electronic message to the intended recipient should be blocked comprises assigning a spam-score to the electronic message based on the examination, and wherein decreasing the likelihood that delivery of the electronic message should be blocked comprises adjusting the spam-score, the method further comprising blocking or delivering the electronic message to the intended recipient according to a comparison of the adjusted spam-score to an overall threshold.

23. A computer-readable storage medium according to claim 22, wherein blocking or delivering the electronic message further comprises blocking delivery of the electronic message to the intended recipient when the adjusted spam-score does not exceed the overall threshold.

24. A computer-readable storage medium according to claim 21, wherein establishing a likelihood that delivery of the electronic message to the intended recipient should be blocked comprises assigning a spam-score to the electronic message based on the examination, and wherein decreasing the likelihood that delivery of the electronic message should be blocked comprises adjusting an overall threshold, the method further comprising blocking or delivering the electronic message to the intended recipient according to a comparison of the spam-score to the adjusted overall threshold.

25. A computer-readable storage medium according to claim 21, wherein the determining comprises determining whether the source of the electronic message is associated with the desirable business, the adjusting further comprising adjusting the likelihood of blocking delivery of the electronic message to the intended recipient if the source of the electronic message is determined to be associated with the desirable business.

26. A computer-readable storage medium according to claim 25, wherein the decreasing the likelihood that delivery of the electronic message should be blocked further comprises decreasing an overall threshold to accomplish delivery of the message if the source of the electronic message is determined to be associated with the desirable business.

27. A computer-readable storage medium according to claim 25, wherein the source comprises an Internet Protocol (IP) address of a sending server of the electronic message.

28. A computer-readable storage medium according to claim 27, wherein determining whether the source is related to the desirable business comprises one or more of comparing the IP address of the source to at least one of an IP address of the intended recipient, comparing prior connection attempts by the source IP address to the intended recipient, comparing prior message traffic between the source IP address and the intended recipient, comparing prior message traffic between the source IP address and other intended recipients within the business, or determining if the source IP address is assigned to be related to a particular business through external verification processes.

29. A computer-readable storage medium according to claim 21, wherein determining comprises determining the presence of business content in the electronic message likely to be used by the desirable business, the decreasing further comprising decreasing the likelihood that delivery of the electronic message to the intended recipient should be blocked if the business content is determined to be present in the electronic message.

30. A computer-readable storage medium according to claim 29, wherein establishing a likelihood that delivery of the electronic message to the intended recipient should be blocked comprises assigning a spam-score to the electronic message based on the examination, the method further comprising:

creating an effective threshold by adjusting an overall threshold based on the presence of the business content, and

blocking delivery of the electronic message to the intended recipient if the spam-score does not cross the effective threshold.

31. A computer-readable storage medium according to claim 29, further comprising establishing a business threshold to govern the determining of the presence of business content.

32. A computer-readable storage medium according to claim 31, further comprising creating an effective threshold by adjusting an overall threshold by an amount proportional to an amount of the business threshold.

33. A computer-readable storage medium according to claim 31, wherein the amount of the business threshold is established by an administrator of the method of filtering for the intended recipient.

34. A computer-readable storage medium according to claim 30, further comprising determining the presence of offending content in the electronic message corresponding to at least one base threshold, the presence of the offending content adjusting the overall threshold prior to creating the effective threshold.

35. A computer-readable storage medium according to claim 34, wherein the amount of the at least one base threshold is established by the intended recipient of the electronic message.

36. A computer-readable storage medium according to claim 34, wherein the at least one base threshold is a content-based tolerance of electronic messages associated with categories selected from the group consisting of sexually explicit content, get-rich-quick content, special-offers content, and racially insensitive content.

37. A computer-readable storage medium according to claim 34, further comprising adjusting the overall threshold by an amount proportional to an amount of the at least one base threshold.

38. A computer-readable storage medium according to claim 30, wherein the overall threshold is established by the intended recipient of the electronic message.

39. A computer-readable storage medium according to claim 21, wherein the desirable business is selected from the group consisting of the legal profession and financial professions.

40. A computer-readable storage medium according to claim 21, wherein the intended recipient is associated with the desirable business.

US10/832,407
2004-04-26
2004-04-26
System and method for filtering electronic messages using business heuristics
Expired - Lifetime
[US7647321B2
(en)](/patent/US7647321B2/en)

## Priority Applications (9)

| Application Number | Priority Date | Filing Date | Title |
| --- | --- | --- | --- |
| US10/832,407 [US7647321B2 (en)](/patent/US7647321B2/en) | 2004-04-26 | 2004-04-26 | System and method for filtering electronic messages using business heuristics |
| AU2005241402A [AU2005241402B2 (en)](/patent/AU2005241402B2/en) | 2004-04-26 | 2005-03-29 | System and method for filtering electronic messages using business heuristics |
| EP05733019A [EP1763789A4 (en)](/patent/EP1763789A4/en) | 2004-04-26 | 2005-03-29 | SYSTEM AND METHOD FOR FILTERING ELECTRONIC MESSAGES THROUGH HEURISTIC EVALUATION OF COMMERCIAL ACTIVITY |
| JP2007510738A [JP4960222B2 (en)](/patent/JP4960222B2/en) | 2004-04-26 | 2005-03-29 | System and method for filtering electronic messages using business heuristics |
| CNA200580013218XA [CN1977263A (en)](/patent/CN1977263A/en) | 2004-04-26 | 2005-03-29 | System and method for filtering electronic messages using business heuristics |
| CA2564232A [CA2564232C (en)](/patent/CA2564232C/en) | 2004-04-26 | 2005-03-29 | System and method for filtering electronic messages using business heuristics |
| KR1020067024774A [KR101208943B1 (en)](/patent/KR101208943B1/en) | 2004-04-26 | 2005-03-29 | System and method for filtering electronic messages using business heuristics |
| PCT/US2005/010276 [WO2005109234A2 (en)](/patent/WO2005109234A2/en) | 2004-04-26 | 2005-03-29 | System and method for filtering electronic messages using business heuristics |
| US12/634,436 [US8321432B2 (en)](/patent/US8321432B2/en) | 2004-04-26 | 2009-12-09 | System and method for filtering electronic messages using business heuristics |

## Applications Claiming Priority (1)

| Application Number | Priority Date | Filing Date | Title |
| --- | --- | --- | --- |
| US10/832,407 [US7647321B2 (en)](/patent/US7647321B2/en) | 2004-04-26 | 2004-04-26 | System and method for filtering electronic messages using business heuristics |

## Related Child Applications (1)

| Application Number | Title | Priority Date | Filing Date |
| --- | --- | --- | --- |
| US12/634,436 Division [US8321432B2 (en)](/patent/US8321432B2/en) | 2004-04-26 | 2009-12-09 | System and method for filtering electronic messages using business heuristics |

## Publications (2)

| Publication Number | Publication Date |
| --- | --- |
| US20050240617A1 [US20050240617A1 (en)](/patent/US20050240617A1/en) | 2005-10-27 |
| US7647321B2 true [US7647321B2 (en)](/patent/US7647321B2/en) | 2010-01-12 |

# Family

## ID=35137736

## Family Applications (2)

| Application Number | Title | Priority Date | Filing Date |
| --- | --- | --- | --- |
| US10/832,407 Expired - Lifetime [US7647321B2 (en)](/patent/US7647321B2/en) | 2004-04-26 | 2004-04-26 | System and method for filtering electronic messages using business heuristics |
| US12/634,436 Expired - Fee Related [US8321432B2 (en)](/patent/US8321432B2/en) | 2004-04-26 | 2009-12-09 | System and method for filtering electronic messages using business heuristics |

## Family Applications After (1)

| Application Number | Title | Priority Date | Filing Date |
| --- | --- | --- | --- |
| US12/634,436 Expired - Fee Related [US8321432B2 (en)](/patent/US8321432B2/en) | 2004-04-26 | 2009-12-09 | System and method for filtering electronic messages using business heuristics |

## Country Status (8)

| Country | Link |
| --- | --- |
| US (2) | [US7647321B2 (en)](/patent/US7647321B2/en) |
| EP (1) | [EP1763789A4 (en)](/patent/EP1763789A4/en) |
| JP (1) | [JP4960222B2 (en)](/patent/JP4960222B2/en) |
| KR (1) | [KR101208943B1 (en)](/patent/KR101208943B1/en) |
| CN (1) | [CN1977263A (en)](/patent/CN1977263A/en) |
| AU (1) | [AU2005241402B2 (en)](/patent/AU2005241402B2/en) |
| CA (1) | [CA2564232C (en)](/patent/CA2564232C/en) |
| WO (1) | [WO2005109234A2 (en)](/patent/WO2005109234A2/en) |

## Cited By (10)

\* Cited by examiner, † Cited by third party

| Publication number | Priority date | Publication date | Assignee | Title |
| --- | --- | --- | --- | --- |
| [US20070294765A1 (en)](/patent/US20070294765A1/en) \* | 2004-07-13 | 2007-12-20 | Sonicwall, Inc. | Managing infectious forwarded messages |
| [US20080104703A1 (en)](/patent/US20080104703A1/en) \* | 2004-07-13 | 2008-05-01 | Mailfrontier, Inc. | Time Zero Detection of Infectious Messages |
| [US20080114838A1 (en)](/patent/US20080114838A1/en) \* | 2006-11-13 | 2008-05-15 | International Business Machines Corporation | Tracking messages in a mentoring environment |
| [US20080178288A1 (en)](/patent/US20080178288A1/en) \* | 2007-01-24 | 2008-07-24 | Secure Computing Corporation | Detecting Image Spam |
| [US20080184366A1 (en)](/patent/US20080184366A1/en) \* | 2004-11-05 | 2008-07-31 | Secure Computing Corporation | Reputation based message processing |
| [US20090064332A1 (en)](/patent/US20090064332A1/en) \* | 2007-04-04 | 2009-03-05 | Phillip Andrew Porras | Method and apparatus for generating highly predictive blacklists |
| [US20090125980A1 (en)](/patent/US20090125980A1/en) \* | 2007-11-09 | 2009-05-14 | Secure Computing Corporation | Network rating |
| [US7890590B1 (en)](/patent/US7890590B1/en) \* | 2007-09-27 | 2011-02-15 | Symantec Corporation | Variable bayesian handicapping to provide adjustable error tolerance level |
| [US20120240228A1 (en)](/patent/US20120240228A1/en) \* | 2007-01-24 | 2012-09-20 | Mcafee, Inc. | Multi-dimensional reputation scoring |
| [US20120259929A1 (en)](/patent/US20120259929A1/en) \* | 2011-04-11 | 2012-10-11 | Microsoft Corporation | Geo-data spam filter |

## Families Citing this family (41)

\* Cited by examiner, † Cited by third party

| Publication number | Priority date | Publication date | Assignee | Title |
| --- | --- | --- | --- | --- |
| [US8037144B2 (en)](/patent/US8037144B2/en) \* | 2004-05-25 | 2011-10-11 | Google Inc. | Electronic message source reputation information system |
| [US7873695B2 (en)](/patent/US7873695B2/en) | 2004-05-29 | 2011-01-18 | Ironport Systems, Inc. | Managing connections and messages at a server by associating different actions for both different senders and different recipients |
| [US7849142B2 (en)](/patent/US7849142B2/en) \* | 2004-05-29 | 2010-12-07 | Ironport Systems, Inc. | Managing connections, messages, and directory harvest attacks at a server |
| [US8484295B2 (en)](/patent/US8484295B2/en) | 2004-12-21 | 2013-07-09 | Mcafee, Inc. | Subscriber reputation filtering method for analyzing subscriber activity and detecting account misuse |
| [US7680890B1 (en)](/patent/US7680890B1/en) | 2004-06-22 | 2010-03-16 | Wei Lin | Fuzzy logic voting method and system for classifying e-mail using inputs from multiple spam classifiers |
| [US7953814B1 (en)](/patent/US7953814B1/en) | 2005-02-28 | 2011-05-31 | Mcafee, Inc. | Stopping and remediating outbound messaging abuse |
| [US8880611B1 (en)](/patent/US8880611B1/en) | 2004-06-30 | 2014-11-04 | Google Inc. | Methods and apparatus for detecting spam messages in an email system |
| [US9398037B1 (en)](/patent/US9398037B1/en) \* | 2004-09-27 | 2016-07-19 | Radix Holdings, Llc | Detecting and processing suspicious network communications |
| [US8495144B1 (en)](/patent/US8495144B1/en) \* | 2004-10-06 | 2013-07-23 | Trend Micro Incorporated | Techniques for identifying spam e-mail |
| [US9160755B2 (en)](/patent/US9160755B2/en) | 2004-12-21 | 2015-10-13 | Mcafee, Inc. | Trusted communication network |
| [US9015472B1 (en)](/patent/US9015472B1/en) | 2005-03-10 | 2015-04-21 | Mcafee, Inc. | Marking electronic messages to indicate human origination |
| [US8738708B2 (en)](/patent/US8738708B2/en) | 2004-12-21 | 2014-05-27 | Mcafee, Inc. | Bounce management in a trusted communication network |
| [US7908328B1 (en)](/patent/US7908328B1/en) \* | 2004-12-27 | 2011-03-15 | Microsoft Corporation | Identification of email forwarders |
| [JP4158927B2 (en)](/patent/JP4158927B2/en) \* | 2005-03-25 | 2008-10-01 | インターナショナル・ビジネス・マシーンズ・コーポレーション | Information presentation device, information presentation method, and program |
| [US20060224673A1 (en)](/patent/US20060224673A1/en) \* | 2005-03-30 | 2006-10-05 | Microsoft Corporation | Throttling inbound electronic messages in a message processing system |
| [JP4669348B2 (en)](/patent/JP4669348B2/en) \* | 2005-05-11 | 2011-04-13 | 株式会社エヌ・ティ・ティ・ドコモ | Spam mail discrimination device and spam mail discrimination method |
| [US7836132B2 (en)](/patent/US7836132B2/en) \* | 2005-12-13 | 2010-11-16 | Microsoft Corporation | Delivery confirmation for e-mail |
| [US8161119B2 (en)](/patent/US8161119B2/en) \* | 2006-12-22 | 2012-04-17 | Cisco Technology, Inc. | Network device provided spam reporting button for instant messaging |
| [US8046415B2 (en)](/patent/US8046415B2/en) \* | 2007-02-09 | 2011-10-25 | Cisco Technology, Inc. | Throttling of mass mailings using network devices |
| [US20100287246A1 (en)](/patent/US20100287246A1/en) \* | 2007-02-14 | 2010-11-11 | Thomas Klos | System for processing electronic mail messages with specially encoded addresses |
| [JP5046158B2 (en)](/patent/JP5046158B2/en) \* | 2007-08-10 | 2012-10-10 | インターナショナル・ビジネス・マシーンズ・コーポレーション | Apparatus and method for detecting characteristics of an e-mail message |
| [JP5020152B2 (en)](/patent/JP5020152B2/en) \* | 2008-04-10 | 2012-09-05 | ヤフー株式会社 | Web page search apparatus, method, and computer program using spam declaration |
| [US10354229B2 (en)](/patent/US10354229B2/en) | 2008-08-04 | 2019-07-16 | Mcafee, Llc | Method and system for centralized contact management |
| [US8195753B2 (en)](/patent/US8195753B2/en) \* | 2009-01-07 | 2012-06-05 | Microsoft Corporation | Honoring user preferences in email systems |
| [US8959157B2 (en)](/patent/US8959157B2/en) \* | 2009-06-26 | 2015-02-17 | Microsoft Corporation | Real-time spam look-up system |
| [US8412847B2 (en)](/patent/US8412847B2/en) \* | 2009-11-02 | 2013-04-02 | Demandbase, Inc. | Mapping network addresses to organizations |
| [US8745143B2 (en)](/patent/US8745143B2/en) | 2010-04-01 | 2014-06-03 | Microsoft Corporation | Delaying inbound and outbound email messages |
| [US9152946B2 (en)](/patent/US9152946B2/en) | 2010-05-21 | 2015-10-06 | Brokersavant Inc. | Apparatuses, methods and systems for a lead generating hub |
| [US9111282B2 (en)](/patent/US9111282B2/en) \* | 2011-03-31 | 2015-08-18 | Google Inc. | Method and system for identifying business records |
| [US8745040B2 (en)](/patent/US8745040B2/en) \* | 2011-06-27 | 2014-06-03 | Bmc Software, Inc. | Service context |
| [US8818994B2 (en)](/patent/US8818994B2/en) \* | 2011-06-27 | 2014-08-26 | Bmc Software, Inc. | Mobile service context |
| [US20130073568A1 (en)](/patent/US20130073568A1/en) \* | 2011-09-21 | 2013-03-21 | Vladimir Federov | Ranking structured objects and actions on a social networking system |
| [US8700913B1 (en)](/patent/US8700913B1/en) | 2011-09-23 | 2014-04-15 | Trend Micro Incorporated | Detection of fake antivirus in computers |
| [WO2013183115A1 (en)](/patent/WO2013183115A1/en) \* | 2012-06-05 | 2013-12-12 | 株式会社日立製作所 | Log management system and program |
| [US20140358939A1 (en)](/patent/US20140358939A1/en) \* | 2013-05-31 | 2014-12-04 | Emailvision Holdings Limited | List hygiene tool |
| [US8892672B1 (en)](/patent/US8892672B1/en) \* | 2014-01-28 | 2014-11-18 | Fmr Llc | Detecting unintended recipients of electronic communications |
| [US10171403B2 (en)](/patent/US10171403B2/en) | 2015-11-30 | 2019-01-01 | International Business Machines Corporation | Determining intended electronic message recipients via linguistic profiles |
| [US11115359B2 (en)](/patent/US11115359B2/en) \* | 2016-11-03 | 2021-09-07 | Samsung Electronics Co., Ltd. | Method and apparatus for importance filtering a plurality of messages |
| [US10839353B2 (en)](/patent/US10839353B2/en) | 2018-05-24 | 2020-11-17 | Mxtoolbox, Inc. | Systems and methods for improved email security by linking customer domains to outbound sources |
| [US11539541B1 (en)](/patent/US11539541B1/en) \* | 2019-03-18 | 2022-12-27 | 8X8, Inc. | Apparatuses and methods involving data-communications room predictions |
| [US11082373B1 (en)](/patent/US11082373B1/en) | 2020-03-11 | 2021-08-03 | Vmware, Inc. | Context driven dynamic actions embedded in messages |

## Citations (76)

\* Cited by examiner, † Cited by third party

| Publication number | Priority date | Publication date | Assignee | Title |
| --- | --- | --- | --- | --- |
| [US4837798A (en)](/patent/US4837798A/en) | 1986-06-02 | 1989-06-06 | American Telephone And Telegraph Company | Communication system having unified messaging |
| [WO1996035994A1 (en)](/patent/WO1996035994A1/en) | 1995-05-08 | 1996-11-14 | Compuserve Incorporated | Rules based electronic message management system |
| [WO1997012321A1 (en)](/patent/WO1997012321A1/en) | 1995-09-26 | 1997-04-03 | Trend Micro, Incorporated | Virus detection and removal apparatus for computer networks |
| [US5619648A (en)](/patent/US5619648A/en) | 1994-11-30 | 1997-04-08 | Lucent Technologies Inc. | Message filtering techniques |
| [US5627764A (en)](/patent/US5627764A/en) | 1991-10-04 | 1997-05-06 | Banyan Systems, Inc. | Automatic electronic messaging system with feedback and work flow administration |
| [US5634005A (en)](/patent/US5634005A/en) | 1992-11-09 | 1997-05-27 | Kabushiki Kaisha Toshiba | System for automatically sending mail message by storing rule according to the language specification of the message including processing condition and processing content |
| [WO1997027546A1 (en)](/patent/WO1997027546A1/en) | 1996-01-26 | 1997-07-31 | Ex Machina, Inc. | System and method for transmission of data |
| [US5742668A (en)](/patent/US5742668A/en) | 1994-09-19 | 1998-04-21 | Bell Communications Research, Inc. | Electronic massaging network |
| [US5771355A (en)](/patent/US5771355A/en) | 1995-12-21 | 1998-06-23 | Intel Corporation | Transmitting electronic mail by either reference or value at file-replication points to minimize costs |
| [US5796948A (en)](/patent/US5796948A/en) | 1996-11-12 | 1998-08-18 | Cohen; Elliot D. | Offensive message interceptor for computers |
| [WO1998037680A2 (en)](/patent/WO1998037680A2/en) | 1997-02-25 | 1998-08-27 | Intervoice Limited Partnership | E-mail server for message filtering and routing |
| [US5832208A (en)](/patent/US5832208A/en) | 1996-09-05 | 1998-11-03 | Cheyenne Software International Sales Corp. | Anti-virus agent for use with databases and mail servers |
| [US5844969A (en)](/patent/US5844969A/en) | 1997-01-23 | 1998-12-01 | At&T Corp. | Communication system, method and device for remotely re-transmitting received electronic mail directed to a destination terminal to a new destination terminal |
| [WO1999006929A2 (en)](/patent/WO1999006929A2/en) | 1997-08-03 | 1999-02-11 | At & T Corp. | An extensible proxy framework for e-mail agents |
| [US5889943A (en)](/patent/US5889943A/en) | 1995-09-26 | 1999-03-30 | Trend Micro Incorporated | Apparatus and method for electronic mail virus detection and elimination |
| [US5905777A (en)](/patent/US5905777A/en) | 1996-09-27 | 1999-05-18 | At&T Corp. | E-mail paging system |
| [US5937162A (en)](/patent/US5937162A/en) | 1995-04-06 | 1999-08-10 | Exactis.Com, Inc. | Method and apparatus for high volume e-mail delivery |
| [US5968117A (en)](/patent/US5968117A/en) | 1998-01-20 | 1999-10-19 | Aurora Communications Exchange Ltd. | Device and system to facilitate accessing electronic mail from remote user-interface devices |
| [US5987611A (en)](/patent/US5987611A/en) | 1996-12-31 | 1999-11-16 | Zone Labs, Inc. | System and methodology for managing internet access on a per application basis for client computers connected to the internet |
| [US5999932A (en)](/patent/US5999932A/en) | 1998-01-13 | 1999-12-07 | Bright Light Technologies, Inc. | System and method for filtering unsolicited electronic mail messages using data matching and heuristic processing |
| [WO1999065256A2 (en)](/patent/WO1999065256A2/en) | 1998-06-10 | 1999-12-16 | Logica, Inc. | System and method for delivering e-mail notification to mobile phones |
| [WO1999067731A1 (en)](/patent/WO1999067731A1/en) | 1998-06-23 | 1999-12-29 | Microsoft Corporation | A technique which utilizes a probabilistic classifier to detect 'junk' e-mail |
| [US6014429A (en)](/patent/US6014429A/en) | 1996-08-12 | 2000-01-11 | Lucent Technologies, Inc. | Two-way wireless messaging system with transaction server |
| [US6023723A (en)](/patent/US6023723A/en) | 1997-12-22 | 2000-02-08 | Accepted Marketing, Inc. | Method and system for filtering unwanted junk e-mail utilizing a plurality of filtering mechanisms |
| [US6052709A (en)](/patent/US6052709A/en) | 1997-12-23 | 2000-04-18 | Bright Light Technologies, Inc. | Apparatus and method for controlling delivery of unsolicited electronic mail |
| [US6061718A (en)](/patent/US6061718A/en) | 1997-07-23 | 2000-05-09 | Ericsson Inc. | Electronic mail delivery system in wired or wireless communications system |
| [US6073165A (en)](/patent/US6073165A/en) | 1997-07-29 | 2000-06-06 | Jfax Communications, Inc. | Filtering computer network messages directed to a user's e-mail box based on user defined filters, and forwarding a filtered message to the user's receiver |
| [US6075863A (en)](/patent/US6075863A/en) | 1996-02-28 | 2000-06-13 | Encanto Networks | Intelligent communication device |
| [US6092194A (en)](/patent/US6092194A/en) | 1996-11-08 | 2000-07-18 | Finjan Software, Ltd. | System and method for protecting a computer and a network from hostile downloadables |
| [WO2000042747A1 (en)](/patent/WO2000042747A1/en) | 1999-01-13 | 2000-07-20 | Soobok Lee | Internet e-mail add-on service system |
| [WO2000049776A1 (en)](/patent/WO2000049776A1/en) | 1999-02-17 | 2000-08-24 | Argo Interactive Limited | Method and apparatus for proxying and filtering electronic mail |
| [US6112227A (en)](/patent/US6112227A/en) | 1998-08-06 | 2000-08-29 | Heiner; Jeffrey Nelson | Filter-in method for reducing junk e-mail |
| [US6118856A (en)](/patent/US6118856A/en) | 1998-12-28 | 2000-09-12 | Nortel Networks Corporation | Method and apparatus for automatically forwarding an email message or portion thereof to a remote device |
| [US6138146A (en)](/patent/US6138146A/en) | 1997-09-29 | 2000-10-24 | Ericsson Inc. | Electronic mail forwarding system and method |
| [US6146026A (en)](/patent/US6146026A/en) | 1996-12-27 | 2000-11-14 | Canon Kabushiki Kaisha | System and apparatus for selectively publishing electronic-mail |
| [US6147987A (en)](/patent/US6147987A/en) | 1997-04-08 | 2000-11-14 | 3Com Corporation | Supporting load sharing across multiple network access servers |
| [US6178331B1 (en)](/patent/US6178331B1/en) | 1997-06-17 | 2001-01-23 | Bulletin.Net, Inc. | System and process for allowing wireless messaging |
| [US6249805B1 (en)](/patent/US6249805B1/en) | 1997-08-12 | 2001-06-19 | Micron Electronics, Inc. | Method and system for filtering unauthorized electronic mail messages |
| [US6249807B1 (en)](/patent/US6249807B1/en) | 1998-11-17 | 2001-06-19 | Kana Communications, Inc. | Method and apparatus for performing enterprise email management |
| [WO2001046867A1 (en)](/patent/WO2001046867A1/en) | 1999-12-22 | 2001-06-28 | Setnet Corp. | Industrial capacity clustered mail server system and method |
| [US6263202B1 (en)](/patent/US6263202B1/en) | 1998-01-28 | 2001-07-17 | Uniden Corporation | Communication system and wireless communication terminal device used therein |
| [US6266664B1 (en)](/patent/US6266664B1/en) \* | 1997-10-01 | 2001-07-24 | Rulespace, Inc. | Method for scanning, analyzing and rating digital information content |
| [US6301245B1 (en)](/patent/US6301245B1/en) | 1998-06-09 | 2001-10-09 | Unisys Corporation | Universal Messaging system providing integrated voice, data and fax messaging services to PC/web-based clients, including a large object server for efficiently distributing voice/fax messages to web-based clients |
| [US20010032095A1 (en)](/patent/US20010032095A1/en) | 2000-01-14 | 2001-10-18 | Balbach Carl Teo | Context-specific contact information |
| [US6317751B1 (en)](/patent/US6317751B1/en) | 1998-09-28 | 2001-11-13 | Merrill Lynch & Co., Inc. | Compliance archival data process and system |
| [US6321267B1 (en)](/patent/US6321267B1/en) | 1999-11-23 | 2001-11-20 | Escom Corporation | Method and apparatus for filtering junk email |
| [US6334140B1 (en)](/patent/US6334140B1/en) | 1997-09-25 | 2001-12-25 | Nec Corporation | Electronic mail server in which electronic mail is processed |
| [US6335966B1 (en)](/patent/US6335966B1/en) | 1999-03-29 | 2002-01-01 | Matsushita Graphic Communication Systems, Inc. | Image communication apparatus server apparatus and capability exchanging method |
| [WO2002008938A2 (en)](/patent/WO2002008938A2/en) | 2000-07-24 | 2002-01-31 | Vignette Corporation | Method and system for managing message pacing |
| [US6389276B1 (en)](/patent/US6389276B1/en) | 1998-12-23 | 2002-05-14 | Bell Atlantic Mobile | Systems and methods for providing voice mail notification from a separate voice mail system to mobile telephone |
| [US20020059454A1 (en)](/patent/US20020059454A1/en) | 2000-05-16 | 2002-05-16 | Barrett Joseph G. | E-mail sender identification |
| [US6404762B1 (en)](/patent/US6404762B1/en) | 1998-06-09 | 2002-06-11 | Unisys Corporation | Universal messaging system providing integrated voice, data and fax messaging services to pc/web-based clients, including a session manager for maintaining a session between a messaging platform and the web-based clients |
| [US6411684B1 (en)](/patent/US6411684B1/en) | 1994-09-16 | 2002-06-25 | Avaya Technology Corp. | Network-based multimedia communications and directory system and method of operation |
| [US6434601B1 (en)](/patent/US6434601B1/en) | 1999-03-31 | 2002-08-13 | Micron Technology, Inc. | Pre test electronic mail process |
| [US6438215B1 (en)](/patent/US6438215B1/en) | 2000-02-29 | 2002-08-20 | Ameritech Corporation | Method and system for filter based message processing in a unified messaging system |
| [US6442589B1 (en)](/patent/US6442589B1/en) | 1999-01-14 | 2002-08-27 | Fujitsu Limited | Method and system for sorting and forwarding electronic messages and other data |
| [US6453327B1 (en)](/patent/US6453327B1/en) | 1996-06-10 | 2002-09-17 | Sun Microsystems, Inc. | Method and apparatus for identifying and discarding junk electronic mail |
| [US6487586B2 (en)](/patent/US6487586B2/en) | 1998-09-23 | 2002-11-26 | John W. L. Ogilvie | Self-removing email verified or designated as such by a message distributor for the convenience of a recipient |
| [US20020199095A1 (en)](/patent/US20020199095A1/en) \* | 1997-07-24 | 2002-12-26 | Jean-Christophe Bandini | Method and system for filtering communication |
| [US6513045B1 (en)](/patent/US6513045B1/en) | 1999-11-17 | 2003-01-28 | International Business Machines Corporation | Method and an apparatus for providing cross product automated user assistance in the planning, configuration, and management of information systems |
| [US20030101181A1 (en)](/patent/US20030101181A1/en) \* | 2001-11-02 | 2003-05-29 | Khalid Al-Kofahi | Systems, Methods, and software for classifying text from judicial opinions and other documents |
| [US6574658B1 (en)](/patent/US6574658B1/en) | 1999-01-29 | 2003-06-03 | Lucent Technologies Inc. | System and method for secure classification of electronic mail |
| [US6609196B1 (en)](/patent/US6609196B1/en) | 1997-07-24 | 2003-08-19 | Tumbleweed Communications Corp. | E-mail firewall with stored key encryption/decryption |
| [US6615241B1 (en)](/patent/US6615241B1/en) \* | 1997-07-18 | 2003-09-02 | Net Exchange, Llc | Correspondent-centric management email system uses message-correspondent relationship data table for automatically linking a single stored message with its correspondents |
| [US6615258B1 (en)](/patent/US6615258B1/en) | 1997-09-26 | 2003-09-02 | Worldcom, Inc. | Integrated customer interface for web based data management |
| [US6650890B1 (en)](/patent/US6650890B1/en) | 2000-09-29 | 2003-11-18 | Postini, Inc. | Value-added electronic messaging services and transparent implementation thereof using intermediate server |
| [US6654787B1 (en)](/patent/US6654787B1/en) | 1998-12-31 | 2003-11-25 | Brightmail, Incorporated | Method and apparatus for filtering e-mail |
| [US6691156B1 (en)](/patent/US6691156B1/en) | 2000-03-10 | 2004-02-10 | International Business Machines Corporation | Method for restricting delivery of unsolicited E-mail |
| [US6711618B1 (en)](/patent/US6711618B1/en) | 1999-09-03 | 2004-03-23 | Cisco Technology, Inc. | Apparatus and method for providing server state and attribute management for voice enabled web applications |
| [US20040117648A1 (en)](/patent/US20040117648A1/en) \* | 2002-12-16 | 2004-06-17 | Kissel Timo S. | Proactive protection against e-mail worms and spam |
| [US20040128355A1 (en)](/patent/US20040128355A1/en) \* | 2002-12-25 | 2004-07-01 | Kuo-Jen Chao | Community-based message classification and self-amending system for a messaging system |
| [US6779021B1 (en)](/patent/US6779021B1/en) | 2000-07-28 | 2004-08-17 | International Business Machines Corporation | Method and system for predicting and managing undesirable electronic mail |
| [US20040267893A1 (en)](/patent/US20040267893A1/en) \* | 2003-06-30 | 2004-12-30 | Wei Lin | Fuzzy logic voting method and system for classifying E-mail using inputs from multiple spam classifiers |
| [US6868498B1 (en)](/patent/US6868498B1/en) | 1999-09-01 | 2005-03-15 | Peter L. Katsikas | System for eliminating unauthorized electronic mail |
| [US20050210116A1 (en)](/patent/US20050210116A1/en) \* | 2004-03-22 | 2005-09-22 | Samson Ronald W | Notification and summarization of E-mail messages held in SPAM quarantine |
| [US7257564B2 (en)](/patent/US7257564B2/en) \* | 2003-10-03 | 2007-08-14 | Tumbleweed Communications Corp. | Dynamic message filtering |

## Family Cites Families (4)

\* Cited by examiner, † Cited by third party

| Publication number | Priority date | Publication date | Assignee | Title |
| --- | --- | --- | --- | --- |
| [EP0569950B1 (en)](/patent/EP0569950B1/en) \* | 1992-05-11 | 1999-12-08 | Fuji Photo Film Co., Ltd. | Molded articles for photographic photosensitive materials |
| [US5937161A (en)](/patent/US5937161A/en) | 1996-04-12 | 1999-08-10 | Usa.Net, Inc. | Electronic message forwarding system |
| [CN1332333C (en)](/patent/CN1332333C/en) | 2002-02-19 | 2007-08-15 | 波斯蒂尼公司 | E-mail management services |
| [US20060265459A1 (en)](/patent/US20060265459A1/en) | 2003-02-19 | 2006-11-23 | Postini, Inc. | Systems and methods for managing the transmission of synchronous electronic messages |

* 2004
  + 2004-04-26
    US
    US10/832,407
    [patent/US7647321B2/en](/patent/US7647321B2/en)
    not\_active
    Expired - Lifetime
* 2005
  + 2005-03-29
    WO
    PCT/US2005/010276
    [patent/WO2005109234A2/en](/patent/WO2005109234A2/en)
    not\_active
    Ceased
  + 2005-03-29
    AU
    AU2005241402A
    [patent/AU2005241402B2/en](/patent/AU2005241402B2/en)
    not\_active
    Ceased
  + 2005-03-29
    EP
    EP05733019A
    [patent/EP1763789A4/en](/patent/EP1763789A4/en)
    not\_active
    Ceased
  + 2005-03-29
    CA
    CA2564232A
    [patent/CA2564232C/en](/patent/CA2564232C/en)
    not\_active
    Expired - Lifetime
  + 2005-03-29
    JP
    JP2007510738A
    [patent/JP4960222B2/en](/patent/JP4960222B2/en)
    not\_active
    Expired - Lifetime
  + 2005-03-29
    KR
    KR1020067024774A
    [patent/KR101208943B1/en](/patent/KR101208943B1/en)
    not\_active
    Expired - Lifetime
  + 2005-03-29
    CN
    CNA200580013218XA
    [patent/CN1977263A/en](/patent/CN1977263A/en)
    active
    Pending
* 2009
  + 2009-12-09
    US
    US12/634,436
    [patent/US8321432B2/en](/patent/US8321432B2/en)
    not\_active
    Expired - Fee Related

## Patent Citations (76)

\* Cited by examiner, † Cited by third party

| Publication number | Priority date | Publication date | Assignee | Title |
| --- | --- | --- | --- | --- |
| [US4837798A (en)](/patent/US4837798A/en) | 1986-06-02 | 1989-06-06 | American Telephone And Telegraph Company | Communication system having unified messaging |
| [US5627764A (en)](/patent/US5627764A/en) | 1991-10-04 | 1997-05-06 | Banyan Systems, Inc. | Automatic electronic messaging system with feedback and work flow administration |
| [US5634005A (en)](/patent/US5634005A/en) | 1992-11-09 | 1997-05-27 | Kabushiki Kaisha Toshiba | System for automatically sending mail message by storing rule according to the language specification of the message including processing condition and processing content |
| [US6411684B1 (en)](/patent/US6411684B1/en) | 1994-09-16 | 2002-06-25 | Avaya Technology Corp. | Network-based multimedia communications and directory system and method of operation |
| [US5742668A (en)](/patent/US5742668A/en) | 1994-09-19 | 1998-04-21 | Bell Communications Research, Inc. | Electronic massaging network |
| [US5619648A (en)](/patent/US5619648A/en) | 1994-11-30 | 1997-04-08 | Lucent Technologies Inc. | Message filtering techniques |
| [US5937162A (en)](/patent/US5937162A/en) | 1995-04-06 | 1999-08-10 | Exactis.Com, Inc. | Method and apparatus for high volume e-mail delivery |
| [WO1996035994A1 (en)](/patent/WO1996035994A1/en) | 1995-05-08 | 1996-11-14 | Compuserve Incorporated | Rules based electronic message management system |
| [US5889943A (en)](/patent/US5889943A/en) | 1995-09-26 | 1999-03-30 | Trend Micro Incorporated | Apparatus and method for electronic mail virus detection and elimination |
| [WO1997012321A1 (en)](/patent/WO1997012321A1/en) | 1995-09-26 | 1997-04-03 | Trend Micro, Incorporated | Virus detection and removal apparatus for computer networks |
| [US5771355A (en)](/patent/US5771355A/en) | 1995-12-21 | 1998-06-23 | Intel Corporation | Transmitting electronic mail by either reference or value at file-replication points to minimize costs |
| [WO1997027546A1 (en)](/patent/WO1997027546A1/en) | 1996-01-26 | 1997-07-31 | Ex Machina, Inc. | System and method for transmission of data |
| [US6075863A (en)](/patent/US6075863A/en) | 1996-02-28 | 2000-06-13 | Encanto Networks | Intelligent communication device |
| [US6453327B1 (en)](/patent/US6453327B1/en) | 1996-06-10 | 2002-09-17 | Sun Microsystems, Inc. | Method and apparatus for identifying and discarding junk electronic mail |
| [US6014429A (en)](/patent/US6014429A/en) | 1996-08-12 | 2000-01-11 | Lucent Technologies, Inc. | Two-way wireless messaging system with transaction server |
| [US5832208A (en)](/patent/US5832208A/en) | 1996-09-05 | 1998-11-03 | Cheyenne Software International Sales Corp. | Anti-virus agent for use with databases and mail servers |
| [US5905777A (en)](/patent/US5905777A/en) | 1996-09-27 | 1999-05-18 | At&T Corp. | E-mail paging system |
| [US6092194A (en)](/patent/US6092194A/en) | 1996-11-08 | 2000-07-18 | Finjan Software, Ltd. | System and method for protecting a computer and a network from hostile downloadables |
| [US5796948A (en)](/patent/US5796948A/en) | 1996-11-12 | 1998-08-18 | Cohen; Elliot D. | Offensive message interceptor for computers |
| [US6146026A (en)](/patent/US6146026A/en) | 1996-12-27 | 2000-11-14 | Canon Kabushiki Kaisha | System and apparatus for selectively publishing electronic-mail |
| [US5987611A (en)](/patent/US5987611A/en) | 1996-12-31 | 1999-11-16 | Zone Labs, Inc. | System and methodology for managing internet access on a per application basis for client computers connected to the internet |
| [US5844969A (en)](/patent/US5844969A/en) | 1997-01-23 | 1998-12-01 | At&T Corp. | Communication system, method and device for remotely re-transmitting received electronic mail directed to a destination terminal to a new destination terminal |
| [WO1998037680A2 (en)](/patent/WO1998037680A2/en) | 1997-02-25 | 1998-08-27 | Intervoice Limited Partnership | E-mail server for message filtering and routing |
| [US6147987A (en)](/patent/US6147987A/en) | 1997-04-08 | 2000-11-14 | 3Com Corporation | Supporting load sharing across multiple network access servers |
| [US6178331B1 (en)](/patent/US6178331B1/en) | 1997-06-17 | 2001-01-23 | Bulletin.Net, Inc. | System and process for allowing wireless messaging |
| [US6615241B1 (en)](/patent/US6615241B1/en) \* | 1997-07-18 | 2003-09-02 | Net Exchange, Llc | Correspondent-centric management email system uses message-correspondent relationship data table for automatically linking a single stored message with its correspondents |
| [US6061718A (en)](/patent/US6061718A/en) | 1997-07-23 | 2000-05-09 | Ericsson Inc. | Electronic mail delivery system in wired or wireless communications system |
| [US6609196B1 (en)](/patent/US6609196B1/en) | 1997-07-24 | 2003-08-19 | Tumbleweed Communications Corp. | E-mail firewall with stored key encryption/decryption |
| [US20020199095A1 (en)](/patent/US20020199095A1/en) \* | 1997-07-24 | 2002-12-26 | Jean-Christophe Bandini | Method and system for filtering communication |
| [US6073165A (en)](/patent/US6073165A/en) | 1997-07-29 | 2000-06-06 | Jfax Communications, Inc. | Filtering computer network messages directed to a user's e-mail box based on user defined filters, and forwarding a filtered message to the user's receiver |
| [WO1999006929A2 (en)](/patent/WO1999006929A2/en) | 1997-08-03 | 1999-02-11 | At & T Corp. | An extensible proxy framework for e-mail agents |
| [US6249805B1 (en)](/patent/US6249805B1/en) | 1997-08-12 | 2001-06-19 | Micron Electronics, Inc. | Method and system for filtering unauthorized electronic mail messages |
| [US6334140B1 (en)](/patent/US6334140B1/en) | 1997-09-25 | 2001-12-25 | Nec Corporation | Electronic mail server in which electronic mail is processed |
| [US6615258B1 (en)](/patent/US6615258B1/en) | 1997-09-26 | 2003-09-02 | Worldcom, Inc. | Integrated customer interface for web based data management |
| [US6138146A (en)](/patent/US6138146A/en) | 1997-09-29 | 2000-10-24 | Ericsson Inc. | Electronic mail forwarding system and method |
| [US6266664B1 (en)](/patent/US6266664B1/en) \* | 1997-10-01 | 2001-07-24 | Rulespace, Inc. | Method for scanning, analyzing and rating digital information content |
| [US6023723A (en)](/patent/US6023723A/en) | 1997-12-22 | 2000-02-08 | Accepted Marketing, Inc. | Method and system for filtering unwanted junk e-mail utilizing a plurality of filtering mechanisms |
| [US6052709A (en)](/patent/US6052709A/en) | 1997-12-23 | 2000-04-18 | Bright Light Technologies, Inc. | Apparatus and method for controlling delivery of unsolicited electronic mail |
| [US5999932A (en)](/patent/US5999932A/en) | 1998-01-13 | 1999-12-07 | Bright Light Technologies, Inc. | System and method for filtering unsolicited electronic mail messages using data matching and heuristic processing |
| [US5968117A (en)](/patent/US5968117A/en) | 1998-01-20 | 1999-10-19 | Aurora Communications Exchange Ltd. | Device and system to facilitate accessing electronic mail from remote user-interface devices |
| [US6263202B1 (en)](/patent/US6263202B1/en) | 1998-01-28 | 2001-07-17 | Uniden Corporation | Communication system and wireless communication terminal device used therein |
| [US6404762B1 (en)](/patent/US6404762B1/en) | 1998-06-09 | 2002-06-11 | Unisys Corporation | Universal messaging system providing integrated voice, data and fax messaging services to pc/web-based clients, including a session manager for maintaining a session between a messaging platform and the web-based clients |
| [US6301245B1 (en)](/patent/US6301245B1/en) | 1998-06-09 | 2001-10-09 | Unisys Corporation | Universal Messaging system providing integrated voice, data and fax messaging services to PC/web-based clients, including a large object server for efficiently distributing voice/fax messages to web-based clients |
| [WO1999065256A2 (en)](/patent/WO1999065256A2/en) | 1998-06-10 | 1999-12-16 | Logica, Inc. | System and method for delivering e-mail notification to mobile phones |
| [WO1999067731A1 (en)](/patent/WO1999067731A1/en) | 1998-06-23 | 1999-12-29 | Microsoft Corporation | A technique which utilizes a probabilistic classifier to detect 'junk' e-mail |
| [US6112227A (en)](/patent/US6112227A/en) | 1998-08-06 | 2000-08-29 | Heiner; Jeffrey Nelson | Filter-in method for reducing junk e-mail |
| [US6487586B2 (en)](/patent/US6487586B2/en) | 1998-09-23 | 2002-11-26 | John W. L. Ogilvie | Self-removing email verified or designated as such by a message distributor for the convenience of a recipient |
| [US6317751B1 (en)](/patent/US6317751B1/en) | 1998-09-28 | 2001-11-13 | Merrill Lynch & Co., Inc. | Compliance archival data process and system |
| [US6249807B1 (en)](/patent/US6249807B1/en) | 1998-11-17 | 2001-06-19 | Kana Communications, Inc. | Method and apparatus for performing enterprise email management |
| [US6389276B1 (en)](/patent/US6389276B1/en) | 1998-12-23 | 2002-05-14 | Bell Atlantic Mobile | Systems and methods for providing voice mail notification from a separate voice mail system to mobile telephone |
| [US6118856A (en)](/patent/US6118856A/en) | 1998-12-28 | 2000-09-12 | Nortel Networks Corporation | Method and apparatus for automatically forwarding an email message or portion thereof to a remote device |
| [US6654787B1 (en)](/patent/US6654787B1/en) | 1998-12-31 | 2003-11-25 | Brightmail, Incorporated | Method and apparatus for filtering e-mail |
| [WO2000042747A1 (en)](/patent/WO2000042747A1/en) | 1999-01-13 | 2000-07-20 | Soobok Lee | Internet e-mail add-on service system |
| [US6442589B1 (en)](/patent/US6442589B1/en) | 1999-01-14 | 2002-08-27 | Fujitsu Limited | Method and system for sorting and forwarding electronic messages and other data |
| [US6574658B1 (en)](/patent/US6574658B1/en) | 1999-01-29 | 2003-06-03 | Lucent Technologies Inc. | System and method for secure classification of electronic mail |
| [WO2000049776A1 (en)](/patent/WO2000049776A1/en) | 1999-02-17 | 2000-08-24 | Argo Interactive Limited | Method and apparatus for proxying and filtering electronic mail |
| [US6335966B1 (en)](/patent/US6335966B1/en) | 1999-03-29 | 2002-01-01 | Matsushita Graphic Communication Systems, Inc. | Image communication apparatus server apparatus and capability exchanging method |
| [US6434601B1 (en)](/patent/US6434601B1/en) | 1999-03-31 | 2002-08-13 | Micron Technology, Inc. | Pre test electronic mail process |
| [US6868498B1 (en)](/patent/US6868498B1/en) | 1999-09-01 | 2005-03-15 | Peter L. Katsikas | System for eliminating unauthorized electronic mail |
| [US6711618B1 (en)](/patent/US6711618B1/en) | 1999-09-03 | 2004-03-23 | Cisco Technology, Inc. | Apparatus and method for providing server state and attribute management for voice enabled web applications |
| [US6513045B1 (en)](/patent/US6513045B1/en) | 1999-11-17 | 2003-01-28 | International Business Machines Corporation | Method and an apparatus for providing cross product automated user assistance in the planning, configuration, and management of information systems |
| [US6321267B1 (en)](/patent/US6321267B1/en) | 1999-11-23 | 2001-11-20 | Escom Corporation | Method and apparatus for filtering junk email |
| [WO2001046867A1 (en)](/patent/WO2001046867A1/en) | 1999-12-22 | 2001-06-28 | Setnet Corp. | Industrial capacity clustered mail server system and method |
| [US20010032095A1 (en)](/patent/US20010032095A1/en) | 2000-01-14 | 2001-10-18 | Balbach Carl Teo | Context-specific contact information |
| [US6438215B1 (en)](/patent/US6438215B1/en) | 2000-02-29 | 2002-08-20 | Ameritech Corporation | Method and system for filter based message processing in a unified messaging system |
| [US6691156B1 (en)](/patent/US6691156B1/en) | 2000-03-10 | 2004-02-10 | International Business Machines Corporation | Method for restricting delivery of unsolicited E-mail |
| [US20020059454A1 (en)](/patent/US20020059454A1/en) | 2000-05-16 | 2002-05-16 | Barrett Joseph G. | E-mail sender identification |
| [WO2002008938A2 (en)](/patent/WO2002008938A2/en) | 2000-07-24 | 2002-01-31 | Vignette Corporation | Method and system for managing message pacing |
| [US6779021B1 (en)](/patent/US6779021B1/en) | 2000-07-28 | 2004-08-17 | International Business Machines Corporation | Method and system for predicting and managing undesirable electronic mail |
| [US6650890B1 (en)](/patent/US6650890B1/en) | 2000-09-29 | 2003-11-18 | Postini, Inc. | Value-added electronic messaging services and transparent implementation thereof using intermediate server |
| [US20030101181A1 (en)](/patent/US20030101181A1/en) \* | 2001-11-02 | 2003-05-29 | Khalid Al-Kofahi | Systems, Methods, and software for classifying text from judicial opinions and other documents |
| [US20040117648A1 (en)](/patent/US20040117648A1/en) \* | 2002-12-16 | 2004-06-17 | Kissel Timo S. | Proactive protection against e-mail worms and spam |
| [US20040128355A1 (en)](/patent/US20040128355A1/en) \* | 2002-12-25 | 2004-07-01 | Kuo-Jen Chao | Community-based message classification and self-amending system for a messaging system |
| [US20040267893A1 (en)](/patent/US20040267893A1/en) \* | 2003-06-30 | 2004-12-30 | Wei Lin | Fuzzy logic voting method and system for classifying E-mail using inputs from multiple spam classifiers |
| [US7257564B2 (en)](/patent/US7257564B2/en) \* | 2003-10-03 | 2007-08-14 | Tumbleweed Communications Corp. | Dynamic message filtering |
| [US20050210116A1 (en)](/patent/US20050210116A1/en) \* | 2004-03-22 | 2005-09-22 | Samson Ronald W | Notification and summarization of E-mail messages held in SPAM quarantine |

## Non-Patent Citations (32)

\* Cited by examiner, † Cited by third party

| Title |
| --- |
| "[Automated Spam Detection,](http://scholar.google.com/scholar?q="Automated+Spam+Detection%2C")" R. Lonn, Feb. 16, 1999. |
| "[MsgTo.com Stops Spam Email](http://scholar.google.com/scholar?q="MsgTo.com+Stops+Spam+Email")", web page circa Nov. 19, 1999, from www.applesforhealth.com. |
| "[The Species Filter](http://scholar.google.com/scholar?q="The+Species+Filter")", by Rafe Needleman, ed., dated Aug. 6, 1999, from www.RedHerring.com. |
| Bounce Spam Mail, from Albert Yale Software, dated 1997-2000. |
| BrightMail, from BrightMail, Inc., dated 1997-2000. |
| CSM Internet Mail Scanner, from CSM-USA, Inc., dated 1999. |
| CVS.Sourceforge.Net, "[Spam Filtering ESMTP Demon](http://scholar.google.com/scholar?q="Spam+Filtering+ESMTP+Demon")", copyright notice dated 2000, publ. at http://cvs.sourceforge.net/viewcvs.py/clocc/clocc/src/donc/smt-p. lisp?rev=1.4. |
| CyberSitter AntiSpam, from CyberSitter.com, distributed by Solid Oak Software, circa 1999-2000. |
| DL MailFilter, from DeadLetter and Leem Han Cheong, dated Nov. 1999. |
| E-Mail Chompaer, from Lorenzo Pasqualis, dated 1996-97. |
| E-Mail Remover, from Victor Javier, Virtual Network, Inc., Singapore, dated Mar.-Jul. 1998, and 1999. |
| EMC News Release, "[EMC Launches Centera, Ushers in New Era of Content-Addresses Storage,](http://scholar.google.com/scholar?q="EMC+Launches+Centera%2C+Ushers+in+New+Era+of+Content-Addresses+Storage%2C")" New York, Apr. 29, 2002. www.emc.com/news/press-releases/view.jsp?id=1254. |
| European Examination Report, EP 01977347.2 dated Aug. 26, 2005. |
| FlameThrower, from Eagle Research, Inc., dated 2000. |
| http://web.archive.org/web19990128140052/http://www.chooseyourmail.com/, Yr 1999. |
| http://web.archive.org/web20000815053401/http://www.brightmail.com/corporate/overview/, Yr 2000. |
| http://web.archive.org/web20000815064559/www.commtouch.com/solutions/index.shtml, Yr 2000. |
| http://web.archive.org/web20000816134259/www.antivirus.com/products/email-groupware.htm, Yr 2000. |
| http://web.archive.org/web20000824040241/www.messagelabs.com/about/overview/overview.htm, Yr 2000. |
| http://web.archive.org/web20001205151400/mailcircuit.com/route.htm, Yr 2000. |
| Interceptor, from Grok Development Ltd., dated 1999-2000. |
| International Search Report, Form PCT/ISA/210 dated Apr. 14, 2004, PCT Application No. PCT/US03/04757. |
| JOC E-Mail Checker, from JOCSoft and Jose Olice Civit, dated 2000. |
| Official Sep. 1999 AUP (Auto Update Program) v5.0 Build 447, Product Update Release, winserver.com. |
| PCT/US05/10276, International Search Report and Written Opinion dated Nov. 14, 2006. |
| Praetor, from Computer Mail Services, Inc., circa 1998-99. |
| Quickhead-E, from Danere Software Innovations, dated Mar. 2000. |
| Spam Attack Pro, circa 1996-97, from softwiz.com. |
| Spam Buster, from Contact Plus Corp., dated 2000. |
| SpamEater, from High Mountain Software, dated 1997-2000. |
| Supplementary European Search Report, EP 01977347 dated Apr. 7, 2005. |
| Supplementary European Search Report, EP 03711094.7 dated Sep. 6, 2005. |

## Cited By (31)

\* Cited by examiner, † Cited by third party

| Publication number | Priority date | Publication date | Assignee | Title |
| --- | --- | --- | --- | --- |
| [US8955136B2 (en)](/patent/US8955136B2/en) | 2004-07-13 | 2015-02-10 | Sonicwall, Inc. | Analyzing traffic patterns to detect infectious messages |
| [US10069851B2 (en)](/patent/US10069851B2/en) | 2004-07-13 | 2018-09-04 | Sonicwall Inc. | Managing infectious forwarded messages |
| [US9237163B2 (en)](/patent/US9237163B2/en) | 2004-07-13 | 2016-01-12 | Dell Software Inc. | Managing infectious forwarded messages |
| [US20080134336A1 (en)](/patent/US20080134336A1/en) \* | 2004-07-13 | 2008-06-05 | Mailfrontier, Inc. | Analyzing traffic patterns to detect infectious messages |
| [US9154511B1 (en)](/patent/US9154511B1/en) \* | 2004-07-13 | 2015-10-06 | Dell Software Inc. | Time zero detection of infectious messages |
| [US9516047B2 (en)](/patent/US9516047B2/en) | 2004-07-13 | 2016-12-06 | Dell Software Inc. | Time zero classification of messages |
| [US20070294765A1 (en)](/patent/US20070294765A1/en) \* | 2004-07-13 | 2007-12-20 | Sonicwall, Inc. | Managing infectious forwarded messages |
| [US8850566B2 (en)](/patent/US8850566B2/en) | 2004-07-13 | 2014-09-30 | Sonicwall, Inc. | Time zero detection of infectious messages |
| [US8955106B2 (en)](/patent/US8955106B2/en) | 2004-07-13 | 2015-02-10 | Sonicwall, Inc. | Managing infectious forwarded messages |
| [US8122508B2 (en)](/patent/US8122508B2/en) | 2004-07-13 | 2012-02-21 | Sonicwall, Inc. | Analyzing traffic patterns to detect infectious messages |
| [US20080104703A1 (en)](/patent/US20080104703A1/en) \* | 2004-07-13 | 2008-05-01 | Mailfrontier, Inc. | Time Zero Detection of Infectious Messages |
| [US10084801B2 (en)](/patent/US10084801B2/en) | 2004-07-13 | 2018-09-25 | Sonicwall Inc. | Time zero classification of messages |
| [US9325724B2 (en)](/patent/US9325724B2/en) | 2004-07-13 | 2016-04-26 | Dell Software Inc. | Time zero classification of messages |
| [US20080184366A1 (en)](/patent/US20080184366A1/en) \* | 2004-11-05 | 2008-07-31 | Secure Computing Corporation | Reputation based message processing |
| [US8635690B2 (en)](/patent/US8635690B2/en) | 2004-11-05 | 2014-01-21 | Mcafee, Inc. | Reputation based message processing |
| [US8510388B2 (en)](/patent/US8510388B2/en) \* | 2006-11-13 | 2013-08-13 | International Business Machines Corporation | Tracking messages in a mentoring environment |
| [US20080114838A1 (en)](/patent/US20080114838A1/en) \* | 2006-11-13 | 2008-05-15 | International Business Machines Corporation | Tracking messages in a mentoring environment |
| [US20120240228A1 (en)](/patent/US20120240228A1/en) \* | 2007-01-24 | 2012-09-20 | Mcafee, Inc. | Multi-dimensional reputation scoring |
| [US8763114B2 (en)](/patent/US8763114B2/en) | 2007-01-24 | 2014-06-24 | Mcafee, Inc. | Detecting image spam |
| [US8762537B2 (en)](/patent/US8762537B2/en) | 2007-01-24 | 2014-06-24 | Mcafee, Inc. | Multi-dimensional reputation scoring |
| [US10050917B2 (en)](/patent/US10050917B2/en) | 2007-01-24 | 2018-08-14 | Mcafee, Llc | Multi-dimensional reputation scoring |
| [US9009321B2 (en)](/patent/US9009321B2/en) \* | 2007-01-24 | 2015-04-14 | Mcafee, Inc. | Multi-dimensional reputation scoring |
| [US9544272B2 (en)](/patent/US9544272B2/en) | 2007-01-24 | 2017-01-10 | Intel Corporation | Detecting image spam |
| [US20080178288A1 (en)](/patent/US20080178288A1/en) \* | 2007-01-24 | 2008-07-24 | Secure Computing Corporation | Detecting Image Spam |
| [US9083712B2 (en)](/patent/US9083712B2/en) \* | 2007-04-04 | 2015-07-14 | Sri International | Method and apparatus for generating highly predictive blacklists |
| [US20090064332A1 (en)](/patent/US20090064332A1/en) \* | 2007-04-04 | 2009-03-05 | Phillip Andrew Porras | Method and apparatus for generating highly predictive blacklists |
| [US7890590B1 (en)](/patent/US7890590B1/en) \* | 2007-09-27 | 2011-02-15 | Symantec Corporation | Variable bayesian handicapping to provide adjustable error tolerance level |
| [US20090125980A1 (en)](/patent/US20090125980A1/en) \* | 2007-11-09 | 2009-05-14 | Secure Computing Corporation | Network rating |
| [US9288173B2 (en)](/patent/US9288173B2/en) | 2011-04-11 | 2016-03-15 | Microsoft Technology Licensing, Llc | Geo-data spam filter |
| [US8626856B2 (en)](/patent/US8626856B2/en) \* | 2011-04-11 | 2014-01-07 | Microsoft Corporation | Geo-data spam filter |
| [US20120259929A1 (en)](/patent/US20120259929A1/en) \* | 2011-04-11 | 2012-10-11 | Microsoft Corporation | Geo-data spam filter |

## Also Published As

| Publication number | Publication date |
| --- | --- |
| [CA2564232C (en)](/patent/CA2564232C/en) | 2015-12-01 |
| [EP1763789A4 (en)](/patent/EP1763789A4/en) | 2009-03-04 |
| [KR101208943B1 (en)](/patent/KR101208943B1/en) | 2012-12-07 |
| [EP1763789A2 (en)](/patent/EP1763789A2/en) | 2007-03-21 |
| [US20100088765A1 (en)](/patent/US20100088765A1/en) | 2010-04-08 |
| [JP4960222B2 (en)](/patent/JP4960222B2/en) | 2012-06-27 |
| [US20050240617A1 (en)](/patent/US20050240617A1/en) | 2005-10-27 |
| [CA2564232A1 (en)](/patent/CA2564232A1/en) | 2005-11-17 |
| [AU2005241402B2 (en)](/patent/AU2005241402B2/en) | 2011-04-21 |
| [KR20070054144A (en)](/patent/KR20070054144A/en) | 2007-05-28 |
| [US8321432B2 (en)](/patent/US8321432B2/en) | 2012-11-27 |
| [AU2005241402A1 (en)](/patent/AU2005241402A1/en) | 2005-11-17 |
| [JP2007535277A (en)](/patent/JP2007535277A/en) | 2007-11-29 |
| [CN1977263A (en)](/patent/CN1977263A/en) | 2007-06-06 |
| [WO2005109234A2 (en)](/patent/WO2005109234A2/en) | 2005-11-17 |
| [WO2005109234A3 (en)](/patent/WO2005109234A3/en) | 2007-01-11 |

## Similar Documents

| Publication | Publication Date | Title |
| --- | --- | --- |
| [US8321432B2 (en)](/patent/US8321432B2/en) | 2012-11-27 | System and method for filtering electronic messages using business heuristics |
| [US8583787B2 (en)](/patent/US8583787B2/en) | 2013-11-12 | Zero-minute virus and spam detection |
| [US6941348B2 (en)](/patent/US6941348B2/en) | 2005-09-06 | Systems and methods for managing the transmission of electronic messages through active message date updating |
| [US7653698B2 (en)](/patent/US7653698B2/en) | 2010-01-26 | Identifying e-mail messages from allowed senders |
| [US8364773B2 (en)](/patent/US8364773B2/en) | 2013-01-29 | E-mail authentication |
| [US8195753B2 (en)](/patent/US8195753B2/en) | 2012-06-05 | Honoring user preferences in email systems |
| [US10284597B2 (en)](/patent/US10284597B2/en) | 2019-05-07 | E-mail authentication |
| [US20060129644A1 (en)](/patent/US20060129644A1/en) | 2006-06-15 | Email filtering system and method |
| [US20060265459A1 (en)](/patent/US20060265459A1/en) | 2006-11-23 | Systems and methods for managing the transmission of synchronous electronic messages |
| [US7958187B2 (en)](/patent/US7958187B2/en) | 2011-06-07 | Systems and methods for managing directory harvest attacks via electronic messages |

## Legal Events

| Date | Code | Title | Description |
| --- | --- | --- | --- |
| 2004-04-26 | AS | Assignment | **Owner name**: POSTINI INC., CALIFORNIA  **Free format text**: ASSIGNMENT OF ASSIGNORS INTEREST;ASSIGNORS:LUND, PETER K.;PETRY, SCOTT M.;TITUS, JASON H.;REEL/FRAME:015265/0836  **Effective date**: 20040413 |
| 2009-04-30 | AS | Assignment | **Owner name**: GOOGLE INC., CALIFORNIA  **Free format text**: ASSIGNMENT OF ASSIGNORS INTEREST;ASSIGNOR:POSTINI, INC.;REEL/FRAME:022620/0513  **Effective date**: 20090325  **Owner name**: GOOGLE INC.,CALIFORNIA  **Free format text**: ASSIGNMENT OF ASSIGNORS INTEREST;ASSIGNOR:POSTINI, INC.;REEL/FRAME:022620/0513  **Effective date**: 20090325 |
| 2009-12-23 | STCF | Information on status: patent grant | **Free format text**: PATENTED CASE |
| 2013-03-18 | FPAY | Fee payment | **Year of fee payment**: 4 |
| 2017-07-12 | FPAY | Fee payment | **Year of fee payment**: 8 |
| 2017-10-02 | AS | Assignment | **Owner name**: GOOGLE LLC, CALIFORNIA  **Free format text**: CHANGE OF NAME;ASSIGNOR:GOOGLE INC.;REEL/FRAME:044101/0610  **Effective date**: 20170929 |
| 2021-07-12 | MAFP | Maintenance fee payment | **Free format text**: PAYMENT OF MAINTENANCE FEE, 12TH YEAR, LARGE ENTITY (ORIGINAL EVENT CODE: M1553); ENTITY STATUS OF PATENT OWNER: LARGE ENTITY  **Year of fee payment**: 12 |
