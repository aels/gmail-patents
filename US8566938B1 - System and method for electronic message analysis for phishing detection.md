Source: https://patents.google.com/patent/US8566938B1/en

---

# US8566938B1 - System and method for electronic message analysis for phishing detection - Google Patents

System and method for electronic message analysis for phishing detection

[Download PDF](https://patentimages.storage.googleapis.com/99/43/f1/968cd2c19d69bb/US8566938.pdf)

## Info

Publication number
:   US8566938B1

US8566938B1
US13/668,349
US201213668349A
US8566938B1
US 8566938 B1
US8566938 B1
US 8566938B1

US 201213668349 A
US201213668349 A
US 201213668349A
US 8566938 B1
US8566938 B1
US 8566938B1

Authority
:   US
:   United States

Prior art keywords
:   email
:   sender
:   recipient
:   organization
:   received

Prior art date
:   2012-11-05

Legal status (The legal status is an assumption and is not a legal conclusion. Google has not performed a legal analysis and makes no representation as to the accuracy of the status listed.)
:   Active

Application number
:   US13/668,349

Inventor
:   Gagan Prakash
:   Ravi AGARWAL

Current Assignee (The listed assignees may be inaccurate. Google has not performed a legal analysis and makes no representation or warranty as to the accuracy of the list.)
:   Vade USA Inc

Original Assignee
:   Astra Identity Inc

Priority date (The priority date is an assumption and is not a legal conclusion. Google has not performed a legal analysis and makes no representation as to the accuracy of the date listed.)
:   2012-11-05

Filing date
:   2012-11-05

Publication date
:   2013-10-22
:   2012-11-05
    Assigned to OSATECH, INC.
    reassignment
    OSATECH, INC.
    ASSIGNMENT OF ASSIGNORS INTEREST (SEE DOCUMENT FOR DETAILS).
    Assignors: AGARWAL, RAVI, PRAKASH, GAGAN
:   2012-11-05
    Priority to US13/668,349
    priority
    Critical
    patent/US8566938B1/en
:   2012-11-05
    Application filed by Astra Identity Inc
    filed
    Critical
    Astra Identity Inc
:   2012-11-05
    Assigned to OSATECH INC.
    reassignment
    OSATECH INC.
    ASSIGNMENT OF ASSIGNORS INTEREST (SEE DOCUMENT FOR DETAILS).
    Assignors: AGARWAL, RAVI, PRAKASH, GAGAN
:   2013-08-20
    Assigned to Astra Identity, Inc.
    reassignment
    Astra Identity, Inc.
    ASSIGNMENT OF ASSIGNORS INTEREST (SEE DOCUMENT FOR DETAILS).
    Assignors: OSATECH, INC.
:   2013-10-03
    Priority to US14/045,244
    priority
    patent/US9154514B1/en
:   2013-10-22
    Publication of US8566938B1
    publication
    Critical
    patent/US8566938B1/en
:   2013-10-22
    Application granted
    granted
    Critical
:   2015-09-24
    Priority to US14/864,656
    priority
    patent/US9501746B2/en
:   2018-04-17
    Assigned to VADE SDECURE SAS
    reassignment
    VADE SDECURE SAS
    ASSIGNMENT OF ASSIGNORS INTEREST (SEE DOCUMENT FOR DETAILS).
    Assignors: Astra Identity, Inc.
:   2018-06-07
    Assigned to VADE SECURE SAS
    reassignment
    VADE SECURE SAS
    CORRECTIVE ASSIGNMENT TO CORRECT THE ASSIGNEE NAME PREVIOUSLY RECORDED AT REEL: 045780 FRAME: 0001. ASSIGNOR(S) HEREBY CONFIRMS THE ASSIGNMENT.
    Assignors: Astra Identity, Inc.
:   2022-03-03
    Assigned to VADE USA, INCORPORATED
    reassignment
    VADE USA, INCORPORATED
    CHANGE OF NAME (SEE DOCUMENT FOR DETAILS).
    Assignors: VADE SECURE, INCORPORATED
:   Status
    Active
    legal-status
    Critical
    Current
:   2032-11-05
    Anticipated expiration
    legal-status
    Critical

## Links

* [USPTO](https://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO1&Sect2=HITOFF&p=1&u=/netahtml/PTO/srchnum.html&r=1&f=G&l=50&d=PALL&s1=8566938.PN.)
* [USPTO PatentCenter](https://patentcenter.uspto.gov/applications/13668349)
* [USPTO Assignment](https://assignment.uspto.gov/patent/index.html#/patent/search/resultFilter?searchInput=8566938)
* [Espacenet](https://worldwide.espacenet.com/publicationDetails/biblio?CC=US&NR=8566938B1&KC=B1&FT=D)
* [Global Dossier](https://globaldossier.uspto.gov/result/application/US/13668349/1)
* [Discuss](https://patents.stackexchange.com/questions/tagged/US8566938)

## Images

* ![](https://patentimages.storage.googleapis.com/5e/dd/b0/28b192ee564999/US08566938-20131022-D00000.png)
* ![](https://patentimages.storage.googleapis.com/9c/dd/44/965ed18e291f1c/US08566938-20131022-D00001.png)
* ![](https://patentimages.storage.googleapis.com/d3/1e/b0/8ba3c86a0d48ca/US08566938-20131022-D00002.png)
* ![](https://patentimages.storage.googleapis.com/d4/86/43/80b24e5713d232/US08566938-20131022-D00003.png)

## Classifications

* + H—ELECTRICITY
  + H04—ELECTRIC COMMUNICATION TECHNIQUE
  + H04L—TRANSMISSION OF DIGITAL INFORMATION, e.g. TELEGRAPHIC COMMUNICATION
  + H04L63/00—Network architectures or network communication protocols for network security
  + H04L63/14—Network architectures or network communication protocols for network security for detecting or protecting against malicious traffic
  + H04L63/1441—Countermeasures against malicious traffic
  + H04L63/1483—Countermeasures against malicious traffic service impersonation, e.g. phishing, pharming or web spoofing
* + G—PHYSICS
  + G06—COMPUTING OR CALCULATING; COUNTING
  + G06Q—INFORMATION AND COMMUNICATION TECHNOLOGY [ICT] SPECIALLY ADAPTED FOR ADMINISTRATIVE, COMMERCIAL, FINANCIAL, MANAGERIAL OR SUPERVISORY PURPOSES; SYSTEMS OR METHODS SPECIALLY ADAPTED FOR ADMINISTRATIVE, COMMERCIAL, FINANCIAL, MANAGERIAL OR SUPERVISORY PURPOSES, NOT OTHERWISE PROVIDED FOR
  + G06Q10/00—Administration; Management
  + G06Q10/10—Office automation; Time management
  + G06Q10/107—Computer-aided management of electronic mailing [e-mailing]
* + H—ELECTRICITY
  + H04—ELECTRIC COMMUNICATION TECHNIQUE
  + H04L—TRANSMISSION OF DIGITAL INFORMATION, e.g. TELEGRAPHIC COMMUNICATION
  + H04L51/00—User-to-user messaging in packet-switching networks, transmitted according to store-and-forward or real-time protocols, e.g. e-mail
  + H04L51/21—Monitoring or handling of messages
  + H04L51/212—Monitoring or handling of messages using filtering or selective blocking

## Definitions

* fake emails
  contain links that when followed takes the user to a website, which may install malware on the recipient's computer or pose as a familiar website and ask for confidential information, such as login credentials and/or account numbers.
* Perpetrators
  may also use a compromised computer as the launch point to further penetrate the organization's computer network to access data stored on other computers, servers, and devices. Phishers may also delete and change information or even damage physical systems controlled by computers.
* Existing solutions
  are based on checking IP address associated with the phishing email or checking the text of an email for an URL to detect whether the email is a phishing email. Further, existing solutions are not integrated into email servers and clients and therefore, are restricted to some minimal checks to detect phishing activities. These techniques seem to work only when phishers use IP addresses or URLs that are suspected to be malevolent and therefore, they are typically, not robust enough to prevent sophisticated phishing attacks.
* a system and method for analyzing electronic messages for phishing detection
  are disclosed.
* the method
  includes obtaining email characteristics by parsing a received email message by a recipient/recipient organization based on a set of predetermined email characteristics.
* the email characteristics of the received email message
  are then compared with email characteristics associated with the recipient/recipient organization and/or the sender/sender organization.
* the received email message by the recipient/recipient organization
  is then declared as a phishing electronic message based on the outcome of the comparison.
* a system
  in yet another embodiment, includes an anti-phishing server and the anti-phishing server includes a processor and memory and wherein the memory includes an anti-phishing module, wherein the anti-phishing module comprises an import module, an analysis and data warehouse module, a mail handler module, an organizational analysis module, an outbound mail relay module, a configuration and management module that are configured to receive an email message by one or more recipients/recipient's organizations from one or more senders/sender's organizations via the mail handler module. Further configured to obtain email characteristics by parsing the received email message based on a set of predetermined email characteristics by the analysis and data warehouse module.
* FIG. 1
  illustrates an exemplary block diagram of a system for analyzing electronic messages for phishing detection
* FIG. 2
  illustrates a flow diagram of an exemplary method for analyzing electronic messages for phishing detection, such as those shown in FIG. 1 .
* FIG. 3
  illustrates another flow diagram of an exemplary method for analyzing electronic messages for phishing detection, such as those shown in FIG. 1 .
* FIG. 1
  illustrates an exemplary block diagram of a system 100 for analyzing electronic messages for phishing detection.
* the system 100
  includes a recipient organization mail server 110 and its associated organization computer system administrator/organization users 190 , one or more recipient email clients 130 , such as desktop software, server software, mobile device software or internet browser based software such as Microsoft Outlook, Gmail and so on 130 and its associated recipients 132 , and one or more sender's email clients 140 and their associated senders 141 that are coupled to one or more anti-phishing servers 150 via Internet/Intranet 120 .
* the one or more anti-phishing servers 150
  are coupled to a database 180 .
* FIG. 1
  illustrates an exemplary block diagram of a system 100 for analyzing electronic messages for phishing detection.
* the system 100
  includes a recipient organization mail server 110 and its associated organization computer system administrator/organization users 190 , one or more recipient email clients 130 , such as desktop software, server software, mobile device software or internet browser based software such as Microsoft Outlook, Gmail and so on 130 and
* each of the one or more recipient's email client 130
  includes an email client plugin module 131 .
* memory 160 in each anti-phishing server 150
  includes an anti-phishing module 170 .
* the anti-phishing module 170
  includes an import module 171 , an analysis and data warehouse module 172 , mail handler module 173 , an organizational analysis module 174 , an outbound mail relay module, and a configuration and management module 176 .
* the one or more recipients/recipient organization
  receives an email message from one or more senders/sender's organization via the mail handler module 173 .
* the analysis and data warehouse module
  then obtain email characteristics by parsing the received email message based on a set of predetermined email characteristics.
* Exemplary email characteristics
  are network path used to reach a recipient/recipient organization, geography associated with IP address, email client software used by the sender/sender organization, email client software version used by the sender/sender organization, date, day of week, time, time period of the email, time zone of the sender/sender organization, presence and details of digital signatures in the email, meta data present in header portion of the email, character set used in content of the email, format of the email, email length and subject length, character case of the email, character case of the subject, style of introduction at the top of the email, style and content of the sender/sender organization's signature in the body of the email, other recipient's included in the email, to, and copy circulated (cc'd) email addresses, senders name, sender's from and reply to email address, sender's organization name, senders domain name, sender's organization's Domain Name Service (DNS) settings including SPF records, sender organization's mail server information, including server ip address, sender server network path,
* emails received by the recipient/recipient organization over a predetermined time interval
  are imported by the import module 171 on its own or optionally via the email client plugin module 131 .
* the analysis and data warehouse module 172
  then parses the recipient/recipient organization's received emails based on the set of predetermined email characteristics to obtain email characteristics of the imported emails.
* the analysis and data warehouse module 172
  then stores the obtained email characteristics associated with recipient/recipient organization and sender/sender organization in the database 180 .
* the configuration and management module
  is configured to allow an administrator to select desired email characteristics to be included in the set of characteristics used for comparing the characteristics of the received email message and to assign or change a weight of how much each characteristic should influence the likelihood that a new message is a phishing message.
* the analysis and data warehouse module 172
  compares email characteristics of the received email message with email characteristics associated with the recipient/recipient organization and/or from that sender/sender organization by the analysis and data warehouse module. In some embodiments, the analysis and data warehouse module 172 obtains a statistical distribution of each of the stored email characteristics associated with the recipient/recipient organization for a sender/sender organization. The analysis and data warehouse module 172 then compares the email characteristics of the received email message with statistical distribution of each email characteristics associated with the recipient/recipient organization for that sender/sender organization.
* the analysis and data warehouse module 172
  then scores and declares the received email message by the recipient/recipient organization as a phishing electronic message based on the outcome of the comparison.
* the analysis and data warehouse module 172
  determines degree of variance of each email characteristic when compared with the associated statistical distribution. The analysis and data warehouse module 172 then establishes a score based on the determined degree of variance for each email characteristic, wherein the analysis and data warehouse module 172 assigns weights for each established score based on the determined degree of variance. The analysis and data warehouse module 172 then obtains a combined score by adding scores of all the email characteristics in the received email based on the assigned weights.
* the analysis and data warehouse module 172
  stores logs of received emails and any associated phishing activity along with details of why the email was determined to be a phishing email in the database.
* the configuration and management module 176
  then outputs logs of received emails and any associated phishing activity for viewing on a display device.
* the mail handler module 173
  quarantines emails determined to be phishing emails.
* the configuration and management module 176
  then outputs quarantined emails for viewing on a display device or forwards these emails to certain users or adds certain text to the header or subject of the email to mark them as suspect.
* either the email client plugin module 131 or the outbound mail relay module 175
  parses outbound emails sent by the recipient/recipient organization based on a set of predetermined outbound email characteristics to determine if the outbound email is a response or forward of a previously received email by the recipient/recipient organization.
* the analysis and data warehouse module 172
  updates email characteristics of the previously received emails based on the above determination to determine that the characteristics of previously received email are more likely to represent a legitimate sender/sender organization.
* the analysis and data warehouse module 172
  compares ongoing emails received from the sender/sender organizations with email characteristics, and wherein the analysis and data warehouse module scores and declares any of the ongoing emails received from sender/sender organizations as phishing based on the outcome of the comparison.
* either the mail handler module 173 or the email client plugin module 131
  includes visual identifications and reasoning information to the received email based on the outcome of the comparison to assist the recipient/recipient organization of the nature of the received email.
* either the email client plugin module 131 or the configuration and management module 176
  obtains contact and background information from the email recipient/recipient organizations' online social networks.
* the analysis and data warehouse module 172
  then stores the contact and background information in the database.
* the analysis and data ware house module 172
  upon receiving an email, determines whether the contact and background information in the received email is statistically matches the stored contact and background information in the database 180 .
* the analysis and data warehouse module 172
  then scores and declares the received email as a phishing email based on the outcome of the determination.
* the organization analysis data warehouse module 172
  determines coordinated phishing attacks against an organization by spotting phishing attacks having similar characteristics against multiple users in the organization.
* the organization analysis module 174
  monitors changing patterns of outbound emails to determine whether an organization's email client has been compromised and the sender/sender organization is sending a phishing email.
* either the email client plugin module 131 or the configuration and management module 176
  allows users to specify an email as a phishing attempt or a legitimate email and use the characteristics of this flagged email to filter messages to other users in the organization.
* FIG. 2
  a flow diagram 200 for carrying out analysis of electronic messages for phishing detection will be described.
* emails received by the recipient/recipient organization over a predetermined time interval
  are imported.
* email characteristics of the imported emails
  are obtained by parsing the recipient's/recipient organization's received emails based on the set of predetermined email characteristics.
* Exemplary email characteristics
  are network path used to reach a recipient/recipient organization, geography associated with IP address, email client software used by the sender/sender organization, email client software version used by the sender/sender organization, date, day of week, time, time period of the email, time zone of the sender/sender organization, presence and details of digital signatures in the email, meta data present in header portion of the email, character set used in content of the email, format of the email, email length and subject length, character case of the email, character case of the subject, style of introduction at the top of the email, style and content of the sender/sender organization's signature in the body of the email, other recipients/recipient organizations included in the email, to, and copy circulated (cc'd) email addresses, senders name, senders from and reply to email address, senders organization name, senders domain name, sender
* the obtained email characteristics associated with the recipient's/recipient's organization's and the sender's/sender organization's received emails
  are stored in a database.
* an email message
  is received from a sender/sender organization for a recipient/recipient organization.
* email characteristics
  are obtained by parsing the received email message based on a set of predetermined email characteristics.
* the email characteristics of the received email message
  is compared with the email characteristics associated with the recipient/recipient organization, and/or the sender/sender organization.
* an administrator
  is allowed to select desired email characteristics to be included in the set of characteristics used for comparing the characteristics of the received email message and to assign a weight of how much each characteristic should influence the likelihood that a new message is a phishing message.
* a statistical distribution of each of the stored email characteristics associated with the recipient/recipient organization and sender/sender organization
  is obtained.
* the email characteristics of the received email message
  are then compared with the obtained statistical distribution of prior email characteristics associated with the recipient/recipient organization and/or sender/sender organization.
* email determined as phishing emails
  are flagged and may be stored for subsequent analysis in determining phishing characteristics of a received email.
* the received email message by the recipient/recipient organization
  is then declared as a phishing electronic message based on the outcome of the comparison.
* degree of variance of each email characteristic when compared with the associated statistical distribution
  is determined.
* a score based on the determined degree of variance
  is then established for each email characteristic.
* weights for each established score
  is assigned based on the determined degree of variance.
* a combined score
  is then obtained by adding scores of all the email characteristics in the received email based on the assigned weights.
* logs of received emails and any associated phishing activity along with details of why the email was determined to be a phishing email
  is stored in the database.
* logs of received emails and any associated phishing activity
  are outputted for viewing on a display device.
* emails determined to be phishing emails
  are quarantined.
* the quarantined emails
  are then outputted for viewing on a display device.
* outbound emails sent by the recipient/recipient organization
  are parsed based on a set of predetermined outbound email characteristics to determine if the outbound email is a response or forward of a previously received email by the recipient/recipient organization.
* the database
  is then updated to indicate that the characteristics of the previously received email are more likely to represent a legitimate sender/sender organization.
* Any ongoing emails received from the sender/sender organization
  are then compared with stored email characteristics. Based on the outcome of the comparison, any of the ongoing emails received from the sender/sender organization are then declared as phishing emails.
* visual identifications and reasoning information on why the received email may be a phishing email
  are included based on the outcome of the comparison to assist the recipient/recipient organization of the nature of the received email.
* contact and background information associated with the email recipient/recipient organizations
  are obtained from recipient/recipient organization's Internet/online social networks.
* the contact and background information
  is then stored in the database.
* correctness of the contact and background information in the received email
  is determined using the stored contact and background information and is used as a factor in determining if the email is a phishing attempt.
* coordinated phishing attacks against an organization
  are determined by spotting phishing attacks having similar characteristics against multiple users in the organization.
* changing patterns of outbound emails
  are monitored to determine whether an email client has been compromised and the sender/sender organization is sending a phishing email.
* users
  are allowed to specify an email as a phishing attempt and use the characteristics of this flagged email to filter messages to other users in the organization.
* outbound emails sent by the recipient/recipient organization
  are parsed based on a set of predetermined outbound email characteristics to determine if the outbound email is a response or forward of a previously received email by the recipient/recipient organization.
* database
  is updated to reflect that the characteristics of the original/previous email that this new email is a reply or forward to most likely represent a legitimate sender/sender organization.
* ongoing emails received from that sender/sender organization
  are compared with stored email characteristics.
* any of the ongoing emails received from sender/sender organizations
  are declared as phishing based on the outcome of the comparison.
* system and method described in FIGS. 1-3
  propose techniques for carrying out analysis of electronic message for phishing detection.
* the technique
  enables to the addition of an indicator to emails to visually indicate to users that an email may be a phishing attempt. Additionally, the technique notifies an organization's computer system administrators regarding any synchronized attacks targeting multiple of their users by identifying any found patterns in incoming emails. Furthermore, the technique alerts an organization's computer system administrators about any possible security compromises that may result in phishing attacks within the organization. In addition, the technique assists in determining any coordinated phishing attacks against an organization by determining phishing attacks with similar characteristics against multiple users of that organization.
* the technique
  uses an outbound email reply as a trust factor for the sender/sender organization of the original email in determining the phishing nature of a received email from the sender/sender organization. Also, the above technique uses changing patterns of outbound emails to help determine whether an email client has been compromised and a sender/sender organization is sending any phishing email. Moreover, the above technique allows users to specify an email as a phishing attempt or a legitimate email and use the characteristics of the flagged email to filter messages to other uses at that organization.

## Landscapes

* Engineering & Computer Science
  (AREA)
* Business, Economics & Management
  (AREA)
* Human Resources & Organizations
  (AREA)
* Computer Security & Cryptography
  (AREA)
* Computer Networks & Wireless Communication
  (AREA)
* Signal Processing
  (AREA)
* Computer Hardware Design
  (AREA)
* Entrepreneurship & Innovation
  (AREA)
* Strategic Management
  (AREA)
* Marketing
  (AREA)
* Economics
  (AREA)
* Operations Research
  (AREA)
* Quality & Reliability
  (AREA)
* Tourism & Hospitality
  (AREA)
* Physics & Mathematics
  (AREA)
* General Business, Economics & Management
  (AREA)
* General Physics & Mathematics
  (AREA)
* Theoretical Computer Science
  (AREA)
* Data Mining & Analysis
  (AREA)
* Computing Systems
  (AREA)
* General Engineering & Computer Science
  (AREA)
* Information Transfer Between Computers
  (AREA)

## Abstract

A system and method for analyzing electronic messages for phishing detection are disclosed. In one example, email characteristics are obtained by parsing a received email message from a sender/sender organization to a recipient/recipient organization based on a set of predetermined email characteristics; the email characteristics of the received email message are then compared with email characteristics associated with the recipient/recipient organization and/or the sender/sender organization, and the received email message is then declared as a phishing electronic message based on the outcome of the comparison.

## Description

BACKGROUND

Existing email protocols on the Internet do not validate the identity of the sender of an email. As a result, bad actors impersonate other people's identity in order to increase the likelihood of recipients opening their messages and attachments. This activity is generally referred to as “phishing” and specifically “spear phishing” when the recipient is targeted by the fake sender who is referred to as a “phisher”. By getting recipients to open these fake emails, the phishers can increase their likelihood of successfully gaining unauthorized access to confidential data, including trade secrets, state secrets, military information, and other information for a variety of motivations, especially for financial gain through fraud, identity theft and/or data theft. The senders typically target and attack multiple users at a specific organization with impersonated emails in order to gain unauthorized access to their confidential data. Once a recipient opens the fake email and sometimes the attachments, the user's computer may be infected and will be used to send out phishing emails on behalf of the phisher. Some fake emails contain links that when followed takes the user to a website, which may install malware on the recipient's computer or pose as a familiar website and ask for confidential information, such as login credentials and/or account numbers. Perpetrators may also use a compromised computer as the launch point to further penetrate the organization's computer network to access data stored on other computers, servers, and devices. Phishers may also delete and change information or even damage physical systems controlled by computers.

Existing solutions are based on checking IP address associated with the phishing email or checking the text of an email for an URL to detect whether the email is a phishing email. Further, existing solutions are not integrated into email servers and clients and therefore, are restricted to some minimal checks to detect phishing activities. These techniques seem to work only when phishers use IP addresses or URLs that are suspected to be malevolent and therefore, they are typically, not robust enough to prevent sophisticated phishing attacks.

SUMMARY

A system and method for analyzing electronic messages for phishing detection are disclosed. In one embodiment, the method includes obtaining email characteristics by parsing a received email message by a recipient/recipient organization based on a set of predetermined email characteristics. The email characteristics of the received email message are then compared with email characteristics associated with the recipient/recipient organization and/or the sender/sender organization. The received email message by the recipient/recipient organization is then declared as a phishing electronic message based on the outcome of the comparison.

In yet another embodiment, a system is disclosed. The system includes an anti-phishing server and the anti-phishing server includes a processor and memory and wherein the memory includes an anti-phishing module, wherein the anti-phishing module comprises an import module, an analysis and data warehouse module, a mail handler module, an organizational analysis module, an outbound mail relay module, a configuration and management module that are configured to receive an email message by one or more recipients/recipient's organizations from one or more senders/sender's organizations via the mail handler module. Further configured to obtain email characteristics by parsing the received email message based on a set of predetermined email characteristics by the analysis and data warehouse module. Further configured to compare the email characteristics of the received email message with email characteristics associated with the recipient/recipient organization and/or the sender/sender organization by the analysis and data warehouse module. Further configured to declare the received email message by the recipient/recipient organization as a phishing electronic message based on the outcome of the comparison by the analysis and data warehouse module.

BRIEF DESCRIPTION OF THE DRAWINGS

Examples of the invention will now be described in detail with reference to the accompanying drawings, in which:

FIG. 1 illustrates an exemplary block diagram of a system for analyzing electronic messages for phishing detection;

FIG. 2 illustrates a flow diagram of an exemplary method for analyzing electronic messages for phishing detection, such as those shown in FIG. 1.

FIG. 3 illustrates another flow diagram of an exemplary method for analyzing electronic messages for phishing detection, such as those shown in FIG. 1.

The drawings described herein are for illustration purposes only and are not intended to limit the scope of the present disclosure in any way.

DETAILED DESCRIPTION

A system and method for analyzing electronic messages for phishing detection are disclosed. In the following detailed description of the examples of the present subject matter, references are made to the accompanying drawings that form a part hereof, and in which are shown by way of illustration specific examples in which the present subject matter may be practiced. These examples are described in sufficient detail to enable those skilled in the art to practice the present subject matter, and it is to be understood that other examples may be utilized and that changes may be made without departing from the scope of the present subject matter. The following detailed description is, therefore, not to be taken in a limiting sense, and the scope of the present subject matter is defined by the appended claims.

The terms “electronic message” and “email” are used interchangeably throughout the document. Further, the term “phishing” is also referred to as “spear phishing” in the document.

FIG. 1 illustrates an exemplary block diagram of a system **100** for analyzing electronic messages for phishing detection. As shown in FIG. 1, the system **100** includes a recipient organization mail server **110** and its associated organization computer system administrator/organization users **190**, one or more recipient email clients **130**, such as desktop software, server software, mobile device software or internet browser based software such as Microsoft Outlook, Gmail and so on **130** and its associated recipients **132**, and one or more sender's email clients **140** and their associated senders **141** that are coupled to one or more anti-phishing servers **150** via Internet/Intranet **120**. Further as shown in FIG. 1, the one or more anti-phishing servers **150** are coupled to a database **180**. Furthermore as shown in FIG. 1, the each of the one or more recipient's email client **130** includes an email client plugin module **131**. In addition as shown in FIG. 1, memory **160** in each anti-phishing server **150** includes an anti-phishing module **170**. The anti-phishing module **170** includes an import module **171**, an analysis and data warehouse module **172**, mail handler module **173**, an organizational analysis module **174**, an outbound mail relay module, and a configuration and management module **176**.

Now, the operation of the system **100** will be described. The one or more recipients/recipient organization receives an email message from one or more senders/sender's organization via the mail handler module **173**. The analysis and data warehouse module then obtain email characteristics by parsing the received email message based on a set of predetermined email characteristics.

Exemplary email characteristics are network path used to reach a recipient/recipient organization, geography associated with IP address, email client software used by the sender/sender organization, email client software version used by the sender/sender organization, date, day of week, time, time period of the email, time zone of the sender/sender organization, presence and details of digital signatures in the email, meta data present in header portion of the email, character set used in content of the email, format of the email, email length and subject length, character case of the email, character case of the subject, style of introduction at the top of the email, style and content of the sender/sender organization's signature in the body of the email, other recipient's included in the email, to, and copy circulated (cc'd) email addresses, senders name, sender's from and reply to email address, sender's organization name, senders domain name, sender's organization's Domain Name Service (DNS) settings including SPF records, sender organization's mail server information, including server ip address, sender server network path, sender email server software and software version, DKIM signature, spam scoring from spam software, message ID, volume of email sent by the sender, volume of email sent by sender's organization, volume of email received by the recipient, volume of email received by recipient organization, details associated with URLs or attachments in the email, whether the recipient/recipient organization has responded to this specific email, and number of interactions between sender/sender organization and recipient associated with the email and the like.

Further, in operation, emails received by the recipient/recipient organization over a predetermined time interval are imported by the import module **171** on its own or optionally via the email client plugin module **131**. The analysis and data warehouse module **172** then parses the recipient/recipient organization's received emails based on the set of predetermined email characteristics to obtain email characteristics of the imported emails. The analysis and data warehouse module **172** then stores the obtained email characteristics associated with recipient/recipient organization and sender/sender organization in the database **180**.

Furthermore, in operation, the configuration and management module is configured to allow an administrator to select desired email characteristics to be included in the set of characteristics used for comparing the characteristics of the received email message and to assign or change a weight of how much each characteristic should influence the likelihood that a new message is a phishing message.

Now, during operation, the analysis and data warehouse module **172** compares email characteristics of the received email message with email characteristics associated with the recipient/recipient organization and/or from that sender/sender organization by the analysis and data warehouse module. In some embodiments, the analysis and data warehouse module **172** obtains a statistical distribution of each of the stored email characteristics associated with the recipient/recipient organization for a sender/sender organization. The analysis and data warehouse module **172** then compares the email characteristics of the received email message with statistical distribution of each email characteristics associated with the recipient/recipient organization for that sender/sender organization.

The analysis and data warehouse module **172** then scores and declares the received email message by the recipient/recipient organization as a phishing electronic message based on the outcome of the comparison.

In some embodiments, the analysis and data warehouse module **172** determines degree of variance of each email characteristic when compared with the associated statistical distribution. The analysis and data warehouse module **172** then establishes a score based on the determined degree of variance for each email characteristic, wherein the analysis and data warehouse module **172** assigns weights for each established score based on the determined degree of variance. The analysis and data warehouse module **172** then obtains a combined score by adding scores of all the email characteristics in the received email based on the assigned weights.

In some embodiments, the analysis and data warehouse module **172** stores logs of received emails and any associated phishing activity along with details of why the email was determined to be a phishing email in the database. The configuration and management module **176** then outputs logs of received emails and any associated phishing activity for viewing on a display device.

In some embodiments, the mail handler module **173** quarantines emails determined to be phishing emails. In these embodiments, the configuration and management module **176** then outputs quarantined emails for viewing on a display device or forwards these emails to certain users or adds certain text to the header or subject of the email to mark them as suspect.

In some embodiments, either the email client plugin module **131** or the outbound mail relay module **175** parses outbound emails sent by the recipient/recipient organization based on a set of predetermined outbound email characteristics to determine if the outbound email is a response or forward of a previously received email by the recipient/recipient organization. The analysis and data warehouse module **172** then updates email characteristics of the previously received emails based on the above determination to determine that the characteristics of previously received email are more likely to represent a legitimate sender/sender organization. The analysis and data warehouse module **172** then compares ongoing emails received from the sender/sender organizations with email characteristics, and wherein the analysis and data warehouse module scores and declares any of the ongoing emails received from sender/sender organizations as phishing based on the outcome of the comparison.

In some embodiments, either the mail handler module **173** or the email client plugin module **131** includes visual identifications and reasoning information to the received email based on the outcome of the comparison to assist the recipient/recipient organization of the nature of the received email.

In some embodiments, either the email client plugin module **131** or the configuration and management module **176** obtains contact and background information from the email recipient/recipient organizations' online social networks. The analysis and data warehouse module **172** then stores the contact and background information in the database. The analysis and data ware house module **172**, upon receiving an email, determines whether the contact and background information in the received email is statistically matches the stored contact and background information in the database **180**. The analysis and data warehouse module **172** then scores and declares the received email as a phishing email based on the outcome of the determination.

In some embodiments, the organization analysis data warehouse module **172** determines coordinated phishing attacks against an organization by spotting phishing attacks having similar characteristics against multiple users in the organization. In some embodiments, the organization analysis module **174** monitors changing patterns of outbound emails to determine whether an organization's email client has been compromised and the sender/sender organization is sending a phishing email. In some embodiments, either the email client plugin module **131** or the configuration and management module **176** allows users to specify an email as a phishing attempt or a legitimate email and use the characteristics of this flagged email to filter messages to other users in the organization.

Now, referring to FIG. 2, a flow diagram **200** for carrying out analysis of electronic messages for phishing detection will be described. At block **210**, emails received by the recipient/recipient organization over a predetermined time interval are imported.

At block **220**, email characteristics of the imported emails are obtained by parsing the recipient's/recipient organization's received emails based on the set of predetermined email characteristics. Exemplary email characteristics are network path used to reach a recipient/recipient organization, geography associated with IP address, email client software used by the sender/sender organization, email client software version used by the sender/sender organization, date, day of week, time, time period of the email, time zone of the sender/sender organization, presence and details of digital signatures in the email, meta data present in header portion of the email, character set used in content of the email, format of the email, email length and subject length, character case of the email, character case of the subject, style of introduction at the top of the email, style and content of the sender/sender organization's signature in the body of the email, other recipients/recipient organizations included in the email, to, and copy circulated (cc'd) email addresses, senders name, senders from and reply to email address, senders organization name, senders domain name, sender's organization's Domain Name Service (DNS) settings including SPF records, sender organization's mail server information, including server ip address, sender server network path, sender email server software and software version, DKIM signature, spam scoring from spam software, message ID, volume of email sent by the sender, volume of email sent by sender's organization, volume of email received by the recipient, volume of email received by recipient organization, details associated with URLs or attachments in the email, whether the recipient/recipient organization has responded to this specific email, and number of interactions between sender and recipient associated with the email and the like.

At block **230**, the obtained email characteristics associated with the recipient's/recipient's organization's and the sender's/sender organization's received emails are stored in a database. At block **240**, an email message is received from a sender/sender organization for a recipient/recipient organization. At block **250**, email characteristics are obtained by parsing the received email message based on a set of predetermined email characteristics.

At block **260**, the email characteristics of the received email message is compared with the email characteristics associated with the recipient/recipient organization, and/or the sender/sender organization. In some embodiments, an administrator is allowed to select desired email characteristics to be included in the set of characteristics used for comparing the characteristics of the received email message and to assign a weight of how much each characteristic should influence the likelihood that a new message is a phishing message. Further in some embodiments, a statistical distribution of each of the stored email characteristics associated with the recipient/recipient organization and sender/sender organization is obtained. The email characteristics of the received email message are then compared with the obtained statistical distribution of prior email characteristics associated with the recipient/recipient organization and/or sender/sender organization. In some embodiments, email determined as phishing emails are flagged and may be stored for subsequent analysis in determining phishing characteristics of a received email.

At block **270**, the received email message by the recipient/recipient organization is then declared as a phishing electronic message based on the outcome of the comparison.

In some embodiments, degree of variance of each email characteristic when compared with the associated statistical distribution is determined. A score based on the determined degree of variance is then established for each email characteristic. Then weights for each established score is assigned based on the determined degree of variance. A combined score is then obtained by adding scores of all the email characteristics in the received email based on the assigned weights.

In some embodiments, logs of received emails and any associated phishing activity along with details of why the email was determined to be a phishing email is stored in the database. In these embodiments, logs of received emails and any associated phishing activity are outputted for viewing on a display device.

In some embodiments, emails determined to be phishing emails are quarantined. The quarantined emails are then outputted for viewing on a display device.

In some embodiments, outbound emails sent by the recipient/recipient organization are parsed based on a set of predetermined outbound email characteristics to determine if the outbound email is a response or forward of a previously received email by the recipient/recipient organization. The database is then updated to indicate that the characteristics of the previously received email are more likely to represent a legitimate sender/sender organization. Any ongoing emails received from the sender/sender organization are then compared with stored email characteristics. Based on the outcome of the comparison, any of the ongoing emails received from the sender/sender organization are then declared as phishing emails.

In some embodiments, visual identifications and reasoning information on why the received email may be a phishing email are included based on the outcome of the comparison to assist the recipient/recipient organization of the nature of the received email.

In some embodiments, contact and background information associated with the email recipient/recipient organizations are obtained from recipient/recipient organization's Internet/online social networks. The contact and background information is then stored in the database. Upon receiving an email, correctness of the contact and background information in the received email is determined using the stored contact and background information and is used as a factor in determining if the email is a phishing attempt.

In some embodiments, coordinated phishing attacks against an organization are determined by spotting phishing attacks having similar characteristics against multiple users in the organization. In some embodiments, changing patterns of outbound emails are monitored to determine whether an email client has been compromised and the sender/sender organization is sending a phishing email. In some embodiments, users are allowed to specify an email as a phishing attempt and use the characteristics of this flagged email to filter messages to other users in the organization.

Now, referring to FIG. 3, another flow diagram **300** for carrying out analysis of electronic messages for phishing detection will be described. At block **310**, outbound emails sent by the recipient/recipient organization are parsed based on a set of predetermined outbound email characteristics to determine if the outbound email is a response or forward of a previously received email by the recipient/recipient organization. At block **320**, database is updated to reflect that the characteristics of the original/previous email that this new email is a reply or forward to most likely represent a legitimate sender/sender organization. At block **330**, ongoing emails received from that sender/sender organization are compared with stored email characteristics. At block **340**, any of the ongoing emails received from sender/sender organizations are declared as phishing based on the outcome of the comparison.

In various examples, system and method described in FIGS. 1-3 propose techniques for carrying out analysis of electronic message for phishing detection. The technique enables to the addition of an indicator to emails to visually indicate to users that an email may be a phishing attempt. Additionally, the technique notifies an organization's computer system administrators regarding any synchronized attacks targeting multiple of their users by identifying any found patterns in incoming emails. Furthermore, the technique alerts an organization's computer system administrators about any possible security compromises that may result in phishing attacks within the organization. In addition, the technique assists in determining any coordinated phishing attacks against an organization by determining phishing attacks with similar characteristics against multiple users of that organization. In addition, the technique, as described in above, uses an outbound email reply as a trust factor for the sender/sender organization of the original email in determining the phishing nature of a received email from the sender/sender organization. Also, the above technique uses changing patterns of outbound emails to help determine whether an email client has been compromised and a sender/sender organization is sending any phishing email. Moreover, the above technique allows users to specify an email as a phishing attempt or a legitimate email and use the characteristics of the flagged email to filter messages to other uses at that organization.

Although certain methods, apparatus, and articles of manufacture have been described herein, the scope of coverage of this patent is not limited thereto. To the contrary, this patent covers all methods, apparatus, and articles of manufacture fairly falling within the scope of the appended claims either literally or under the doctrine of equivalents.

## Claims (30)

What is claimed is:

1. A server implemented method for analyzing electronic messages for phishing detection, comprising:

receiving, by the server, an email message by a recipient/recipient organization from a sender/sender organization;

obtaining, by the server, email characteristics by parsing the received email message based on a set of predetermined email characteristics;

comparing, by the server, the email characteristics of the received email message with the email characteristics associated with the recipient/recipient organization, and/or the sender/sender organization;

declaring, by the server, the received email message by the recipient/recipient organization as a phishing electronic message based on the outcome of the comparison;

wherein the email characteristics are selected from the group consisting of network path used to reach a recipient/recipient organization, geography associated with IP address, email client software used by the sender/sender organization, email client software version used by the sender/sender organization, date, day of week, time, time period of the email, time zone of the sender/sender organization, presence and details of digital signatures in the email, meta data present in header portion of the email, character set used in content of the email, format of the email, email length and subject length, character case of the email, character case of the subject, style of introduction at the top of the email, style and content of the sender/sender organization's signature in the body of the email, other recipient/recipient organizations included in the email, to, and copy circulated (cc'd) email addresses, sender/sender organizations name, sender/sender organizations from and reply to email address, senders organization name, senders domain name, sender's organization's Domain Name Service (DNS) settings including SPF records, sender organization's mail server information, including server ip address, sender/sender organization server network path, sender/sender organization email server software and software version. DKIM signature, spam scoring from spam software, message ID, volume of email sent by the sender/sender organization, volume of email sent by sender's organization, volume of email received by the recipient, volume of email received by recipient organization, details associated with URLs or attachments in the email, whether the recipient/recipient organization has responded to this specific email, and number of interactions between sender and recipient associated with the email and the like; and

allowing an administrator to select desired email characteristics to be included in the set of characteristics used for comparing the characteristics of the received email message and to assign a weight of how much each characteristic should influence the likelihood that a new message is a phishing message.

2. The method of claim 1, further comprising:

importing emails received by the recipient/recipient organization over a predetermined time interval;

obtaining email characteristics of the imported emails by parsing the recipient/recipient organization's received emails based on the set of predetermined email characteristics; and

storing the obtained email characteristics associated with the recipient/recipient organization's and the sender/sender organization's received emails in a database.

3. The method of claim 1, wherein comparing the email characteristics of the received email message with stored email characteristics associated with the recipient/recipient organization and/or the sender/sender organization, comprises:

obtaining a statistical distribution of each of the stored email characteristics associated with the recipient/recipient organization and/or sender/sender organization; and

comparing the email characteristics of the received email message with the obtained statistical distribution of prior email characteristics associated with the recipient/recipient organization and/or sender/sender organization.

4. The method of claim 3, further comprising:

determining degree of variance of each email characteristic when compared with the associated statistical distribution;

establishing a score based on the determined degree of variance for each email characteristic;

assigning weights for each established score based on the determined degree of variance; and

obtaining a combined score by adding scores of all the email characteristics in the received email based on the assigned weights.

5. The method of claim 1, further comprising:

storing logs of received emails and any associated phishing activity along with details of why the email was determined to be a phishing email; and

outputting the logs of the received emails and any associated phishing activity for viewing on a display device.

6. The method of claim 1, further comprising:

quarantining emails determined to be phishing emails;

forwarding quarantined emails to certain users;

adding certain text to the header or subject of quarantined emails to mark them as suspect; and

outputting quarantined emails for viewing on a display device.

7. The method of claim 1, further comprising:

parsing outbound emails sent by the recipient/recipient organization based on a set of predetermined email characteristics to determine if the outbound email is a response or forward of a previously received email by the recipient/recipient organization;

updating the database based on the above determination to indicate that the characteristics of the previously received email are more likely to represent a legitimate sender/sender organization;

comparing ongoing emails received from the sender/sender organization with stored email characteristics; and

declaring any of the ongoing emails received from the sender/sender organizations as phishing based on the outcome of the comparison.

8. The method of claim 1, further comprising:

including visual identifications and reasoning information to the received email based on the outcome of the comparison to assist the recipient/recipient organization of the nature of the received email.

9. The method of claim 1, further comprising:

determining coordinated phishing attacks against an organization by spotting phishing attacks having similar characteristics against multiple users in the organization.

10. The method of claim 1, further comprising:

monitoring changing patterns of outbound emails to determine whether an email client has been compromised and the sender/sender organization is sending a phishing email.

11. The method of claim 1, further comprising:

allowing users to specify an email as a phishing attempt and use the characteristics of this flagged email to filter messages to other users in the organization.

12. A server implemented method for analyzing electronic messages for phishing detection comprising:

receiving, by the server, an email message by a recipient/recipient organization from a sender/sender organization;

obtaining, by the server, email characteristics by parsing the received email message based on a set of predetermined email characteristics;

comparing, by the server the email characteristics of the received email message with the email characteristics associated with the recipient/recipient organization, and/or the sender/sender organization;

declaring, by the server, the received email message by the recipient/recipient organization as a phishing electronic message based on the outcome of the comparison;

obtaining contact and background information associated with an email recipient/recipient organization from the recipient's/recipient organizations' online social networks;

storing the contact and background information in the database;

upon receiving an email, determining whether the contact and background information in the received email is correct using the stored contact and background information; and

using outcome of determination as a factor in declaring the received email as a phishing email.

13. The method of claim 12 further comprising:

importing emails received by the recipient/recipient organization over a predetermined time interval;

obtaining email characteristics of the imported emails by parsing the recipient/recipient organization's received emails based on the set of predetermined email characteristics; and

storing the obtained email characteristics associated with the recipient/recipient organization's and the sender/sender organization's received emails in a database.

14. The method of claim 12 wherein comparing the email characteristics of the received email message with stored email characteristics associated with the recipient/recipient organization and/or the sender/sender organization, comprises:

obtaining a statistical distribution of each of the stored email characteristics associated with the recipient/recipient organization and/or sender/sender organization; and

comparing the email characteristics of the received email message with the obtained statistical distribution of prior email characteristics associated with the recipient/recipient organization and/or sender/sender organization.

15. The method of claim 12 further comprising:

parsing outbound emails sent by the recipient/recipient organization based on a set of predetermined email characteristics to determine if the outbound email is a response or forward of a previously received email by the recipient/recipient organization;

updating the database based on the above determination to indicate that the characteristics of the previously received email are more likely to represent a legitimate sender/sender organization;

comparing ongoing emails received from the sender/sender organization with stored email characteristics; and

declaring any of the ongoing emails received from the sender/sender organizations as phishing based on the outcome of the comparison.

16. A system for analyzing electronic messages for phishing detection, comprising:

one or more recipient's/recipient organization's email servers;

one or more sender's email clients;

one or more recipient's email clients;

Intranet or Internet;

a database; and

one or more anti-phishing servers coupled to the database, and further the one or more anti-phishing servers coupled to the one or more recipient's/recipient's organization's email servers, the one or more sender's email clients, and/or the one or more recipient's email clients via Internet or Intranet, wherein the email client plugin module attaches to one or more recipient's email clients and wherein the anti-phishing server comprises:

a processor; and

a memory coupled to the processor, wherein the memory comprising a anti-phishing module, wherein the anti-phishing module comprises an import module, an analysis and data warehouse module, a mail handler module, an organizational analysis module, an outbound mail relay module, a configuration and management module that are configured to:

receiving an email message from one or more sender/sender organizations by one or more recipients/recipient's organization via the mail handler module;

obtaining email characteristics by parsing the received email message based on a set of predetermined email characteristics by the analysis and data warehouse module;

comparing the email characteristics of the received email message with email characteristics associated with the recipient/recipient organization and/or that sender/sender organization by the analysis and data warehouse module; and

declaring the received email message by the recipient/recipient organization as a phishing electronic message based on the outcome of the comparison by the analysis and data warehouse module;

wherein the email characteristics are selected from the group consisting of network path used to reach a recipient/recipient organization, geography associated with IP address, email client software used by the sender/sender organization, email client software version used by the sender/sender organization, date, day of week, time, time period of the email, time zone of the sender/sender organization, presence and details of digital signatures in the email, meta data present in header portion of the email, character set used in content of the email, format of the email, email length and subject length, character case of the email, character case of the subject, style of introduction at the top of the email, style and content of the sender/sender organization's signature in the body of the email, other recipient/recipient organizations included in the email, to, and copy circulated (cc'd) email addresses, sender/sender organizations name, sender/sender organizations from and reply to email address, senders organization name, senders domain name, sender's organization's Domain Name Service (DNS) settings including SPF records, sender organization's mail server information, including server ip address, sender/sender organization server network path, sender/sender organization email server software and software version, DKIM signature, spam scoring from spam software, message ID, volume of email sent by the sender/sender organization, volume of email sent by sender's organization, volume of email received by the recipient, volume of email received by recipient organization, details associated with URLs or attachments in the email, whether the recipient/recipient organization has responded to this specific email, and number of interactions between sender and recipient associated with the email and the like; and

wherein the configuration and management module allows an administrator to select desired email characteristics to be included in the set of characteristics used for comparing the characteristics of the received email message and to assign a weight of how much each characteristic should influence the likelihood that a new message is a phishing message.

17. The system of claim 16, wherein either the import module or the email client plugin module directly imports emails received by the recipient/recipient organization over a predetermined time interval, wherein the analysis and data warehouse module parses the recipient/recipient organization's received emails based on the set of predetermined email characteristics to obtain email characteristics of the imported emails, and wherein the analysis and data warehouse module stores the obtained email characteristics associated with the recipient/recipient organization's and/or sender/sender organization's received email in the database.

18. The system of claim 16, wherein the analysis and data warehouse module obtains a statistical distribution of each of the stored email characteristics associated with the recipient/recipient organization and/or the sender/sender organization, and wherein the analysis and data warehouse module compares the email characteristics of the received email message with the obtain statistical distribution of prior email characteristics associated with the recipient/recipient organization and/or sender/sender organization.

19. The system of claim 18, wherein the analysis and data warehouse module determines degree of variance of each email characteristic when compared with the associated statistical distribution, wherein the analysis and data warehouse module establishes a score based on the determined degree of variance for each email characteristic, wherein the analysis and data warehouse module assigns weights for each established score based on the determined degree of variance, and wherein the analysis and data warehouse module obtains a combined score by adding scores of all the email characteristics in the received email based on the assigned weights.

20. The system of claim 16, wherein the analysis and data warehouse module stores logs of received emails and any associated phishing activity along with details of why the email was determined to be a phishing email in the database, and wherein the configuration and management module outputs the logs of the received emails and any associated phishing activity for viewing on a display device.

21. The system of claim 16, wherein the mail handler module quarantines emails determined to be phishing emails, wherein the configuration and management module forwards quarantined emails to certain users, wherein the configuration and management module adds certain text to the header or subject of quarantined emails to mark them as suspect, and wherein the configuration and management module outputs the quarantined emails for viewing on a display device.

22. The system of claim 16, wherein either the email client plugin module or the outbound mail relay module parses outbound emails sent by the recipient/recipients' organization based on a set of predetermined email characteristics to determine if the outbound email is a response or forward of a previously received email by the recipient/recipient organization, wherein the analysis and data warehouse module updates the database based on the above determination to indicate that the characteristics of the previously received email are more likely to represent a legitimate sender/sender organization, wherein the analysis and data warehouse module compares ongoing emails received from the sender/sender organizations with stored email characteristics, and wherein the analysis and data warehouse module declares any of the ongoing emails received from the sender/sender organizations as phishing based on the outcome of the comparison.

23. The system of claim 16, wherein the mail handler module along with the email client plugin module includes visual identifications and reasoning information to the received email based on the outcome of the comparison to assist the recipient/recipient organization of the nature of the received email.

24. The system of claim 16, wherein the analysis and data warehouse module determines coordinated phishing attacks against an organization by spotting phishing attacks having similar characteristics against multiple users in the organization.

25. The system of claim 16, wherein the organization analysis module monitors changing patterns of outbound emails to determine whether an email client has been compromised and the sender/sender organization is sending a phishing email.

26. The system of claim 16, wherein either the email client plugin module or the configuration and management module allows users to specify an email as a phishing attempt and use the characteristics of this flagged email to filter messages to other users in the organization.

27. A system for analyzing electronic messages for phishing detection, comprising:

one or more recipient's/recipient organization's email servers;

one or more sender's email clients:

one or more recipient's email clients;

Intranet or Internet;

a database; and

one or more anti-phishing servers coupled to the database, and further the one or more anti-phishing servers coupled to the one or more recipient's/recipient's organization's email servers, the one or more sender's email clients, and/or the one or more recipient's email clients via Internet or Intranet, wherein the email client plugin module attaches to one or more recipient's email clients and wherein the anti-phishing server comprises:

a processor; and

a memory coupled to the processor, wherein the memory comprising a anti-phishing module, wherein the anti-phishing module comprises an import module, an analysis and data warehouse module, a mail handler module, an organizational analysis module, an outbound mail relay module, a configuration and management module that are configured to:

receiving an email message from one or more sender/sender organizations by one or more recipients/recipient's organization via the mail handler module;

obtaining email characteristics by parsing the received email message based on a set of predetermined email characteristics by the analysis and data warehouse module;

comparing the email characteristics of the received email message with email characteristics associated with the recipient/recipient organization and/or that sender/sender organization by the analysis and data warehouse module;

declaring the received email message by the recipient/recipient organization as a phishing electronic message based on the outcome of the comparison by the analysis and data warehouse module; and

wherein the email client plugin module along with the configuration and management module obtains contact and background information associated with an email recipient from the recipient's online social networks, wherein analysis and data warehouse module stores the contact and background information in the database, wherein the analysis and data ware house module, upon receiving an email, determines whether the contact and background information in the received email is correct using the stored contact and background information, and wherein analysis and data warehouse module uses the outcome of the above determination as a factor in declaring the received email as phishing email.

28. The system of claim 27 wherein either the import module or the email client plugin module directly imports emails received by the recipient/recipient organization over a predetermined time interval, wherein the analysis and data warehouse module parses the recipient/recipient organization's received emails based on the set of predetermined email characteristics to obtain email characteristics of the imported emails, and wherein the analysis and data warehouse module stores the obtained email characteristics associated with the recipient/recipient organization's and/or sender/sender organization's received email in the database.

29. The system of claim 27 wherein the analysis and data warehouse module obtains a statistical distribution of each of the stored email characteristics associated with the recipient/recipient organization and/or the sender/sender organization, and wherein the analysis and data warehouse module compares the email characteristics of the received email message with the obtain statistical distribution of prior email characteristics associated with the recipient/recipient organization and/or sender/sender organization.

30. The system of claim 27 wherein either the email client plugin module or the outbound mail relay module parses outbound emails sent by the recipient/recipients' organization based on a set of predetermined email characteristics to determine if the outbound email is a response or forward of a previously received email by the recipient/recipient organization, wherein the analysis and data warehouse module updates the database based on the above determination to indicate that the characteristics of the previously received email are more likely to represent a legitimate sender/sender organization, wherein the analysis and data warehouse module compares ongoing emails received from the sender/sender organizations with stored email characteristics, and wherein the analysis and data warehouse module declares any of the ongoing emails received from the sender/sender organizations as phishing based on the outcome of the comparison.

US13/668,349
2012-11-05
2012-11-05
System and method for electronic message analysis for phishing detection
Active
[US8566938B1
(en)](/patent/US8566938B1/en)

## Priority Applications (3)

| Application Number | Priority Date | Filing Date | Title |
| --- | --- | --- | --- |
| US13/668,349 [US8566938B1 (en)](/patent/US8566938B1/en) | 2012-11-05 | 2012-11-05 | System and method for electronic message analysis for phishing detection |
| US14/045,244 [US9154514B1 (en)](/patent/US9154514B1/en) | 2012-11-05 | 2013-10-03 | Systems and methods for electronic message analysis |
| US14/864,656 [US9501746B2 (en)](/patent/US9501746B2/en) | 2012-11-05 | 2015-09-24 | Systems and methods for electronic message analysis |

## Applications Claiming Priority (1)

| Application Number | Priority Date | Filing Date | Title |
| --- | --- | --- | --- |
| US13/668,349 [US8566938B1 (en)](/patent/US8566938B1/en) | 2012-11-05 | 2012-11-05 | System and method for electronic message analysis for phishing detection |

## Related Child Applications (1)

| Application Number | Title | Priority Date | Filing Date |
| --- | --- | --- | --- |
| US14/045,244 Continuation-In-Part [US9154514B1 (en)](/patent/US9154514B1/en) | 2012-11-05 | 2013-10-03 | Systems and methods for electronic message analysis |

## Publications (1)

| Publication Number | Publication Date |
| --- | --- |
| US8566938B1 true [US8566938B1 (en)](/patent/US8566938B1/en) | 2013-10-22 |

# Family

## ID=49355420

## Family Applications (1)

| Application Number | Title | Priority Date | Filing Date |
| --- | --- | --- | --- |
| US13/668,349 Active [US8566938B1 (en)](/patent/US8566938B1/en) | 2012-11-05 | 2012-11-05 | System and method for electronic message analysis for phishing detection |

## Country Status (1)

| Country | Link |
| --- | --- |
| US (1) | [US8566938B1 (en)](/patent/US8566938B1/en) |

## Cited By (233)

\* Cited by examiner, † Cited by third party

| Publication number | Priority date | Publication date | Assignee | Title |
| --- | --- | --- | --- | --- |
| [US20140020047A1 (en)](/patent/US20140020047A1/en) \* | 2012-07-16 | 2014-01-16 | Nicholas Liebmann | Cloud email message scanning with local policy application in a network environment |
| [US20140082726A1 (en)](/patent/US20140082726A1/en) \* | 2012-09-14 | 2014-03-20 | Return Path, Inc. | Real-time classification of email message traffic |
| [US20140230060A1 (en)](/patent/US20140230060A1/en) \* | 2013-02-08 | 2014-08-14 | PhishMe, Inc. | Collaborative phishing attack detection |
| [US8839369B1 (en)](/patent/US8839369B1/en) \* | 2012-11-09 | 2014-09-16 | Trend Micro Incorporated | Methods and systems for detecting email phishing attacks |
| [US9141790B2 (en)](/patent/US9141790B2/en) | 2013-09-10 | 2015-09-22 | Symantec Corporation | Systems and methods for using event-correlation graphs to detect attacks on computing systems |
| [US9148441B1 (en)](/patent/US9148441B1/en) | 2013-12-23 | 2015-09-29 | Symantec Corporation | Systems and methods for adjusting suspiciousness scores in event-correlation graphs |
| [US9166997B1 (en)](/patent/US9166997B1/en) | 2013-09-19 | 2015-10-20 | Symantec Corporation | Systems and methods for reducing false positives when using event-correlation graphs to detect attacks on computing systems |
| [CN105072137A (en)](/patent/CN105072137A/en) \* | 2015-09-15 | 2015-11-18 | 蔡丝英 | Spear phishing mail detection method and device |
| [US20150356089A1 (en)](/patent/US20150356089A1/en) \* | 2014-06-10 | 2015-12-10 | International Business Machines Corporation | Weighting Search Criteria Based on Similarities to an Ingested Corpus in a Question and Answer (QA) System |
| [US9256739B1 (en)](/patent/US9256739B1/en) \* | 2014-03-21 | 2016-02-09 | Symantec Corporation | Systems and methods for using event-correlation graphs to generate remediation procedures |
| [US9398047B2 (en)](/patent/US9398047B2/en) | 2014-11-17 | 2016-07-19 | Vade Retro Technology, Inc. | Methods and systems for phishing detection |
| [US9473437B1 (en)](/patent/US9473437B1/en) \* | 2012-02-13 | 2016-10-18 | ZapFraud, Inc. | Tertiary classification of communications |
| [WO2016183358A1 (en)](/patent/WO2016183358A1/en) \* | 2015-05-13 | 2016-11-17 | Google Inc. | Identifying phishing communications using templates |
| [US9536221B2 (en)](/patent/US9536221B2/en) | 2008-06-19 | 2017-01-03 | Plentyoffish Media Ulc | System and method for adaptive matching of user profiles based on viewing and contact activity for social relationship services |
| [WO2017019716A1 (en)](/patent/WO2017019716A1/en) \* | 2015-07-30 | 2017-02-02 | Microsoft Technology Licensing, Llc | Third party email signature generation and authentication |
| [US9591017B1 (en)](/patent/US9591017B1/en) \* | 2013-02-08 | 2017-03-07 | PhishMe, Inc. | Collaborative phishing attack detection |
| [US9667645B1 (en)](/patent/US9667645B1/en) | 2013-02-08 | 2017-05-30 | PhishMe, Inc. | Performance benchmarking for simulated phishing attacks |
| [US9672289B1 (en)](/patent/US9672289B1/en) | 2013-07-23 | 2017-06-06 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate matching of clients in a networked environment |
| [US9679259B1 (en)](/patent/US9679259B1/en) | 2013-01-25 | 2017-06-13 | Plentyoffish Media Ulc | Systems and methods for training and employing a machine learning system in evaluating entity pairs |
| [US9774626B1 (en)](/patent/US9774626B1/en) \* | 2016-08-17 | 2017-09-26 | Wombat Security Technologies, Inc. | Method and system for assessing and classifying reported potentially malicious messages in a cybersecurity system |
| [US9781149B1 (en)](/patent/US9781149B1/en) | 2016-08-17 | 2017-10-03 | Wombat Security Technologies, Inc. | Method and system for reducing reporting of non-malicious electronic messages in a cybersecurity system |
| [US9825986B1 (en)](/patent/US9825986B1/en) | 2015-06-29 | 2017-11-21 | Symantec Corporation | Systems and methods for generating contextually meaningful animated visualizations of computer security events |
| [CN107402936A (en)](/patent/CN107402936A/en) \* | 2016-05-20 | 2017-11-28 | 阿里巴巴集团控股有限公司 | information identifying method and device |
| [US9836533B1 (en)](/patent/US9836533B1/en) | 2014-04-07 | 2017-12-05 | Plentyoffish Media Ulc | Apparatus, method and article to effect user interest-based matching in a network environment |
| [US9843594B1 (en)](/patent/US9843594B1/en) | 2014-10-28 | 2017-12-12 | Symantec Corporation | Systems and methods for detecting anomalous messages in automobile networks |
| [US9847973B1 (en)](/patent/US9847973B1/en) | 2016-09-26 | 2017-12-19 | Agari Data, Inc. | Mitigating communication risk by detecting similarity to a trusted message contact |
| [US9870465B1 (en)](/patent/US9870465B1/en) | 2013-12-04 | 2018-01-16 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate automatic detection and removal of fraudulent user information in a network environment |
| [US9906539B2 (en)](/patent/US9906539B2/en) | 2015-04-10 | 2018-02-27 | PhishMe, Inc. | Suspicious message processing and incident response |
| [US9906545B1 (en)](/patent/US9906545B1/en) | 2016-11-22 | 2018-02-27 | Symantec Corporation | Systems and methods for identifying message payload bit fields in electronic communications |
| [US9912687B1 (en)](/patent/US9912687B1/en) | 2016-08-17 | 2018-03-06 | Wombat Security Technologies, Inc. | Advanced processing of electronic messages with attachments in a cybersecurity system |
| [US9967274B2 (en)](/patent/US9967274B2/en) | 2015-11-25 | 2018-05-08 | Symantec Corporation | Systems and methods for identifying compromised devices within industrial control systems |
| [US20180212994A1 (en)](/patent/US20180212994A1/en) \* | 2015-07-14 | 2018-07-26 | China Internet Network Information Center | E-mail anti-phishing system and method |
| [US10069856B2 (en)](/patent/US10069856B2/en) | 2016-05-13 | 2018-09-04 | King Abdulaziz City For Science And Technology | System and method of comparative evaluation for phishing mitigation |
| [US10091077B1 (en)](/patent/US10091077B1/en) | 2016-06-27 | 2018-10-02 | Symantec Corporation | Systems and methods for detecting transactional message sequences that are obscured in multicast communications |
| [US10104100B1 (en)](/patent/US10104100B1/en) | 2016-03-03 | 2018-10-16 | Symantec Corporation | Systems and methods for detecting anomalies that are potentially indicative of malicious attacks |
| [US10108968B1 (en)](/patent/US10108968B1/en) | 2014-03-05 | 2018-10-23 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate automatic detection and removal of fraudulent advertising accounts in a network environment |
| [US10146893B1 (en)](/patent/US10146893B1/en) | 2015-03-27 | 2018-12-04 | Symantec Corporation | Systems and methods for evaluating electronic control units within vehicle emulations |
| [US10193903B1 (en)](/patent/US10193903B1/en) | 2016-04-29 | 2019-01-29 | Symantec Corporation | Systems and methods for detecting suspicious microcontroller messages |
| [US10200259B1 (en)](/patent/US10200259B1/en) | 2016-09-21 | 2019-02-05 | Symantec Corporation | Systems and methods for detecting obscure cyclic application-layer message sequences in transport-layer message sequences |
| [JP2019028724A (en)](/patent/JP2019028724A/en) \* | 2017-07-31 | 2019-02-21 | キヤノンマーケティングジャパン株式会社 | Information processing apparatus, information processing method, and program |
| [US10243904B1 (en)](/patent/US10243904B1/en) | 2017-05-26 | 2019-03-26 | Wombat Security Technologies, Inc. | Determining authenticity of reported user action in cybersecurity risk assessment |
| [US10277628B1 (en)](/patent/US10277628B1/en) | 2013-09-16 | 2019-04-30 | ZapFraud, Inc. | Detecting phishing attempts |
| [US10284579B2 (en)](/patent/US10284579B2/en) | 2017-03-22 | 2019-05-07 | Vade Secure, Inc. | Detection of email spoofing and spear phishing attacks |
| [US10326788B1 (en)](/patent/US10326788B1/en) | 2017-05-05 | 2019-06-18 | Symantec Corporation | Systems and methods for identifying suspicious controller area network messages |
| [US10334015B2 (en)](/patent/US10334015B2/en) | 2017-04-28 | 2019-06-25 | Bank Of America Corporation | Apparatus and methods for shortening user exposure to malicious websites |
| [US20190238571A1 (en)](/patent/US20190238571A1/en) \* | 2018-01-29 | 2019-08-01 | International Business Machines Corporation | Method and system for email phishing attempts identification and notification through organizational cognitive solutions |
| [US10387795B1 (en)](/patent/US10387795B1/en) | 2014-04-02 | 2019-08-20 | Plentyoffish Media Inc. | Systems and methods for training and employing a machine learning system in providing service level upgrade offers |
| [JP2019145107A (en)](/patent/JP2019145107A/en) \* | 2018-02-20 | 2019-08-29 | ダークトレース リミテッドＤａｒｋｔｒａｃｅ Ｌｉｍｉｔｅｄ | Cyber threat defense system protecting e-email network using machine learning model |
| [JP2019145168A (en)](/patent/JP2019145168A/en) \* | 2019-05-23 | 2019-08-29 | キヤノンマーケティングジャパン株式会社 | Information processor, information processing method, and program |
| [US10419478B2 (en)](/patent/US10419478B2/en) \* | 2017-07-05 | 2019-09-17 | Area 1 Security, Inc. | Identifying malicious messages based on received message data of the sender |
| [US10432720B1 (en)](/patent/US10432720B1/en) | 2014-06-25 | 2019-10-01 | Symantec Corporation | Systems and methods for strong information about transmission control protocol connections |
| [WO2020003406A1 (en)](/patent/WO2020003406A1/en) \* | 2018-06-27 | 2020-01-02 | 三菱電機株式会社 | Suspicious mail detection device, suspicious mail detection method, and suspicious mail detection program |
| [US10540607B1 (en)](/patent/US10540607B1/en) | 2013-12-10 | 2020-01-21 | Plentyoffish Media Ulc | Apparatus, method and article to effect electronic message reply rate matching in a network environment |
| [CN111049733A (en)](/patent/CN111049733A/en) \* | 2019-12-10 | 2020-04-21 | 公安部第三研究所 | A concealed identification method for phishing email attacks |
| [US10674009B1 (en)](/patent/US10674009B1/en) | 2013-11-07 | 2020-06-02 | Rightquestion, Llc | Validating automatic number identification data |
| [US10708297B2 (en)](/patent/US10708297B2/en) | 2017-08-25 | 2020-07-07 | Ecrime Management Strategies, Inc. | Security system for detection and mitigation of malicious communications |
| [US10715543B2 (en)](/patent/US10715543B2/en) | 2016-11-30 | 2020-07-14 | Agari Data, Inc. | Detecting computer security risk based on previously observed communications |
| [US10721195B2 (en)](/patent/US10721195B2/en) | 2016-01-26 | 2020-07-21 | ZapFraud, Inc. | Detection of business email compromise |
| [WO2020161466A1 (en)](/patent/WO2020161466A1/en) \* | 2019-02-07 | 2020-08-13 | Egress Software Technologies Ip Ltd | Method and system for processing data packages |
| [US10769221B1 (en)](/patent/US10769221B1/en) | 2012-08-20 | 2020-09-08 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate matching of clients in a networked environment |
| [US10778717B2 (en)](/patent/US10778717B2/en) | 2017-08-31 | 2020-09-15 | Barracuda Networks, Inc. | System and method for email account takeover detection and remediation |
| [US10805314B2 (en)](/patent/US10805314B2/en) | 2017-05-19 | 2020-10-13 | Agari Data, Inc. | Using message context to evaluate security of requested data |
| [US10880322B1 (en)](/patent/US10880322B1/en) | 2016-09-26 | 2020-12-29 | Agari Data, Inc. | Automated tracking of interaction with a resource of a message |
| [US10929559B2 (en)](/patent/US10929559B2/en) | 2016-06-10 | 2021-02-23 | OneTrust, LLC | Data processing systems for data testing to confirm data deletion and related methods |
| [JP2021039754A (en)](/patent/JP2021039754A/en) \* | 2019-08-29 | 2021-03-11 | ダークトレース リミテッドＤａｒｋｔｒａｃｅ Ｌｉｍｉｔｅｄ | Endpoint agent expansion of machine learning cyber defense system for electronic mail |
| [US10949544B2 (en)](/patent/US10949544B2/en) | 2016-06-10 | 2021-03-16 | OneTrust, LLC | Data processing systems for data transfer risk identification and related methods |
| [US10949170B2 (en)](/patent/US10949170B2/en) | 2016-06-10 | 2021-03-16 | OneTrust, LLC | Data processing systems for integration of consumer feedback with data subject access requests and related methods |
| [US10949565B2 (en)](/patent/US10949565B2/en) | 2016-06-10 | 2021-03-16 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US10949567B2 (en)](/patent/US10949567B2/en) | 2016-06-10 | 2021-03-16 | OneTrust, LLC | Data processing systems for fulfilling data subject access requests and related methods |
| [US10956952B2 (en)](/patent/US10956952B2/en) | 2016-04-01 | 2021-03-23 | OneTrust, LLC | Data processing systems and communication systems and methods for the efficient generation of privacy risk assessments |
| [US10963591B2 (en)](/patent/US10963591B2/en) | 2018-09-07 | 2021-03-30 | OneTrust, LLC | Data processing systems for orphaned data identification and deletion and related methods |
| [US10970675B2 (en)](/patent/US10970675B2/en) | 2016-06-10 | 2021-04-06 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US10970371B2 (en)](/patent/US10970371B2/en) | 2016-06-10 | 2021-04-06 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US10972509B2 (en)](/patent/US10972509B2/en) | 2016-06-10 | 2021-04-06 | OneTrust, LLC | Data processing and scanning systems for generating and populating a data inventory |
| [US10984132B2 (en)](/patent/US10984132B2/en) | 2016-06-10 | 2021-04-20 | OneTrust, LLC | Data processing systems and methods for populating and maintaining a centralized database of personal data |
| [US10997315B2 (en)](/patent/US10997315B2/en) | 2016-06-10 | 2021-05-04 | OneTrust, LLC | Data processing systems for fulfilling data subject access requests and related methods |
| [US10997318B2 (en)](/patent/US10997318B2/en) | 2016-06-10 | 2021-05-04 | OneTrust, LLC | Data processing systems for generating and populating a data inventory for processing data access requests |
| [US10997542B2 (en)](/patent/US10997542B2/en) | 2016-06-10 | 2021-05-04 | OneTrust, LLC | Privacy management systems and methods |
| [US11004125B2 (en)](/patent/US11004125B2/en) | 2016-04-01 | 2021-05-11 | OneTrust, LLC | Data processing systems and methods for integrating privacy information management systems with data loss prevention tools or other tools for privacy design |
| [US11019076B1 (en)](/patent/US11019076B1/en) | 2017-04-26 | 2021-05-25 | Agari Data, Inc. | Message security assessment using sender identity profiles |
| [US11023616B2 (en)](/patent/US11023616B2/en) | 2016-06-10 | 2021-06-01 | OneTrust, LLC | Data processing systems for identifying, assessing, and remediating data processing risks using data modeling techniques |
| [US11023842B2 (en)](/patent/US11023842B2/en) | 2016-06-10 | 2021-06-01 | OneTrust, LLC | Data processing systems and methods for bundled privacy policies |
| [US11025651B2 (en)](/patent/US11025651B2/en) | 2018-12-06 | 2021-06-01 | Saudi Arabian Oil Company | System and method for enhanced security analysis for quarantined email messages |
| [US11025675B2 (en)](/patent/US11025675B2/en) | 2016-06-10 | 2021-06-01 | OneTrust, LLC | Data processing systems and methods for performing privacy assessments and monitoring of new versions of computer code for privacy compliance |
| [US11030327B2 (en)](/patent/US11030327B2/en) | 2016-06-10 | 2021-06-08 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11030274B2 (en)](/patent/US11030274B2/en) | 2016-06-10 | 2021-06-08 | OneTrust, LLC | Data processing user interface monitoring systems and related methods |
| [US11030563B2 (en)](/patent/US11030563B2/en) | 2016-06-10 | 2021-06-08 | OneTrust, LLC | Privacy management systems and methods |
| [US11036882B2 (en)](/patent/US11036882B2/en) | 2016-06-10 | 2021-06-15 | OneTrust, LLC | Data processing systems for processing and managing data subject access in a distributed environment |
| [US11038925B2 (en)](/patent/US11038925B2/en) | 2016-06-10 | 2021-06-15 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11036771B2 (en)](/patent/US11036771B2/en) | 2016-06-10 | 2021-06-15 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US11036674B2 (en)](/patent/US11036674B2/en) | 2016-06-10 | 2021-06-15 | OneTrust, LLC | Data processing systems for processing data subject access requests |
| [US11044267B2 (en)](/patent/US11044267B2/en) | 2016-11-30 | 2021-06-22 | Agari Data, Inc. | Using a measure of influence of sender in determining a security risk associated with an electronic message |
| [US11050698B1 (en)](/patent/US11050698B1/en) \* | 2020-09-18 | 2021-06-29 | Area 1 Security, Inc. | Message processing system with business email compromise detection |
| [US11057356B2 (en)](/patent/US11057356B2/en) | 2016-06-10 | 2021-07-06 | OneTrust, LLC | Automated data processing systems and methods for automatically processing data subject access requests using a chatbot |
| [US11062051B2 (en)](/patent/US11062051B2/en) | 2016-06-10 | 2021-07-13 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US11070593B2 (en)](/patent/US11070593B2/en) | 2016-06-10 | 2021-07-20 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11068618B2 (en)](/patent/US11068618B2/en) | 2016-06-10 | 2021-07-20 | OneTrust, LLC | Data processing systems for central consent repository and related methods |
| [US11074367B2 (en)](/patent/US11074367B2/en) | 2016-06-10 | 2021-07-27 | OneTrust, LLC | Data processing systems for identity validation for consumer rights requests and related methods |
| [US11087260B2 (en)](/patent/US11087260B2/en) | 2016-06-10 | 2021-08-10 | OneTrust, LLC | Data processing systems and methods for customizing privacy training |
| [US11100444B2 (en)](/patent/US11100444B2/en) | 2016-06-10 | 2021-08-24 | OneTrust, LLC | Data processing systems and methods for providing training in a vendor procurement process |
| [US11100445B2 (en)](/patent/US11100445B2/en) | 2016-06-10 | 2021-08-24 | OneTrust, LLC | Data processing systems for assessing readiness for responding to privacy-related incidents |
| [US11102244B1 (en)](/patent/US11102244B1/en) | 2017-06-07 | 2021-08-24 | Agari Data, Inc. | Automated intelligence gathering |
| [US11113416B2 (en)](/patent/US11113416B2/en) | 2016-06-10 | 2021-09-07 | OneTrust, LLC | Application privacy scanning systems and related methods |
| [US11122011B2 (en)](/patent/US11122011B2/en) | 2016-06-10 | 2021-09-14 | OneTrust, LLC | Data processing systems and methods for using a data model to select a target data asset in a data migration |
| [US11120161B2 (en)](/patent/US11120161B2/en) | 2016-06-10 | 2021-09-14 | OneTrust, LLC | Data subject access request processing systems and related methods |
| [US11126748B2 (en)](/patent/US11126748B2/en) | 2016-06-10 | 2021-09-21 | OneTrust, LLC | Data processing consent management systems and related methods |
| [GB2581188B (en)](/patent/GB2581188B/en) \* | 2019-02-07 | 2021-09-22 | Egress Software Tech Ip Limited | Method and system for processing data packages |
| [US11132646B2 (en)](/patent/US11132646B2/en) \* | 2017-04-12 | 2021-09-28 | Fujifilm Business Innovation Corp. | Non-transitory computer-readable medium and email processing device for misrepresentation handling |
| [US11134086B2 (en)](/patent/US11134086B2/en) | 2016-06-10 | 2021-09-28 | OneTrust, LLC | Consent conversion optimization systems and related methods |
| [US11138242B2 (en)](/patent/US11138242B2/en) | 2016-06-10 | 2021-10-05 | OneTrust, LLC | Data processing systems and methods for automatically detecting and documenting privacy-related aspects of computer software |
| [US11138299B2 (en)](/patent/US11138299B2/en) | 2016-06-10 | 2021-10-05 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11144675B2 (en)](/patent/US11144675B2/en) | 2018-09-07 | 2021-10-12 | OneTrust, LLC | Data processing systems and methods for automatically protecting sensitive data within privacy management systems |
| [US11144670B2 (en)](/patent/US11144670B2/en) | 2016-06-10 | 2021-10-12 | OneTrust, LLC | Data processing systems for identifying and modifying processes that are subject to data subject access requests |
| [US11146566B2 (en)](/patent/US11146566B2/en) | 2016-06-10 | 2021-10-12 | OneTrust, LLC | Data processing systems for fulfilling data subject access requests and related methods |
| [US11144622B2 (en)](/patent/US11144622B2/en) | 2016-06-10 | 2021-10-12 | OneTrust, LLC | Privacy management systems and methods |
| [US11151233B2 (en)](/patent/US11151233B2/en) | 2016-06-10 | 2021-10-19 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11157600B2 (en)](/patent/US11157600B2/en) | 2016-06-10 | 2021-10-26 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [GB2581189B (en)](/patent/GB2581189B/en) \* | 2019-02-07 | 2021-10-27 | Egress Software Tech Ip Limited | Method and system for processing data packages |
| [GB2581190B (en)](/patent/GB2581190B/en) \* | 2019-02-07 | 2021-10-27 | Egress Software Tech Ip Limited | Method and system for processing data packages |
| [RU2758358C2 (en)](/patent/RU2758358C2/en) \* | 2020-02-26 | 2021-10-28 | Акционерное общество "Лаборатория Касперского" | Method for generating signature for spam detection |
| [US11164156B1 (en)](/patent/US11164156B1/en) \* | 2021-04-30 | 2021-11-02 | Oracle International Corporation | Email message receiving system in a cloud infrastructure |
| [US20210367918A1 (en)](/patent/US20210367918A1/en) \* | 2020-05-22 | 2021-11-25 | Nvidia Corporation | User perceptible indicia for web address identifiers |
| [US11188615B2 (en)](/patent/US11188615B2/en) | 2016-06-10 | 2021-11-30 | OneTrust, LLC | Data processing consent capture systems and related methods |
| [US11188862B2 (en)](/patent/US11188862B2/en) | 2016-06-10 | 2021-11-30 | OneTrust, LLC | Privacy management systems and methods |
| [US11195134B2 (en)](/patent/US11195134B2/en) | 2016-06-10 | 2021-12-07 | OneTrust, LLC | Privacy management systems and methods |
| [US11200341B2 (en)](/patent/US11200341B2/en) | 2016-06-10 | 2021-12-14 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US11210420B2 (en)](/patent/US11210420B2/en) | 2016-06-10 | 2021-12-28 | OneTrust, LLC | Data subject access request processing systems and related methods |
| [US11222139B2 (en)](/patent/US11222139B2/en) | 2016-06-10 | 2022-01-11 | OneTrust, LLC | Data processing systems and methods for automatic discovery and assessment of mobile software development kits |
| [US11222309B2 (en)](/patent/US11222309B2/en) | 2016-06-10 | 2022-01-11 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US11222142B2 (en)](/patent/US11222142B2/en) | 2016-06-10 | 2022-01-11 | OneTrust, LLC | Data processing systems for validating authorization for personal data collection, storage, and processing |
| [US11228620B2 (en)](/patent/US11228620B2/en) | 2016-06-10 | 2022-01-18 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11227247B2 (en)](/patent/US11227247B2/en) | 2016-06-10 | 2022-01-18 | OneTrust, LLC | Data processing systems and methods for bundled privacy policies |
| [US11238390B2 (en)](/patent/US11238390B2/en) | 2016-06-10 | 2022-02-01 | OneTrust, LLC | Privacy management systems and methods |
| [US11244071B2 (en)](/patent/US11244071B2/en) \* | 2016-06-10 | 2022-02-08 | OneTrust, LLC | Data processing systems for use in automatically generating, populating, and submitting data subject access requests |
| [US11244367B2 (en)](/patent/US11244367B2/en) | 2016-04-01 | 2022-02-08 | OneTrust, LLC | Data processing systems and methods for integrating privacy information management systems with data loss prevention tools or other tools for privacy design |
| [US11277448B2 (en)](/patent/US11277448B2/en) | 2016-06-10 | 2022-03-15 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11294939B2 (en)](/patent/US11294939B2/en) | 2016-06-10 | 2022-04-05 | OneTrust, LLC | Data processing systems and methods for automatically detecting and documenting privacy-related aspects of computer software |
| [US11295316B2 (en)](/patent/US11295316B2/en) | 2016-06-10 | 2022-04-05 | OneTrust, LLC | Data processing systems for identity validation for consumer rights requests and related methods |
| [US11297101B1 (en)](/patent/US11297101B1/en) | 2018-08-22 | 2022-04-05 | NuRD LLC | Phishing website detection by checking form differences followed by false credentials submission |
| [US11301589B2 (en)](/patent/US11301589B2/en) | 2016-06-10 | 2022-04-12 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US11301796B2 (en)](/patent/US11301796B2/en) | 2016-06-10 | 2022-04-12 | OneTrust, LLC | Data processing systems and methods for customizing privacy training |
| [US11308435B2 (en)](/patent/US11308435B2/en) | 2016-06-10 | 2022-04-19 | OneTrust, LLC | Data processing systems for identifying, assessing, and remediating data processing risks using data modeling techniques |
| [US11328092B2 (en)](/patent/US11328092B2/en) | 2016-06-10 | 2022-05-10 | OneTrust, LLC | Data processing systems for processing and managing data subject access in a distributed environment |
| [US11336697B2 (en)](/patent/US11336697B2/en) | 2016-06-10 | 2022-05-17 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11341447B2 (en)](/patent/US11341447B2/en) | 2016-06-10 | 2022-05-24 | OneTrust, LLC | Privacy management systems and methods |
| [US11343284B2 (en)](/patent/US11343284B2/en) | 2016-06-10 | 2022-05-24 | OneTrust, LLC | Data processing systems and methods for performing privacy assessments and monitoring of new versions of computer code for privacy compliance |
| [US11354435B2 (en)](/patent/US11354435B2/en) | 2016-06-10 | 2022-06-07 | OneTrust, LLC | Data processing systems for data testing to confirm data deletion and related methods |
| [US11354434B2 (en)](/patent/US11354434B2/en) | 2016-06-10 | 2022-06-07 | OneTrust, LLC | Data processing systems for verification of consent and notice processing and related methods |
| [US11366909B2 (en)](/patent/US11366909B2/en) | 2016-06-10 | 2022-06-21 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11366786B2 (en)](/patent/US11366786B2/en) | 2016-06-10 | 2022-06-21 | OneTrust, LLC | Data processing systems for processing data subject access requests |
| [US11373007B2 (en)](/patent/US11373007B2/en) | 2017-06-16 | 2022-06-28 | OneTrust, LLC | Data processing systems for identifying whether cookies contain personally identifying information |
| [US11392720B2 (en)](/patent/US11392720B2/en) | 2016-06-10 | 2022-07-19 | OneTrust, LLC | Data processing systems for verification of consent and notice processing and related methods |
| [US11397819B2 (en)](/patent/US11397819B2/en) | 2020-11-06 | 2022-07-26 | OneTrust, LLC | Systems and methods for identifying data processing activities based on data discovery results |
| [US11403377B2 (en)](/patent/US11403377B2/en) | 2016-06-10 | 2022-08-02 | OneTrust, LLC | Privacy management systems and methods |
| [US11410106B2 (en)](/patent/US11410106B2/en) | 2016-06-10 | 2022-08-09 | OneTrust, LLC | Privacy management systems and methods |
| [US11411990B2 (en)](/patent/US11411990B2/en) \* | 2019-02-15 | 2022-08-09 | Forcepoint Llc | Early detection of potentially-compromised email accounts |
| [US11418492B2 (en)](/patent/US11418492B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Data processing systems and methods for using a data model to select a target data asset in a data migration |
| [US11416798B2 (en)](/patent/US11416798B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Data processing systems and methods for providing training in a vendor procurement process |
| [US11416634B2 (en)](/patent/US11416634B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US11416589B2 (en)](/patent/US11416589B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11416590B2 (en)](/patent/US11416590B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11416109B2 (en)](/patent/US11416109B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Automated data processing systems and methods for automatically processing data subject access requests using a chatbot |
| [US11431738B2 (en)](/patent/US11431738B2/en) | 2018-12-19 | 2022-08-30 | Abnormal Security Corporation | Multistage analysis of emails to identify security threats |
| [US11438386B2 (en)](/patent/US11438386B2/en) | 2016-06-10 | 2022-09-06 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11436373B2 (en)](/patent/US11436373B2/en) | 2020-09-15 | 2022-09-06 | OneTrust, LLC | Data processing systems and methods for detecting tools for the automatic blocking of consent requests |
| [US11438292B1 (en)](/patent/US11438292B1/en) \* | 2021-04-12 | 2022-09-06 | EMC IP Holding Company LLC | Method and apparatus for filtering undesired email messages |
| [US11444976B2 (en)](/patent/US11444976B2/en) | 2020-07-28 | 2022-09-13 | OneTrust, LLC | Systems and methods for automatically blocking the use of tracking tools |
| [US11442906B2 (en)](/patent/US11442906B2/en) | 2021-02-04 | 2022-09-13 | OneTrust, LLC | Managing custom attributes for domain objects defined within microservices |
| [US11451576B2 (en)](/patent/US11451576B2/en) | 2020-03-12 | 2022-09-20 | Abnormal Security Corporation | Investigation of threats using queryable records of behavior |
| [US11461500B2 (en)](/patent/US11461500B2/en) | 2016-06-10 | 2022-10-04 | OneTrust, LLC | Data processing systems for cookie compliance testing with website scanning and related methods |
| [US11470108B2 (en)](/patent/US11470108B2/en) | 2020-04-23 | 2022-10-11 | Abnormal Security Corporation | Detection and prevention of external fraud |
| [US11470042B2 (en)](/patent/US11470042B2/en) | 2020-02-21 | 2022-10-11 | Abnormal Security Corporation | Discovering email account compromise through assessments of digital activities |
| [US11475136B2 (en)](/patent/US11475136B2/en) | 2016-06-10 | 2022-10-18 | OneTrust, LLC | Data processing systems for data transfer risk identification and related methods |
| [US11475165B2 (en)](/patent/US11475165B2/en) | 2020-08-06 | 2022-10-18 | OneTrust, LLC | Data processing systems and methods for automatically redacting unstructured data from a data subject access request |
| [US11477234B2 (en)](/patent/US11477234B2/en) \* | 2020-02-28 | 2022-10-18 | Abnormal Security Corporation | Federated database for establishing and tracking risk of interactions with third parties |
| [US11481710B2 (en)](/patent/US11481710B2/en) | 2016-06-10 | 2022-10-25 | OneTrust, LLC | Privacy management systems and methods |
| [US11494515B2 (en)](/patent/US11494515B2/en) | 2021-02-08 | 2022-11-08 | OneTrust, LLC | Data processing systems and methods for anonymizing data samples in classification analysis |
| [US11496510B1 (en)](/patent/US11496510B1/en) | 2018-08-24 | 2022-11-08 | NuRD LLC | Fully automated target identification of a phishing web site |
| [US11520928B2 (en)](/patent/US11520928B2/en) | 2016-06-10 | 2022-12-06 | OneTrust, LLC | Data processing systems for generating personal data receipts and related methods |
| [US11526624B2 (en)](/patent/US11526624B2/en) | 2020-09-21 | 2022-12-13 | OneTrust, LLC | Data processing systems and methods for automatically detecting target data transfers and target data processing |
| [US11533315B2 (en)](/patent/US11533315B2/en) | 2021-03-08 | 2022-12-20 | OneTrust, LLC | Data transfer discovery and analysis systems and related methods |
| [US11544667B2 (en)](/patent/US11544667B2/en) | 2016-06-10 | 2023-01-03 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US11544409B2 (en)](/patent/US11544409B2/en) | 2018-09-07 | 2023-01-03 | OneTrust, LLC | Data processing systems and methods for automatically protecting sensitive data within privacy management systems |
| [US11546661B2 (en)](/patent/US11546661B2/en) | 2021-02-18 | 2023-01-03 | OneTrust, LLC | Selective redaction of media content |
| [US11552969B2 (en)](/patent/US11552969B2/en) | 2018-12-19 | 2023-01-10 | Abnormal Security Corporation | Threat detection platforms for detecting, characterizing, and remediating email-based threats in real time |
| [US11563757B2 (en)](/patent/US11563757B2/en) | 2017-08-31 | 2023-01-24 | Barracuda Networks, Inc. | System and method for email account takeover detection and remediation utilizing AI models |
| [US11562097B2 (en)](/patent/US11562097B2/en) | 2016-06-10 | 2023-01-24 | OneTrust, LLC | Data processing systems for central consent repository and related methods |
| [US11562078B2 (en)](/patent/US11562078B2/en) | 2021-04-16 | 2023-01-24 | OneTrust, LLC | Assessing and managing computational risk involved with integrating third party computing functionality within a computing system |
| [US11570132B2 (en)](/patent/US11570132B2/en) | 2020-09-30 | 2023-01-31 | Qatar Foundation Foreducation, Science And Community Development | Systems and methods for encrypted message filtering |
| [US11568008B2 (en)](/patent/US11568008B2/en) | 2013-03-13 | 2023-01-31 | Plentyoffish Media Ulc | Apparatus, method and article to identify discrepancies between clients and in response prompt clients in a networked environment |
| [US11586700B2 (en)](/patent/US11586700B2/en) | 2016-06-10 | 2023-02-21 | OneTrust, LLC | Data processing systems and methods for automatically blocking the use of tracking tools |
| [US11586762B2 (en)](/patent/US11586762B2/en) | 2016-06-10 | 2023-02-21 | OneTrust, LLC | Data processing systems and methods for auditing data request compliance |
| [US11601464B2 (en)](/patent/US11601464B2/en) | 2021-02-10 | 2023-03-07 | OneTrust, LLC | Systems and methods for mitigating risks of third-party computing system functionality integration into a first-party computing system |
| [US11620142B1 (en)](/patent/US11620142B1/en) | 2022-06-03 | 2023-04-04 | OneTrust, LLC | Generating and customizing user interfaces for demonstrating functions of interactive user environments |
| [US11625502B2 (en)](/patent/US11625502B2/en) | 2016-06-10 | 2023-04-11 | OneTrust, LLC | Data processing systems for identifying and modifying processes that are subject to data subject access requests |
| [US11636171B2 (en)](/patent/US11636171B2/en) | 2016-06-10 | 2023-04-25 | OneTrust, LLC | Data processing user interface monitoring systems and related methods |
| [US11651104B2 (en)](/patent/US11651104B2/en) | 2016-06-10 | 2023-05-16 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US11651106B2 (en)](/patent/US11651106B2/en) | 2016-06-10 | 2023-05-16 | OneTrust, LLC | Data processing systems for fulfilling data subject access requests and related methods |
| [US11651402B2 (en)](/patent/US11651402B2/en) | 2016-04-01 | 2023-05-16 | OneTrust, LLC | Data processing systems and communication systems and methods for the efficient generation of risk assessments |
| [US11663303B2 (en)](/patent/US11663303B2/en) | 2020-03-02 | 2023-05-30 | Abnormal Security Corporation | Multichannel threat detection for protecting against account compromise |
| [US11665195B2 (en)](/patent/US11665195B2/en) | 2017-08-31 | 2023-05-30 | Barracuda Networks, Inc. | System and method for email account takeover detection and remediation utilizing anonymized datasets |
| [US11675929B2 (en)](/patent/US11675929B2/en) | 2016-06-10 | 2023-06-13 | OneTrust, LLC | Data processing consent sharing systems and related methods |
| [US11683284B2 (en)](/patent/US11683284B2/en) | 2020-10-23 | 2023-06-20 | Abnormal Security Corporation | Discovering graymail through real-time analysis of incoming email |
| [US11687528B2 (en)](/patent/US11687528B2/en) | 2021-01-25 | 2023-06-27 | OneTrust, LLC | Systems and methods for discovery, classification, and indexing of data in a native computing system |
| [US11687648B2 (en)](/patent/US11687648B2/en) | 2020-12-10 | 2023-06-27 | Abnormal Security Corporation | Deriving and surfacing insights regarding security threats |
| [US11722513B2 (en)](/patent/US11722513B2/en) | 2016-11-30 | 2023-08-08 | Agari Data, Inc. | Using a measure of influence of sender in determining a security risk associated with an electronic message |
| [US11727141B2 (en)](/patent/US11727141B2/en) | 2016-06-10 | 2023-08-15 | OneTrust, LLC | Data processing systems and methods for synching privacy-related user consent across multiple computing devices |
| [US11743294B2 (en)](/patent/US11743294B2/en) | 2018-12-19 | 2023-08-29 | Abnormal Security Corporation | Retrospective learning of communication patterns by machine learning models for discovering abnormal behavior |
| [US11757914B1 (en)](/patent/US11757914B1/en) | 2017-06-07 | 2023-09-12 | Agari Data, Inc. | Automated responsive message to determine a security risk of a message sender |
| [US11775348B2 (en)](/patent/US11775348B2/en) | 2021-02-17 | 2023-10-03 | OneTrust, LLC | Managing custom workflows for domain objects defined within microservices |
| [US11792224B2 (en)](/patent/US11792224B2/en) | 2021-05-26 | 2023-10-17 | Bank Of America Corporation | Information security system and method for phishing threat detection using tokens |
| [US11797528B2 (en)](/patent/US11797528B2/en) | 2020-07-08 | 2023-10-24 | OneTrust, LLC | Systems and methods for targeted data discovery |
| [EP4224351A4 (en)](/patent/EP4224351A4/en) \* | 2020-09-30 | 2023-11-01 | Fujitsu Limited | Verification method, verification program, and information processing device |
| [US11831661B2 (en)](/patent/US11831661B2/en) | 2021-06-03 | 2023-11-28 | Abnormal Security Corporation | Multi-tiered approach to payload detection for incoming communications |
| [US11936604B2 (en)](/patent/US11936604B2/en) | 2016-09-26 | 2024-03-19 | Agari Data, Inc. | Multi-level security analysis and intermediate delivery of an electronic message |
| [US11949713B2 (en)](/patent/US11949713B2/en) | 2020-03-02 | 2024-04-02 | Abnormal Security Corporation | Abuse mailbox for facilitating discovery, investigation, and analysis of email-based threats |
| [US12028373B2 (en)](/patent/US12028373B2/en) | 2021-04-14 | 2024-07-02 | Bank Of America Corporation | Information security system and method for preventing communications from detected phishing domains |
| [US12045266B2 (en)](/patent/US12045266B2/en) | 2016-06-10 | 2024-07-23 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US12052289B2 (en)](/patent/US12052289B2/en) | 2016-06-10 | 2024-07-30 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US12118121B2 (en)](/patent/US12118121B2/en) | 2016-06-10 | 2024-10-15 | OneTrust, LLC | Data subject access request processing systems and related methods |
| [US20240356969A1 (en)](/patent/US20240356969A1/en) \* | 2023-04-24 | 2024-10-24 | Cisco Technology, Inc. | Statistical modeling of email senders to detect business email compromise |
| [US12136055B2 (en)](/patent/US12136055B2/en) | 2016-06-10 | 2024-11-05 | OneTrust, LLC | Data processing systems for identifying, assessing, and remediating data processing risks using data modeling techniques |
| [US12153704B2 (en)](/patent/US12153704B2/en) | 2021-08-05 | 2024-11-26 | OneTrust, LLC | Computing platform for facilitating data exchange among computing environments |
| [US12255915B2 (en)](/patent/US12255915B2/en) | 2018-12-19 | 2025-03-18 | Abnormal Security Corporation | Programmatic discovery, retrieval, and analysis of communications to identify abnormal communication activity |
| [US12265896B2 (en)](/patent/US12265896B2/en) | 2020-10-05 | 2025-04-01 | OneTrust, LLC | Systems and methods for detecting prejudice bias in machine-learning models |
| [US12289304B2 (en)](/patent/US12289304B2/en) | 2021-05-26 | 2025-04-29 | Bank Of America Corporation | Information security system and method for phishing threat prevention using tokens |
| [US12299065B2 (en)](/patent/US12299065B2/en) | 2016-06-10 | 2025-05-13 | OneTrust, LLC | Data processing systems and methods for dynamically determining data processing consent configurations |
| [US12355716B2 (en)](/patent/US12355716B2/en) \* | 2023-11-13 | 2025-07-08 | Cisco Technology, Inc. | Detecting malicious email attachments using context-specific feature sets |
| [US12381915B2 (en)](/patent/US12381915B2/en) | 2016-06-10 | 2025-08-05 | OneTrust, LLC | Data processing systems and methods for performing assessments and monitoring of new versions of computer code for compliance |
| [US12506747B1 (en)](/patent/US12506747B1/en) | 2019-03-29 | 2025-12-23 | Agari Data, Inc. | Message campaign and malicious threat detection |
| [US20260052170A1 (en)](/patent/US20260052170A1/en) \* | 2024-08-13 | 2026-02-19 | Bank Of America Corporation | System and method for detection and prevention of computing device intrusion vectors using ai |
| [US12591828B2 (en)](/patent/US12591828B2/en) | 2016-06-10 | 2026-03-31 | OneTrust, LLC | Data processing systems for fulfilling data subject access requests and related methods |
| [US12688324B2 (en)](/patent/US12688324B2/en) | 2016-06-10 | 2026-07-21 | OneTrust, LLC | Data processing systems for webform crawling to map processing activities and related methods |

## Citations (4)

\* Cited by examiner, † Cited by third party

| Publication number | Priority date | Publication date | Assignee | Title |
| --- | --- | --- | --- | --- |
| [US20060123464A1 (en)](/patent/US20060123464A1/en) \* | 2004-12-02 | 2006-06-08 | Microsoft Corporation | Phishing detection, prevention, and notification |
| [US20060168066A1 (en)](/patent/US20060168066A1/en) \* | 2004-11-10 | 2006-07-27 | David Helsper | Email anti-phishing inspector |
| [US20070101423A1 (en)](/patent/US20070101423A1/en) \* | 2003-09-08 | 2007-05-03 | Mailfrontier, Inc. | Fraudulent message detection |
| [US20080133672A1 (en)](/patent/US20080133672A1/en) \* | 2006-12-01 | 2008-06-05 | Microsoft Corporation | Email safety determination |

* 2012
  + 2012-11-05
    US
    US13/668,349
    [patent/US8566938B1/en](/patent/US8566938B1/en)
    active
    Active

## Patent Citations (4)

\* Cited by examiner, † Cited by third party

| Publication number | Priority date | Publication date | Assignee | Title |
| --- | --- | --- | --- | --- |
| [US20070101423A1 (en)](/patent/US20070101423A1/en) \* | 2003-09-08 | 2007-05-03 | Mailfrontier, Inc. | Fraudulent message detection |
| [US20060168066A1 (en)](/patent/US20060168066A1/en) \* | 2004-11-10 | 2006-07-27 | David Helsper | Email anti-phishing inspector |
| [US20060123464A1 (en)](/patent/US20060123464A1/en) \* | 2004-12-02 | 2006-06-08 | Microsoft Corporation | Phishing detection, prevention, and notification |
| [US20080133672A1 (en)](/patent/US20080133672A1/en) \* | 2006-12-01 | 2008-06-05 | Microsoft Corporation | Email safety determination |

## Non-Patent Citations (1)

\* Cited by examiner, † Cited by third party

| Title |
| --- |
| Spoof Email Tutorial, eBay, 2006. \* |

## Cited By (371)

\* Cited by examiner, † Cited by third party

| Publication number | Priority date | Publication date | Assignee | Title |
| --- | --- | --- | --- | --- |
| [US9536221B2 (en)](/patent/US9536221B2/en) | 2008-06-19 | 2017-01-03 | Plentyoffish Media Ulc | System and method for adaptive matching of user profiles based on viewing and contact activity for social relationship services |
| [US10129194B1 (en)](/patent/US10129194B1/en) | 2012-02-13 | 2018-11-13 | ZapFraud, Inc. | Tertiary classification of communications |
| [US9473437B1 (en)](/patent/US9473437B1/en) \* | 2012-02-13 | 2016-10-18 | ZapFraud, Inc. | Tertiary classification of communications |
| [US10581780B1 (en)](/patent/US10581780B1/en) | 2012-02-13 | 2020-03-03 | ZapFraud, Inc. | Tertiary classification of communications |
| [US10129195B1 (en)](/patent/US10129195B1/en) | 2012-02-13 | 2018-11-13 | ZapFraud, Inc. | Tertiary classification of communications |
| [US10171475B2 (en)](/patent/US10171475B2/en) | 2012-07-16 | 2019-01-01 | Mcafee, Llc | Cloud email message scanning with local policy application in a network environment |
| [US20140020047A1 (en)](/patent/US20140020047A1/en) \* | 2012-07-16 | 2014-01-16 | Nicholas Liebmann | Cloud email message scanning with local policy application in a network environment |
| [US9049235B2 (en)](/patent/US9049235B2/en) \* | 2012-07-16 | 2015-06-02 | Mcafee, Inc. | Cloud email message scanning with local policy application in a network environment |
| [US9705889B2 (en)](/patent/US9705889B2/en) | 2012-07-16 | 2017-07-11 | Mcafee, Inc. | Cloud email message scanning with local policy application in a network environment |
| [US10769221B1 (en)](/patent/US10769221B1/en) | 2012-08-20 | 2020-09-08 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate matching of clients in a networked environment |
| [US11908001B2 (en)](/patent/US11908001B2/en) | 2012-08-20 | 2024-02-20 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate matching of clients in a networked environment |
| [US9143476B2 (en)](/patent/US9143476B2/en) \* | 2012-09-14 | 2015-09-22 | Return Path, Inc. | Real-time classification of email message traffic |
| [US20140082726A1 (en)](/patent/US20140082726A1/en) \* | 2012-09-14 | 2014-03-20 | Return Path, Inc. | Real-time classification of email message traffic |
| [US8839369B1 (en)](/patent/US8839369B1/en) \* | 2012-11-09 | 2014-09-16 | Trend Micro Incorporated | Methods and systems for detecting email phishing attacks |
| [US9679259B1 (en)](/patent/US9679259B1/en) | 2013-01-25 | 2017-06-13 | Plentyoffish Media Ulc | Systems and methods for training and employing a machine learning system in evaluating entity pairs |
| [US9674221B1 (en)](/patent/US9674221B1/en) | 2013-02-08 | 2017-06-06 | PhishMe, Inc. | Collaborative phishing attack detection |
| [US20140230060A1 (en)](/patent/US20140230060A1/en) \* | 2013-02-08 | 2014-08-14 | PhishMe, Inc. | Collaborative phishing attack detection |
| [US10819744B1 (en)](/patent/US10819744B1/en) | 2013-02-08 | 2020-10-27 | Cofense Inc | Collaborative phishing attack detection |
| [US9398038B2 (en)](/patent/US9398038B2/en) \* | 2013-02-08 | 2016-07-19 | PhishMe, Inc. | Collaborative phishing attack detection |
| [US9591017B1 (en)](/patent/US9591017B1/en) \* | 2013-02-08 | 2017-03-07 | PhishMe, Inc. | Collaborative phishing attack detection |
| [US9667645B1 (en)](/patent/US9667645B1/en) | 2013-02-08 | 2017-05-30 | PhishMe, Inc. | Performance benchmarking for simulated phishing attacks |
| [US10187407B1 (en)](/patent/US10187407B1/en) | 2013-02-08 | 2019-01-22 | Cofense Inc. | Collaborative phishing attack detection |
| [US11568008B2 (en)](/patent/US11568008B2/en) | 2013-03-13 | 2023-01-31 | Plentyoffish Media Ulc | Apparatus, method and article to identify discrepancies between clients and in response prompt clients in a networked environment |
| [US11175808B2 (en)](/patent/US11175808B2/en) | 2013-07-23 | 2021-11-16 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate matching of clients in a networked environment |
| [US9672289B1 (en)](/patent/US9672289B1/en) | 2013-07-23 | 2017-06-06 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate matching of clients in a networked environment |
| [US11747971B2 (en)](/patent/US11747971B2/en) | 2013-07-23 | 2023-09-05 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate matching of clients in a networked environment |
| [US9141790B2 (en)](/patent/US9141790B2/en) | 2013-09-10 | 2015-09-22 | Symantec Corporation | Systems and methods for using event-correlation graphs to detect attacks on computing systems |
| [US10277628B1 (en)](/patent/US10277628B1/en) | 2013-09-16 | 2019-04-30 | ZapFraud, Inc. | Detecting phishing attempts |
| [US11729211B2 (en)](/patent/US11729211B2/en) | 2013-09-16 | 2023-08-15 | ZapFraud, Inc. | Detecting phishing attempts |
| [US10609073B2 (en)](/patent/US10609073B2/en) | 2013-09-16 | 2020-03-31 | ZapFraud, Inc. | Detecting phishing attempts |
| [US12261883B2 (en)](/patent/US12261883B2/en) | 2013-09-16 | 2025-03-25 | ZapFraud, Inc. | Detecting phishing attempts |
| [US9166997B1 (en)](/patent/US9166997B1/en) | 2013-09-19 | 2015-10-20 | Symantec Corporation | Systems and methods for reducing false positives when using event-correlation graphs to detect attacks on computing systems |
| [US11005989B1 (en)](/patent/US11005989B1/en) | 2013-11-07 | 2021-05-11 | Rightquestion, Llc | Validating automatic number identification data |
| [US10694029B1 (en)](/patent/US10694029B1/en) | 2013-11-07 | 2020-06-23 | Rightquestion, Llc | Validating automatic number identification data |
| [US11856132B2 (en)](/patent/US11856132B2/en) | 2013-11-07 | 2023-12-26 | Rightquestion, Llc | Validating automatic number identification data |
| [US10674009B1 (en)](/patent/US10674009B1/en) | 2013-11-07 | 2020-06-02 | Rightquestion, Llc | Validating automatic number identification data |
| [US12238243B2 (en)](/patent/US12238243B2/en) | 2013-11-07 | 2025-02-25 | Rightquestion, Llc | Validating automatic number identification data |
| [US11949747B2 (en)](/patent/US11949747B2/en) | 2013-12-04 | 2024-04-02 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate automatic detection and removal of fraudulent user information in a network environment |
| [US12373552B2 (en)](/patent/US12373552B2/en) | 2013-12-04 | 2025-07-29 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate automatic detection and removal of fraudulent user information in a network environment |
| [US10637959B2 (en)](/patent/US10637959B2/en) | 2013-12-04 | 2020-04-28 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate automatic detection and removal of fraudulent user information in a network environment |
| [US9870465B1 (en)](/patent/US9870465B1/en) | 2013-12-04 | 2018-01-16 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate automatic detection and removal of fraudulent user information in a network environment |
| [US11546433B2 (en)](/patent/US11546433B2/en) | 2013-12-04 | 2023-01-03 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate automatic detection and removal of fraudulent user information in a network environment |
| [US10277710B2 (en)](/patent/US10277710B2/en) | 2013-12-04 | 2019-04-30 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate automatic detection and removal of fraudulent user information in a network environment |
| [US10540607B1 (en)](/patent/US10540607B1/en) | 2013-12-10 | 2020-01-21 | Plentyoffish Media Ulc | Apparatus, method and article to effect electronic message reply rate matching in a network environment |
| [US9148441B1 (en)](/patent/US9148441B1/en) | 2013-12-23 | 2015-09-29 | Symantec Corporation | Systems and methods for adjusting suspiciousness scores in event-correlation graphs |
| [US10108968B1 (en)](/patent/US10108968B1/en) | 2014-03-05 | 2018-10-23 | Plentyoffish Media Ulc | Apparatus, method and article to facilitate automatic detection and removal of fraudulent advertising accounts in a network environment |
| [US9256739B1 (en)](/patent/US9256739B1/en) \* | 2014-03-21 | 2016-02-09 | Symantec Corporation | Systems and methods for using event-correlation graphs to generate remediation procedures |
| [US10387795B1 (en)](/patent/US10387795B1/en) | 2014-04-02 | 2019-08-20 | Plentyoffish Media Inc. | Systems and methods for training and employing a machine learning system in providing service level upgrade offers |
| [US9836533B1 (en)](/patent/US9836533B1/en) | 2014-04-07 | 2017-12-05 | Plentyoffish Media Ulc | Apparatus, method and article to effect user interest-based matching in a network environment |
| [US9720977B2 (en)](/patent/US9720977B2/en) \* | 2014-06-10 | 2017-08-01 | International Business Machines Corporation | Weighting search criteria based on similarities to an ingested corpus in a question and answer (QA) system |
| [US9715531B2 (en)](/patent/US9715531B2/en) \* | 2014-06-10 | 2017-07-25 | International Business Machines Corporation | Weighting search criteria based on similarities to an ingested corpus in a question and answer (QA) system |
| [US20160224566A1 (en)](/patent/US20160224566A1/en) \* | 2014-06-10 | 2016-08-04 | International Business Machines Corporation | Weighting Search Criteria Based on Similarities to an Ingested Corpus in a Question and Answer (QA) System |
| [US20150356089A1 (en)](/patent/US20150356089A1/en) \* | 2014-06-10 | 2015-12-10 | International Business Machines Corporation | Weighting Search Criteria Based on Similarities to an Ingested Corpus in a Question and Answer (QA) System |
| [US10432720B1 (en)](/patent/US10432720B1/en) | 2014-06-25 | 2019-10-01 | Symantec Corporation | Systems and methods for strong information about transmission control protocol connections |
| [US9843594B1 (en)](/patent/US9843594B1/en) | 2014-10-28 | 2017-12-12 | Symantec Corporation | Systems and methods for detecting anomalous messages in automobile networks |
| [US9398047B2 (en)](/patent/US9398047B2/en) | 2014-11-17 | 2016-07-19 | Vade Retro Technology, Inc. | Methods and systems for phishing detection |
| [US10146893B1 (en)](/patent/US10146893B1/en) | 2015-03-27 | 2018-12-04 | Symantec Corporation | Systems and methods for evaluating electronic control units within vehicle emulations |
| [US9906539B2 (en)](/patent/US9906539B2/en) | 2015-04-10 | 2018-02-27 | PhishMe, Inc. | Suspicious message processing and incident response |
| [US9906554B2 (en)](/patent/US9906554B2/en) | 2015-04-10 | 2018-02-27 | PhishMe, Inc. | Suspicious message processing and incident response |
| [US9596265B2 (en)](/patent/US9596265B2/en) | 2015-05-13 | 2017-03-14 | Google Inc. | Identifying phishing communications using templates |
| [US9756073B2 (en)](/patent/US9756073B2/en) | 2015-05-13 | 2017-09-05 | Google Inc. | Identifying phishing communications using templates |
| [WO2016183358A1 (en)](/patent/WO2016183358A1/en) \* | 2015-05-13 | 2016-11-17 | Google Inc. | Identifying phishing communications using templates |
| [EP3706391A1 (en)](/patent/EP3706391A1/en) \* | 2015-05-13 | 2020-09-09 | Google LLC | Identifying phishing communications using templates |
| [US9825986B1 (en)](/patent/US9825986B1/en) | 2015-06-29 | 2017-11-21 | Symantec Corporation | Systems and methods for generating contextually meaningful animated visualizations of computer security events |
| [US10764327B2 (en)](/patent/US10764327B2/en) \* | 2015-07-14 | 2020-09-01 | China Internet Network Information Center | E-mail anti-phishing system and method |
| [US20180212994A1 (en)](/patent/US20180212994A1/en) \* | 2015-07-14 | 2018-07-26 | China Internet Network Information Center | E-mail anti-phishing system and method |
| [WO2017019716A1 (en)](/patent/WO2017019716A1/en) \* | 2015-07-30 | 2017-02-02 | Microsoft Technology Licensing, Llc | Third party email signature generation and authentication |
| [US10116609B2 (en)](/patent/US10116609B2/en) | 2015-07-30 | 2018-10-30 | Microsoft Technology Licensing, Llc | Third party email signature generation and authentication |
| [CN105072137A (en)](/patent/CN105072137A/en) \* | 2015-09-15 | 2015-11-18 | 蔡丝英 | Spear phishing mail detection method and device |
| [US9967274B2 (en)](/patent/US9967274B2/en) | 2015-11-25 | 2018-05-08 | Symantec Corporation | Systems and methods for identifying compromised devices within industrial control systems |
| [US11595336B2 (en)](/patent/US11595336B2/en) | 2016-01-26 | 2023-02-28 | ZapFraud, Inc. | Detecting of business email compromise |
| [US10721195B2 (en)](/patent/US10721195B2/en) | 2016-01-26 | 2020-07-21 | ZapFraud, Inc. | Detection of business email compromise |
| [US10104100B1 (en)](/patent/US10104100B1/en) | 2016-03-03 | 2018-10-16 | Symantec Corporation | Systems and methods for detecting anomalies that are potentially indicative of malicious attacks |
| [US11651402B2 (en)](/patent/US11651402B2/en) | 2016-04-01 | 2023-05-16 | OneTrust, LLC | Data processing systems and communication systems and methods for the efficient generation of risk assessments |
| [US10956952B2 (en)](/patent/US10956952B2/en) | 2016-04-01 | 2021-03-23 | OneTrust, LLC | Data processing systems and communication systems and methods for the efficient generation of privacy risk assessments |
| [US11004125B2 (en)](/patent/US11004125B2/en) | 2016-04-01 | 2021-05-11 | OneTrust, LLC | Data processing systems and methods for integrating privacy information management systems with data loss prevention tools or other tools for privacy design |
| [US11244367B2 (en)](/patent/US11244367B2/en) | 2016-04-01 | 2022-02-08 | OneTrust, LLC | Data processing systems and methods for integrating privacy information management systems with data loss prevention tools or other tools for privacy design |
| [US12288233B2 (en)](/patent/US12288233B2/en) | 2016-04-01 | 2025-04-29 | OneTrust, LLC | Data processing systems and methods for integrating privacy information management systems with data loss prevention tools or other tools for privacy design |
| [US10193903B1 (en)](/patent/US10193903B1/en) | 2016-04-29 | 2019-01-29 | Symantec Corporation | Systems and methods for detecting suspicious microcontroller messages |
| [US10069856B2 (en)](/patent/US10069856B2/en) | 2016-05-13 | 2018-09-04 | King Abdulaziz City For Science And Technology | System and method of comparative evaluation for phishing mitigation |
| [CN107402936A (en)](/patent/CN107402936A/en) \* | 2016-05-20 | 2017-11-28 | 阿里巴巴集团控股有限公司 | information identifying method and device |
| [US11651104B2 (en)](/patent/US11651104B2/en) | 2016-06-10 | 2023-05-16 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US11461500B2 (en)](/patent/US11461500B2/en) | 2016-06-10 | 2022-10-04 | OneTrust, LLC | Data processing systems for cookie compliance testing with website scanning and related methods |
| [US12694044B2 (en)](/patent/US12694044B2/en) | 2016-06-10 | 2026-07-28 | OneTrust, LLC | Data processing systems and methods for automatically detecting and documenting privacy-related aspects of computer software |
| [US12688324B2 (en)](/patent/US12688324B2/en) | 2016-06-10 | 2026-07-21 | OneTrust, LLC | Data processing systems for webform crawling to map processing activities and related methods |
| [US12609938B2 (en)](/patent/US12609938B2/en) | 2016-06-10 | 2026-04-21 | One Trust, LLC | Consent conversion optimization systems and related methods |
| [US12591828B2 (en)](/patent/US12591828B2/en) | 2016-06-10 | 2026-03-31 | OneTrust, LLC | Data processing systems for fulfilling data subject access requests and related methods |
| [US12412140B2 (en)](/patent/US12412140B2/en) | 2016-06-10 | 2025-09-09 | OneTrust, LLC | Data processing systems and methods for bundled privacy policies |
| [US12381915B2 (en)](/patent/US12381915B2/en) | 2016-06-10 | 2025-08-05 | OneTrust, LLC | Data processing systems and methods for performing assessments and monitoring of new versions of computer code for compliance |
| [US12299065B2 (en)](/patent/US12299065B2/en) | 2016-06-10 | 2025-05-13 | OneTrust, LLC | Data processing systems and methods for dynamically determining data processing consent configurations |
| [US12216794B2 (en)](/patent/US12216794B2/en) | 2016-06-10 | 2025-02-04 | OneTrust, LLC | Data processing systems and methods for synching privacy-related user consent across multiple computing devices |
| [US12204564B2 (en)](/patent/US12204564B2/en) | 2016-06-10 | 2025-01-21 | OneTrust, LLC | Data processing systems and methods for automatically detecting and documenting privacy-related aspects of computer software |
| [US12190330B2 (en)](/patent/US12190330B2/en) | 2016-06-10 | 2025-01-07 | OneTrust, LLC | Data processing systems for identity validation for consumer rights requests and related methods |
| [US12164667B2 (en)](/patent/US12164667B2/en) | 2016-06-10 | 2024-12-10 | OneTrust, LLC | Application privacy scanning systems and related methods |
| [US12158975B2 (en)](/patent/US12158975B2/en) | 2016-06-10 | 2024-12-03 | OneTrust, LLC | Data processing consent sharing systems and related methods |
| [US12147578B2 (en)](/patent/US12147578B2/en) | 2016-06-10 | 2024-11-19 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US10929559B2 (en)](/patent/US10929559B2/en) | 2016-06-10 | 2021-02-23 | OneTrust, LLC | Data processing systems for data testing to confirm data deletion and related methods |
| [US12136055B2 (en)](/patent/US12136055B2/en) | 2016-06-10 | 2024-11-05 | OneTrust, LLC | Data processing systems for identifying, assessing, and remediating data processing risks using data modeling techniques |
| [US10949544B2 (en)](/patent/US10949544B2/en) | 2016-06-10 | 2021-03-16 | OneTrust, LLC | Data processing systems for data transfer risk identification and related methods |
| [US10949170B2 (en)](/patent/US10949170B2/en) | 2016-06-10 | 2021-03-16 | OneTrust, LLC | Data processing systems for integration of consumer feedback with data subject access requests and related methods |
| [US10949565B2 (en)](/patent/US10949565B2/en) | 2016-06-10 | 2021-03-16 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US10949567B2 (en)](/patent/US10949567B2/en) | 2016-06-10 | 2021-03-16 | OneTrust, LLC | Data processing systems for fulfilling data subject access requests and related methods |
| [US12118121B2 (en)](/patent/US12118121B2/en) | 2016-06-10 | 2024-10-15 | OneTrust, LLC | Data subject access request processing systems and related methods |
| [US12086748B2 (en)](/patent/US12086748B2/en) | 2016-06-10 | 2024-09-10 | OneTrust, LLC | Data processing systems for assessing readiness for responding to privacy-related incidents |
| [US10970675B2 (en)](/patent/US10970675B2/en) | 2016-06-10 | 2021-04-06 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US10970371B2 (en)](/patent/US10970371B2/en) | 2016-06-10 | 2021-04-06 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US10972509B2 (en)](/patent/US10972509B2/en) | 2016-06-10 | 2021-04-06 | OneTrust, LLC | Data processing and scanning systems for generating and populating a data inventory |
| [US10984132B2 (en)](/patent/US10984132B2/en) | 2016-06-10 | 2021-04-20 | OneTrust, LLC | Data processing systems and methods for populating and maintaining a centralized database of personal data |
| [US12052289B2 (en)](/patent/US12052289B2/en) | 2016-06-10 | 2024-07-30 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US10997315B2 (en)](/patent/US10997315B2/en) | 2016-06-10 | 2021-05-04 | OneTrust, LLC | Data processing systems for fulfilling data subject access requests and related methods |
| [US10997318B2 (en)](/patent/US10997318B2/en) | 2016-06-10 | 2021-05-04 | OneTrust, LLC | Data processing systems for generating and populating a data inventory for processing data access requests |
| [US10997542B2 (en)](/patent/US10997542B2/en) | 2016-06-10 | 2021-05-04 | OneTrust, LLC | Privacy management systems and methods |
| [US12045266B2 (en)](/patent/US12045266B2/en) | 2016-06-10 | 2024-07-23 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US12026651B2 (en)](/patent/US12026651B2/en) | 2016-06-10 | 2024-07-02 | OneTrust, LLC | Data processing systems and methods for providing training in a vendor procurement process |
| [US11960564B2 (en)](/patent/US11960564B2/en) | 2016-06-10 | 2024-04-16 | OneTrust, LLC | Data processing systems and methods for automatically blocking the use of tracking tools |
| [US11023616B2 (en)](/patent/US11023616B2/en) | 2016-06-10 | 2021-06-01 | OneTrust, LLC | Data processing systems for identifying, assessing, and remediating data processing risks using data modeling techniques |
| [US11023842B2 (en)](/patent/US11023842B2/en) | 2016-06-10 | 2021-06-01 | OneTrust, LLC | Data processing systems and methods for bundled privacy policies |
| [US11921894B2 (en)](/patent/US11921894B2/en) | 2016-06-10 | 2024-03-05 | OneTrust, LLC | Data processing systems for generating and populating a data inventory for processing data access requests |
| [US11025675B2 (en)](/patent/US11025675B2/en) | 2016-06-10 | 2021-06-01 | OneTrust, LLC | Data processing systems and methods for performing privacy assessments and monitoring of new versions of computer code for privacy compliance |
| [US11030327B2 (en)](/patent/US11030327B2/en) | 2016-06-10 | 2021-06-08 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11030274B2 (en)](/patent/US11030274B2/en) | 2016-06-10 | 2021-06-08 | OneTrust, LLC | Data processing user interface monitoring systems and related methods |
| [US11030563B2 (en)](/patent/US11030563B2/en) | 2016-06-10 | 2021-06-08 | OneTrust, LLC | Privacy management systems and methods |
| [US11036882B2 (en)](/patent/US11036882B2/en) | 2016-06-10 | 2021-06-15 | OneTrust, LLC | Data processing systems for processing and managing data subject access in a distributed environment |
| [US11038925B2 (en)](/patent/US11038925B2/en) | 2016-06-10 | 2021-06-15 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11036771B2 (en)](/patent/US11036771B2/en) | 2016-06-10 | 2021-06-15 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US11036674B2 (en)](/patent/US11036674B2/en) | 2016-06-10 | 2021-06-15 | OneTrust, LLC | Data processing systems for processing data subject access requests |
| [US11868507B2 (en)](/patent/US11868507B2/en) | 2016-06-10 | 2024-01-09 | OneTrust, LLC | Data processing systems for cookie compliance testing with website scanning and related methods |
| [US11847182B2 (en)](/patent/US11847182B2/en) | 2016-06-10 | 2023-12-19 | OneTrust, LLC | Data processing consent capture systems and related methods |
| [US11057356B2 (en)](/patent/US11057356B2/en) | 2016-06-10 | 2021-07-06 | OneTrust, LLC | Automated data processing systems and methods for automatically processing data subject access requests using a chatbot |
| [US11062051B2 (en)](/patent/US11062051B2/en) | 2016-06-10 | 2021-07-13 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US11070593B2 (en)](/patent/US11070593B2/en) | 2016-06-10 | 2021-07-20 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11068618B2 (en)](/patent/US11068618B2/en) | 2016-06-10 | 2021-07-20 | OneTrust, LLC | Data processing systems for central consent repository and related methods |
| [US11074367B2 (en)](/patent/US11074367B2/en) | 2016-06-10 | 2021-07-27 | OneTrust, LLC | Data processing systems for identity validation for consumer rights requests and related methods |
| [US11087260B2 (en)](/patent/US11087260B2/en) | 2016-06-10 | 2021-08-10 | OneTrust, LLC | Data processing systems and methods for customizing privacy training |
| [US11100444B2 (en)](/patent/US11100444B2/en) | 2016-06-10 | 2021-08-24 | OneTrust, LLC | Data processing systems and methods for providing training in a vendor procurement process |
| [US11100445B2 (en)](/patent/US11100445B2/en) | 2016-06-10 | 2021-08-24 | OneTrust, LLC | Data processing systems for assessing readiness for responding to privacy-related incidents |
| [US11727141B2 (en)](/patent/US11727141B2/en) | 2016-06-10 | 2023-08-15 | OneTrust, LLC | Data processing systems and methods for synching privacy-related user consent across multiple computing devices |
| [US11113416B2 (en)](/patent/US11113416B2/en) | 2016-06-10 | 2021-09-07 | OneTrust, LLC | Application privacy scanning systems and related methods |
| [US11122011B2 (en)](/patent/US11122011B2/en) | 2016-06-10 | 2021-09-14 | OneTrust, LLC | Data processing systems and methods for using a data model to select a target data asset in a data migration |
| [US11120162B2 (en)](/patent/US11120162B2/en) | 2016-06-10 | 2021-09-14 | OneTrust, LLC | Data processing systems for data testing to confirm data deletion and related methods |
| [US11120161B2 (en)](/patent/US11120161B2/en) | 2016-06-10 | 2021-09-14 | OneTrust, LLC | Data subject access request processing systems and related methods |
| [US11126748B2 (en)](/patent/US11126748B2/en) | 2016-06-10 | 2021-09-21 | OneTrust, LLC | Data processing consent management systems and related methods |
| [US11675929B2 (en)](/patent/US11675929B2/en) | 2016-06-10 | 2023-06-13 | OneTrust, LLC | Data processing consent sharing systems and related methods |
| [US11651106B2 (en)](/patent/US11651106B2/en) | 2016-06-10 | 2023-05-16 | OneTrust, LLC | Data processing systems for fulfilling data subject access requests and related methods |
| [US11134086B2 (en)](/patent/US11134086B2/en) | 2016-06-10 | 2021-09-28 | OneTrust, LLC | Consent conversion optimization systems and related methods |
| [US11138242B2 (en)](/patent/US11138242B2/en) | 2016-06-10 | 2021-10-05 | OneTrust, LLC | Data processing systems and methods for automatically detecting and documenting privacy-related aspects of computer software |
| [US11138299B2 (en)](/patent/US11138299B2/en) | 2016-06-10 | 2021-10-05 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11138336B2 (en)](/patent/US11138336B2/en) | 2016-06-10 | 2021-10-05 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US11138318B2 (en)](/patent/US11138318B2/en) | 2016-06-10 | 2021-10-05 | OneTrust, LLC | Data processing systems for data transfer risk identification and related methods |
| [US11645418B2 (en)](/patent/US11645418B2/en) | 2016-06-10 | 2023-05-09 | OneTrust, LLC | Data processing systems for data testing to confirm data deletion and related methods |
| [US11144670B2 (en)](/patent/US11144670B2/en) | 2016-06-10 | 2021-10-12 | OneTrust, LLC | Data processing systems for identifying and modifying processes that are subject to data subject access requests |
| [US11146566B2 (en)](/patent/US11146566B2/en) | 2016-06-10 | 2021-10-12 | OneTrust, LLC | Data processing systems for fulfilling data subject access requests and related methods |
| [US11144622B2 (en)](/patent/US11144622B2/en) | 2016-06-10 | 2021-10-12 | OneTrust, LLC | Privacy management systems and methods |
| [US11151233B2 (en)](/patent/US11151233B2/en) | 2016-06-10 | 2021-10-19 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11645353B2 (en)](/patent/US11645353B2/en) | 2016-06-10 | 2023-05-09 | OneTrust, LLC | Data processing consent capture systems and related methods |
| [US11157600B2 (en)](/patent/US11157600B2/en) | 2016-06-10 | 2021-10-26 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11636171B2 (en)](/patent/US11636171B2/en) | 2016-06-10 | 2023-04-25 | OneTrust, LLC | Data processing user interface monitoring systems and related methods |
| [US11625502B2 (en)](/patent/US11625502B2/en) | 2016-06-10 | 2023-04-11 | OneTrust, LLC | Data processing systems for identifying and modifying processes that are subject to data subject access requests |
| [US11609939B2 (en)](/patent/US11609939B2/en) | 2016-06-10 | 2023-03-21 | OneTrust, LLC | Data processing systems and methods for automatically detecting and documenting privacy-related aspects of computer software |
| [US11586762B2 (en)](/patent/US11586762B2/en) | 2016-06-10 | 2023-02-21 | OneTrust, LLC | Data processing systems and methods for auditing data request compliance |
| [US11586700B2 (en)](/patent/US11586700B2/en) | 2016-06-10 | 2023-02-21 | OneTrust, LLC | Data processing systems and methods for automatically blocking the use of tracking tools |
| [US11182501B2 (en)](/patent/US11182501B2/en) | 2016-06-10 | 2021-11-23 | OneTrust, LLC | Data processing systems for fulfilling data subject access requests and related methods |
| [US11562097B2 (en)](/patent/US11562097B2/en) | 2016-06-10 | 2023-01-24 | OneTrust, LLC | Data processing systems for central consent repository and related methods |
| [US11188615B2 (en)](/patent/US11188615B2/en) | 2016-06-10 | 2021-11-30 | OneTrust, LLC | Data processing consent capture systems and related methods |
| [US11188862B2 (en)](/patent/US11188862B2/en) | 2016-06-10 | 2021-11-30 | OneTrust, LLC | Privacy management systems and methods |
| [US11195134B2 (en)](/patent/US11195134B2/en) | 2016-06-10 | 2021-12-07 | OneTrust, LLC | Privacy management systems and methods |
| [US11200341B2 (en)](/patent/US11200341B2/en) | 2016-06-10 | 2021-12-14 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US11210420B2 (en)](/patent/US11210420B2/en) | 2016-06-10 | 2021-12-28 | OneTrust, LLC | Data subject access request processing systems and related methods |
| [US11222139B2 (en)](/patent/US11222139B2/en) | 2016-06-10 | 2022-01-11 | OneTrust, LLC | Data processing systems and methods for automatic discovery and assessment of mobile software development kits |
| [US11222309B2 (en)](/patent/US11222309B2/en) | 2016-06-10 | 2022-01-11 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US11222142B2 (en)](/patent/US11222142B2/en) | 2016-06-10 | 2022-01-11 | OneTrust, LLC | Data processing systems for validating authorization for personal data collection, storage, and processing |
| [US11228620B2 (en)](/patent/US11228620B2/en) | 2016-06-10 | 2022-01-18 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11227247B2 (en)](/patent/US11227247B2/en) | 2016-06-10 | 2022-01-18 | OneTrust, LLC | Data processing systems and methods for bundled privacy policies |
| [US11238390B2 (en)](/patent/US11238390B2/en) | 2016-06-10 | 2022-02-01 | OneTrust, LLC | Privacy management systems and methods |
| [US11240273B2 (en)](/patent/US11240273B2/en) | 2016-06-10 | 2022-02-01 | OneTrust, LLC | Data processing and scanning systems for generating and populating a data inventory |
| [US11244071B2 (en)](/patent/US11244071B2/en) \* | 2016-06-10 | 2022-02-08 | OneTrust, LLC | Data processing systems for use in automatically generating, populating, and submitting data subject access requests |
| [US11244072B2 (en)](/patent/US11244072B2/en) | 2016-06-10 | 2022-02-08 | OneTrust, LLC | Data processing systems for identifying, assessing, and remediating data processing risks using data modeling techniques |
| [US11558429B2 (en)](/patent/US11558429B2/en) | 2016-06-10 | 2023-01-17 | OneTrust, LLC | Data processing and scanning systems for generating and populating a data inventory |
| [US11256777B2 (en)](/patent/US11256777B2/en) | 2016-06-10 | 2022-02-22 | OneTrust, LLC | Data processing user interface monitoring systems and related methods |
| [US11277448B2 (en)](/patent/US11277448B2/en) | 2016-06-10 | 2022-03-15 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11294939B2 (en)](/patent/US11294939B2/en) | 2016-06-10 | 2022-04-05 | OneTrust, LLC | Data processing systems and methods for automatically detecting and documenting privacy-related aspects of computer software |
| [US11295316B2 (en)](/patent/US11295316B2/en) | 2016-06-10 | 2022-04-05 | OneTrust, LLC | Data processing systems for identity validation for consumer rights requests and related methods |
| [US11556672B2 (en)](/patent/US11556672B2/en) | 2016-06-10 | 2023-01-17 | OneTrust, LLC | Data processing systems for verification of consent and notice processing and related methods |
| [US11301589B2 (en)](/patent/US11301589B2/en) | 2016-06-10 | 2022-04-12 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US11301796B2 (en)](/patent/US11301796B2/en) | 2016-06-10 | 2022-04-12 | OneTrust, LLC | Data processing systems and methods for customizing privacy training |
| [US11308435B2 (en)](/patent/US11308435B2/en) | 2016-06-10 | 2022-04-19 | OneTrust, LLC | Data processing systems for identifying, assessing, and remediating data processing risks using data modeling techniques |
| [US11328240B2 (en)](/patent/US11328240B2/en) | 2016-06-10 | 2022-05-10 | OneTrust, LLC | Data processing systems for assessing readiness for responding to privacy-related incidents |
| [US11328092B2 (en)](/patent/US11328092B2/en) | 2016-06-10 | 2022-05-10 | OneTrust, LLC | Data processing systems for processing and managing data subject access in a distributed environment |
| [US11334681B2 (en)](/patent/US11334681B2/en) | 2016-06-10 | 2022-05-17 | OneTrust, LLC | Application privacy scanning systems and related meihods |
| [US11334682B2 (en)](/patent/US11334682B2/en) | 2016-06-10 | 2022-05-17 | OneTrust, LLC | Data subject access request processing systems and related methods |
| [US11336697B2 (en)](/patent/US11336697B2/en) | 2016-06-10 | 2022-05-17 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11341447B2 (en)](/patent/US11341447B2/en) | 2016-06-10 | 2022-05-24 | OneTrust, LLC | Privacy management systems and methods |
| [US11343284B2 (en)](/patent/US11343284B2/en) | 2016-06-10 | 2022-05-24 | OneTrust, LLC | Data processing systems and methods for performing privacy assessments and monitoring of new versions of computer code for privacy compliance |
| [US11347889B2 (en)](/patent/US11347889B2/en) | 2016-06-10 | 2022-05-31 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US11354435B2 (en)](/patent/US11354435B2/en) | 2016-06-10 | 2022-06-07 | OneTrust, LLC | Data processing systems for data testing to confirm data deletion and related methods |
| [US11354434B2 (en)](/patent/US11354434B2/en) | 2016-06-10 | 2022-06-07 | OneTrust, LLC | Data processing systems for verification of consent and notice processing and related methods |
| [US11361057B2 (en)](/patent/US11361057B2/en) | 2016-06-10 | 2022-06-14 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US11366909B2 (en)](/patent/US11366909B2/en) | 2016-06-10 | 2022-06-21 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11366786B2 (en)](/patent/US11366786B2/en) | 2016-06-10 | 2022-06-21 | OneTrust, LLC | Data processing systems for processing data subject access requests |
| [US11550897B2 (en)](/patent/US11550897B2/en) | 2016-06-10 | 2023-01-10 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11392720B2 (en)](/patent/US11392720B2/en) | 2016-06-10 | 2022-07-19 | OneTrust, LLC | Data processing systems for verification of consent and notice processing and related methods |
| [US11551174B2 (en)](/patent/US11551174B2/en) | 2016-06-10 | 2023-01-10 | OneTrust, LLC | Privacy management systems and methods |
| [US11403377B2 (en)](/patent/US11403377B2/en) | 2016-06-10 | 2022-08-02 | OneTrust, LLC | Privacy management systems and methods |
| [US11409908B2 (en)](/patent/US11409908B2/en) | 2016-06-10 | 2022-08-09 | OneTrust, LLC | Data processing systems and methods for populating and maintaining a centralized database of personal data |
| [US11410106B2 (en)](/patent/US11410106B2/en) | 2016-06-10 | 2022-08-09 | OneTrust, LLC | Privacy management systems and methods |
| [US11544405B2 (en)](/patent/US11544405B2/en) | 2016-06-10 | 2023-01-03 | OneTrust, LLC | Data processing systems for verification of consent and notice processing and related methods |
| [US11418492B2 (en)](/patent/US11418492B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Data processing systems and methods for using a data model to select a target data asset in a data migration |
| [US11416636B2 (en)](/patent/US11416636B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Data processing consent management systems and related methods |
| [US11416798B2 (en)](/patent/US11416798B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Data processing systems and methods for providing training in a vendor procurement process |
| [US11416634B2 (en)](/patent/US11416634B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Consent receipt management systems and related methods |
| [US11418516B2 (en)](/patent/US11418516B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Consent conversion optimization systems and related methods |
| [US11416589B2 (en)](/patent/US11416589B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11416576B2 (en)](/patent/US11416576B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Data processing consent capture systems and related methods |
| [US11416590B2 (en)](/patent/US11416590B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Data processing and scanning systems for assessing vendor risk |
| [US11416109B2 (en)](/patent/US11416109B2/en) | 2016-06-10 | 2022-08-16 | OneTrust, LLC | Automated data processing systems and methods for automatically processing data subject access requests using a chatbot |
| [US11544667B2 (en)](/patent/US11544667B2/en) | 2016-06-10 | 2023-01-03 | OneTrust, LLC | Data processing systems for generating and populating a data inventory |
| [US11520928B2 (en)](/patent/US11520928B2/en) | 2016-06-10 | 2022-12-06 | OneTrust, LLC | Data processing systems for generating personal data receipts and related methods |
| [US11488085B2 (en)](/patent/US11488085B2/en) | 2016-06-10 | 2022-11-01 | OneTrust, LLC | Questionnaire response automation for compliance management |
| [US11438386B2 (en)](/patent/US11438386B2/en) | 2016-06-10 | 2022-09-06 | OneTrust, LLC | Data processing systems for data-transfer risk identification, cross-border visualization generation, and related methods |
| [US11481710B2 (en)](/patent/US11481710B2/en) | 2016-06-10 | 2022-10-25 | OneTrust, LLC | Privacy management systems and methods |
| [US11475136B2 (en)](/patent/US11475136B2/en) | 2016-06-10 | 2022-10-18 | OneTrust, LLC | Data processing systems for data transfer risk identification and related methods |
| [US11468196B2 (en)](/patent/US11468196B2/en) | 2016-06-10 | 2022-10-11 | OneTrust, LLC | Data processing systems for validating authorization for personal data collection, storage, and processing |
| [US11468386B2 (en)](/patent/US11468386B2/en) | 2016-06-10 | 2022-10-11 | OneTrust, LLC | Data processing systems and methods for bundled privacy policies |
| [US11461722B2 (en)](/patent/US11461722B2/en) | 2016-06-10 | 2022-10-04 | OneTrust, LLC | Questionnaire response automation for compliance management |
| [US11449633B2 (en)](/patent/US11449633B2/en) | 2016-06-10 | 2022-09-20 | OneTrust, LLC | Data processing systems and methods for automatic discovery and assessment of mobile software development kits |
| [US10091077B1 (en)](/patent/US10091077B1/en) | 2016-06-27 | 2018-10-02 | Symantec Corporation | Systems and methods for detecting transactional message sequences that are obscured in multicast communications |
| [US9781149B1 (en)](/patent/US9781149B1/en) | 2016-08-17 | 2017-10-03 | Wombat Security Technologies, Inc. | Method and system for reducing reporting of non-malicious electronic messages in a cybersecurity system |
| [US9912687B1 (en)](/patent/US9912687B1/en) | 2016-08-17 | 2018-03-06 | Wombat Security Technologies, Inc. | Advanced processing of electronic messages with attachments in a cybersecurity system |
| [US10063584B1 (en)](/patent/US10063584B1/en) | 2016-08-17 | 2018-08-28 | Wombat Security Technologies, Inc. | Advanced processing of electronic messages with attachments in a cybersecurity system |
| [US10027701B1 (en)](/patent/US10027701B1/en) | 2016-08-17 | 2018-07-17 | Wombat Security Technologies, Inc. | Method and system for reducing reporting of non-malicious electronic messages in a cybersecurity system |
| [US9774626B1 (en)](/patent/US9774626B1/en) \* | 2016-08-17 | 2017-09-26 | Wombat Security Technologies, Inc. | Method and system for assessing and classifying reported potentially malicious messages in a cybersecurity system |
| [US10200259B1 (en)](/patent/US10200259B1/en) | 2016-09-21 | 2019-02-05 | Symantec Corporation | Systems and methods for detecting obscure cyclic application-layer message sequences in transport-layer message sequences |
| [US10880322B1 (en)](/patent/US10880322B1/en) | 2016-09-26 | 2020-12-29 | Agari Data, Inc. | Automated tracking of interaction with a resource of a message |
| [US12316591B2 (en)](/patent/US12316591B2/en) | 2016-09-26 | 2025-05-27 | Agari Data, Inc. | Multi-level security analysis and intermediate delivery of an electronic message |
| [US9847973B1 (en)](/patent/US9847973B1/en) | 2016-09-26 | 2017-12-19 | Agari Data, Inc. | Mitigating communication risk by detecting similarity to a trusted message contact |
| [US10805270B2 (en)](/patent/US10805270B2/en) | 2016-09-26 | 2020-10-13 | Agari Data, Inc. | Mitigating communication risk by verifying a sender of a message |
| [US11936604B2 (en)](/patent/US11936604B2/en) | 2016-09-26 | 2024-03-19 | Agari Data, Inc. | Multi-level security analysis and intermediate delivery of an electronic message |
| [US10326735B2 (en)](/patent/US10326735B2/en) | 2016-09-26 | 2019-06-18 | Agari Data, Inc. | Mitigating communication risk by detecting similarity to a trusted message contact |
| [US12074850B2 (en)](/patent/US12074850B2/en) | 2016-09-26 | 2024-08-27 | Agari Data, Inc. | Mitigating communication risk by verifying a sender of a message |
| [US11595354B2 (en)](/patent/US11595354B2/en) | 2016-09-26 | 2023-02-28 | Agari Data, Inc. | Mitigating communication risk by detecting similarity to a trusted message contact |
| [US10992645B2 (en)](/patent/US10992645B2/en) | 2016-09-26 | 2021-04-27 | Agari Data, Inc. | Mitigating communication risk by detecting similarity to a trusted message contact |
| [US9906545B1 (en)](/patent/US9906545B1/en) | 2016-11-22 | 2018-02-27 | Symantec Corporation | Systems and methods for identifying message payload bit fields in electronic communications |
| [US11044267B2 (en)](/patent/US11044267B2/en) | 2016-11-30 | 2021-06-22 | Agari Data, Inc. | Using a measure of influence of sender in determining a security risk associated with an electronic message |
| [US11722513B2 (en)](/patent/US11722513B2/en) | 2016-11-30 | 2023-08-08 | Agari Data, Inc. | Using a measure of influence of sender in determining a security risk associated with an electronic message |
| [US10715543B2 (en)](/patent/US10715543B2/en) | 2016-11-30 | 2020-07-14 | Agari Data, Inc. | Detecting computer security risk based on previously observed communications |
| [US10284579B2 (en)](/patent/US10284579B2/en) | 2017-03-22 | 2019-05-07 | Vade Secure, Inc. | Detection of email spoofing and spear phishing attacks |
| [US11132646B2 (en)](/patent/US11132646B2/en) \* | 2017-04-12 | 2021-09-28 | Fujifilm Business Innovation Corp. | Non-transitory computer-readable medium and email processing device for misrepresentation handling |
| [US12184662B2 (en)](/patent/US12184662B2/en) | 2017-04-26 | 2024-12-31 | Agari Data, Inc. | Message security assessment using sender identity profiles |
| [US11722497B2 (en)](/patent/US11722497B2/en) | 2017-04-26 | 2023-08-08 | Agari Data, Inc. | Message security assessment using sender identity profiles |
| [US11019076B1 (en)](/patent/US11019076B1/en) | 2017-04-26 | 2021-05-25 | Agari Data, Inc. | Message security assessment using sender identity profiles |
| [US10334015B2 (en)](/patent/US10334015B2/en) | 2017-04-28 | 2019-06-25 | Bank Of America Corporation | Apparatus and methods for shortening user exposure to malicious websites |
| [US10326788B1 (en)](/patent/US10326788B1/en) | 2017-05-05 | 2019-06-18 | Symantec Corporation | Systems and methods for identifying suspicious controller area network messages |
| [US12689631B2 (en)](/patent/US12689631B2/en) | 2017-05-19 | 2026-07-21 | Agari Data, Inc. | Using message context to evaluate security of requested data |
| [US10805314B2 (en)](/patent/US10805314B2/en) | 2017-05-19 | 2020-10-13 | Agari Data, Inc. | Using message context to evaluate security of requested data |
| [US10243904B1 (en)](/patent/US10243904B1/en) | 2017-05-26 | 2019-03-26 | Wombat Security Technologies, Inc. | Determining authenticity of reported user action in cybersecurity risk assessment |
| [US12081503B2 (en)](/patent/US12081503B2/en) | 2017-05-26 | 2024-09-03 | Proofpoint, Inc. | Determining authenticity of reported user action in cybersecurity risk assessment |
| [US10778626B2 (en)](/patent/US10778626B2/en) | 2017-05-26 | 2020-09-15 | Proofpoint, Inc. | Determining authenticity of reported user action in cybersecurity risk assessment |
| [US11757914B1 (en)](/patent/US11757914B1/en) | 2017-06-07 | 2023-09-12 | Agari Data, Inc. | Automated responsive message to determine a security risk of a message sender |
| [US11102244B1 (en)](/patent/US11102244B1/en) | 2017-06-07 | 2021-08-24 | Agari Data, Inc. | Automated intelligence gathering |
| [US11663359B2 (en)](/patent/US11663359B2/en) | 2017-06-16 | 2023-05-30 | OneTrust, LLC | Data processing systems for identifying whether cookies contain personally identifying information |
| [US11373007B2 (en)](/patent/US11373007B2/en) | 2017-06-16 | 2022-06-28 | OneTrust, LLC | Data processing systems for identifying whether cookies contain personally identifying information |
| [US10419478B2 (en)](/patent/US10419478B2/en) \* | 2017-07-05 | 2019-09-17 | Area 1 Security, Inc. | Identifying malicious messages based on received message data of the sender |
| [JP2019028724A (en)](/patent/JP2019028724A/en) \* | 2017-07-31 | 2019-02-21 | キヤノンマーケティングジャパン株式会社 | Information processing apparatus, information processing method, and program |
| [US11516248B2 (en)](/patent/US11516248B2/en) | 2017-08-25 | 2022-11-29 | Ecrime Management Strategies, Inc. | Security system for detection and mitigation of malicious communications |
| [US10708297B2 (en)](/patent/US10708297B2/en) | 2017-08-25 | 2020-07-07 | Ecrime Management Strategies, Inc. | Security system for detection and mitigation of malicious communications |
| [US11563757B2 (en)](/patent/US11563757B2/en) | 2017-08-31 | 2023-01-24 | Barracuda Networks, Inc. | System and method for email account takeover detection and remediation utilizing AI models |
| [US10778717B2 (en)](/patent/US10778717B2/en) | 2017-08-31 | 2020-09-15 | Barracuda Networks, Inc. | System and method for email account takeover detection and remediation |
| [US11665195B2 (en)](/patent/US11665195B2/en) | 2017-08-31 | 2023-05-30 | Barracuda Networks, Inc. | System and method for email account takeover detection and remediation utilizing anonymized datasets |
| [US20190238571A1 (en)](/patent/US20190238571A1/en) \* | 2018-01-29 | 2019-08-01 | International Business Machines Corporation | Method and system for email phishing attempts identification and notification through organizational cognitive solutions |
| [US10834111B2 (en)](/patent/US10834111B2/en) \* | 2018-01-29 | 2020-11-10 | International Business Machines Corporation | Method and system for email phishing attempts identification and notification through organizational cognitive solutions |
| [JP7614715B2 (en)](/patent/JP7614715B2/en) | 2018-02-20 | 2025-01-16 | ダークトレース リミテッド | Cyber threat defense system that uses machine learning models to protect email networks |
| [JP2019145107A (en)](/patent/JP2019145107A/en) \* | 2018-02-20 | 2019-08-29 | ダークトレース リミテッドＤａｒｋｔｒａｃｅ Ｌｉｍｉｔｅｄ | Cyber threat defense system protecting e-email network using machine learning model |
| [WO2020003406A1 (en)](/patent/WO2020003406A1/en) \* | 2018-06-27 | 2020-01-02 | 三菱電機株式会社 | Suspicious mail detection device, suspicious mail detection method, and suspicious mail detection program |
| [US12095814B2 (en)](/patent/US12095814B2/en) | 2018-08-22 | 2024-09-17 | NuRD LLC | Phishing website detection by checking form differences followed by false credentials submission |
| [US12706949B2 (en)](/patent/US12706949B2/en) | 2018-08-22 | 2026-08-11 | NuRD LLC | Phishing website detection by checking form differences followed by false credentials submission |
| [US11297101B1 (en)](/patent/US11297101B1/en) | 2018-08-22 | 2022-04-05 | NuRD LLC | Phishing website detection by checking form differences followed by false credentials submission |
| [US11496510B1 (en)](/patent/US11496510B1/en) | 2018-08-24 | 2022-11-08 | NuRD LLC | Fully automated target identification of a phishing web site |
| [US10963591B2 (en)](/patent/US10963591B2/en) | 2018-09-07 | 2021-03-30 | OneTrust, LLC | Data processing systems for orphaned data identification and deletion and related methods |
| [US11144675B2 (en)](/patent/US11144675B2/en) | 2018-09-07 | 2021-10-12 | OneTrust, LLC | Data processing systems and methods for automatically protecting sensitive data within privacy management systems |
| [US11544409B2 (en)](/patent/US11544409B2/en) | 2018-09-07 | 2023-01-03 | OneTrust, LLC | Data processing systems and methods for automatically protecting sensitive data within privacy management systems |
| [US11947708B2 (en)](/patent/US11947708B2/en) | 2018-09-07 | 2024-04-02 | OneTrust, LLC | Data processing systems and methods for automatically protecting sensitive data within privacy management systems |
| [US11157654B2 (en)](/patent/US11157654B2/en) | 2018-09-07 | 2021-10-26 | OneTrust, LLC | Data processing systems for orphaned data identification and deletion and related methods |
| [US11593523B2 (en)](/patent/US11593523B2/en) | 2018-09-07 | 2023-02-28 | OneTrust, LLC | Data processing systems for orphaned data identification and deletion and related methods |
| [US11025651B2 (en)](/patent/US11025651B2/en) | 2018-12-06 | 2021-06-01 | Saudi Arabian Oil Company | System and method for enhanced security analysis for quarantined email messages |
| [US12556550B2 (en)](/patent/US12556550B2/en) | 2018-12-19 | 2026-02-17 | Abnormal Ai, Inc. | Threat detection platforms for detecting, characterizing, and remediating email-based threats in real time |
| [US11743294B2 (en)](/patent/US11743294B2/en) | 2018-12-19 | 2023-08-29 | Abnormal Security Corporation | Retrospective learning of communication patterns by machine learning models for discovering abnormal behavior |
| [US12255915B2 (en)](/patent/US12255915B2/en) | 2018-12-19 | 2025-03-18 | Abnormal Security Corporation | Programmatic discovery, retrieval, and analysis of communications to identify abnormal communication activity |
| [US11973772B2 (en)](/patent/US11973772B2/en) | 2018-12-19 | 2024-04-30 | Abnormal Security Corporation | Multistage analysis of emails to identify security threats |
| [US11552969B2 (en)](/patent/US11552969B2/en) | 2018-12-19 | 2023-01-10 | Abnormal Security Corporation | Threat detection platforms for detecting, characterizing, and remediating email-based threats in real time |
| [US11824870B2 (en)](/patent/US11824870B2/en) | 2018-12-19 | 2023-11-21 | Abnormal Security Corporation | Threat detection platforms for detecting, characterizing, and remediating email-based threats in real time |
| [US11431738B2 (en)](/patent/US11431738B2/en) | 2018-12-19 | 2022-08-30 | Abnormal Security Corporation | Multistage analysis of emails to identify security threats |
| [US11425106B2 (en)](/patent/US11425106B2/en) | 2019-02-07 | 2022-08-23 | Egress Software Technologies Ip Limited | Method and system for processing data packages |
| [GB2581190B (en)](/patent/GB2581190B/en) \* | 2019-02-07 | 2021-10-27 | Egress Software Tech Ip Limited | Method and system for processing data packages |
| [US11425105B2 (en)](/patent/US11425105B2/en) | 2019-02-07 | 2022-08-23 | Egress Software Technologies Ip Limited | Method and system for processing data packages |
| [GB2581189B (en)](/patent/GB2581189B/en) \* | 2019-02-07 | 2021-10-27 | Egress Software Tech Ip Limited | Method and system for processing data packages |
| [AU2020219455B2 (en)](/patent/AU2020219455B2/en) \* | 2019-02-07 | 2024-12-19 | Egress Software Technologies Ip Ltd | Method and system for processing data packages |
| [WO2020161466A1 (en)](/patent/WO2020161466A1/en) \* | 2019-02-07 | 2020-08-13 | Egress Software Technologies Ip Ltd | Method and system for processing data packages |
| [GB2581188B (en)](/patent/GB2581188B/en) \* | 2019-02-07 | 2021-09-22 | Egress Software Tech Ip Limited | Method and system for processing data packages |
| [US10911417B2 (en)](/patent/US10911417B2/en) | 2019-02-07 | 2021-02-02 | Egress Software Technologies Ip Limited | Method and system for processing data packages |
| [AU2020218635B2 (en)](/patent/AU2020218635B2/en) \* | 2019-02-07 | 2024-12-19 | Egress Software Technologies Ip Ltd | Method and system for processing data packages |
| [WO2020161468A1 (en)](/patent/WO2020161468A1/en) \* | 2019-02-07 | 2020-08-13 | Egress Software Technologies Ip Ltd | Method and system for processing data packages |
| [WO2020161467A1 (en)](/patent/WO2020161467A1/en) \* | 2019-02-07 | 2020-08-13 | Egress Software Technologies Ip Ltd | Method and system for processing data packages |
| [AU2020219929B2 (en)](/patent/AU2020219929B2/en) \* | 2019-02-07 | 2025-01-09 | Egress Software Technologies Ip Ltd | Method and system for processing data packages |
| [US11411990B2 (en)](/patent/US11411990B2/en) \* | 2019-02-15 | 2022-08-09 | Forcepoint Llc | Early detection of potentially-compromised email accounts |
| [US12506747B1 (en)](/patent/US12506747B1/en) | 2019-03-29 | 2025-12-23 | Agari Data, Inc. | Message campaign and malicious threat detection |
| [JP2019145168A (en)](/patent/JP2019145168A/en) \* | 2019-05-23 | 2019-08-29 | キヤノンマーケティングジャパン株式会社 | Information processor, information processing method, and program |
| [JP7648353B2 (en)](/patent/JP7648353B2/en) | 2019-08-29 | 2025-03-18 | ダークトレース リミテッド | Endpoint Agent Extensions for Machine Learning Cyber Defense System for Email |
| [JP2021039754A (en)](/patent/JP2021039754A/en) \* | 2019-08-29 | 2021-03-11 | ダークトレース リミテッドＤａｒｋｔｒａｃｅ Ｌｉｍｉｔｅｄ | Endpoint agent expansion of machine learning cyber defense system for electronic mail |
| [CN111049733A (en)](/patent/CN111049733A/en) \* | 2019-12-10 | 2020-04-21 | 公安部第三研究所 | A concealed identification method for phishing email attacks |
| [US12081522B2 (en)](/patent/US12081522B2/en) | 2020-02-21 | 2024-09-03 | Abnormal Security Corporation | Discovering email account compromise through assessments of digital activities |
| [US11470042B2 (en)](/patent/US11470042B2/en) | 2020-02-21 | 2022-10-11 | Abnormal Security Corporation | Discovering email account compromise through assessments of digital activities |
| [RU2758358C2 (en)](/patent/RU2758358C2/en) \* | 2020-02-26 | 2021-10-28 | Акционерное общество "Лаборатория Касперского" | Method for generating signature for spam detection |
| [US11483344B2 (en)](/patent/US11483344B2/en) | 2020-02-28 | 2022-10-25 | Abnormal Security Corporation | Estimating risk posed by interacting with third parties through analysis of emails addressed to employees of multiple enterprises |
| [US11477235B2 (en)](/patent/US11477235B2/en) | 2020-02-28 | 2022-10-18 | Abnormal Security Corporation | Approaches to creating, managing, and applying a federated database to establish risk posed by third parties |
| [US11477234B2 (en)](/patent/US11477234B2/en) \* | 2020-02-28 | 2022-10-18 | Abnormal Security Corporation | Federated database for establishing and tracking risk of interactions with third parties |
| [US12500927B2 (en)](/patent/US12500927B2/en) | 2020-02-28 | 2025-12-16 | Abnormal Ai, Inc. | Federated database for establishing and tracking risk of interactions with third parties |
| [US11663303B2 (en)](/patent/US11663303B2/en) | 2020-03-02 | 2023-05-30 | Abnormal Security Corporation | Multichannel threat detection for protecting against account compromise |
| [US11949713B2 (en)](/patent/US11949713B2/en) | 2020-03-02 | 2024-04-02 | Abnormal Security Corporation | Abuse mailbox for facilitating discovery, investigation, and analysis of email-based threats |
| [US12470599B2 (en)](/patent/US12470599B2/en) | 2020-03-02 | 2025-11-11 | Abnormal Ai, Inc. | Abuse mailbox for facilitating discovery, investigation, and analysis of email-based threats |
| [US11451576B2 (en)](/patent/US11451576B2/en) | 2020-03-12 | 2022-09-20 | Abnormal Security Corporation | Investigation of threats using queryable records of behavior |
| [US12231453B2 (en)](/patent/US12231453B2/en) | 2020-03-12 | 2025-02-18 | Abnormal Security Corporation | Investigation of threats using queryable records of behavior |
| [US12531888B2 (en)](/patent/US12531888B2/en) | 2020-04-23 | 2026-01-20 | Abnormal Ai, Inc. | Detection and prevention of external fraud |
| [US11706247B2 (en)](/patent/US11706247B2/en) | 2020-04-23 | 2023-07-18 | Abnormal Security Corporation | Detection and prevention of external fraud |
| [US11470108B2 (en)](/patent/US11470108B2/en) | 2020-04-23 | 2022-10-11 | Abnormal Security Corporation | Detection and prevention of external fraud |
| [US11496505B2 (en)](/patent/US11496505B2/en) | 2020-04-23 | 2022-11-08 | Abnormal Security Corporation | Detection and prevention of external fraud |
| [US20210367918A1 (en)](/patent/US20210367918A1/en) \* | 2020-05-22 | 2021-11-25 | Nvidia Corporation | User perceptible indicia for web address identifiers |
| [US12353405B2 (en)](/patent/US12353405B2/en) | 2020-07-08 | 2025-07-08 | OneTrust, LLC | Systems and methods for targeted data discovery |
| [US11797528B2 (en)](/patent/US11797528B2/en) | 2020-07-08 | 2023-10-24 | OneTrust, LLC | Systems and methods for targeted data discovery |
| [US11968229B2 (en)](/patent/US11968229B2/en) | 2020-07-28 | 2024-04-23 | OneTrust, LLC | Systems and methods for automatically blocking the use of tracking tools |
| [US11444976B2 (en)](/patent/US11444976B2/en) | 2020-07-28 | 2022-09-13 | OneTrust, LLC | Systems and methods for automatically blocking the use of tracking tools |
| [US11475165B2 (en)](/patent/US11475165B2/en) | 2020-08-06 | 2022-10-18 | OneTrust, LLC | Data processing systems and methods for automatically redacting unstructured data from a data subject access request |
| [US11436373B2 (en)](/patent/US11436373B2/en) | 2020-09-15 | 2022-09-06 | OneTrust, LLC | Data processing systems and methods for detecting tools for the automatic blocking of consent requests |
| [US11704440B2 (en)](/patent/US11704440B2/en) | 2020-09-15 | 2023-07-18 | OneTrust, LLC | Data processing systems and methods for preventing execution of an action documenting a consent rejection |
| [US11050698B1 (en)](/patent/US11050698B1/en) \* | 2020-09-18 | 2021-06-29 | Area 1 Security, Inc. | Message processing system with business email compromise detection |
| [US11526624B2 (en)](/patent/US11526624B2/en) | 2020-09-21 | 2022-12-13 | OneTrust, LLC | Data processing systems and methods for automatically detecting target data transfers and target data processing |
| [US11784953B2 (en)](/patent/US11784953B2/en) | 2020-09-30 | 2023-10-10 | Qatar Foundation For Education, Science And Community Development | Systems and methods for encrypted message filtering |
| [EP4224351A4 (en)](/patent/EP4224351A4/en) \* | 2020-09-30 | 2023-11-01 | Fujitsu Limited | Verification method, verification program, and information processing device |
| [US11570132B2 (en)](/patent/US11570132B2/en) | 2020-09-30 | 2023-01-31 | Qatar Foundation Foreducation, Science And Community Development | Systems and methods for encrypted message filtering |
| [US12265896B2 (en)](/patent/US12265896B2/en) | 2020-10-05 | 2025-04-01 | OneTrust, LLC | Systems and methods for detecting prejudice bias in machine-learning models |
| [US11683284B2 (en)](/patent/US11683284B2/en) | 2020-10-23 | 2023-06-20 | Abnormal Security Corporation | Discovering graymail through real-time analysis of incoming email |
| [US11615192B2 (en)](/patent/US11615192B2/en) | 2020-11-06 | 2023-03-28 | OneTrust, LLC | Systems and methods for identifying data processing activities based on data discovery results |
| [US12277232B2 (en)](/patent/US12277232B2/en) | 2020-11-06 | 2025-04-15 | OneTrust, LLC | Systems and methods for identifying data processing activities based on data discovery results |
| [US11397819B2 (en)](/patent/US11397819B2/en) | 2020-11-06 | 2022-07-26 | OneTrust, LLC | Systems and methods for identifying data processing activities based on data discovery results |
| [US11687648B2 (en)](/patent/US11687648B2/en) | 2020-12-10 | 2023-06-27 | Abnormal Security Corporation | Deriving and surfacing insights regarding security threats |
| [US11704406B2 (en)](/patent/US11704406B2/en) | 2020-12-10 | 2023-07-18 | Abnormal Security Corporation | Deriving and surfacing insights regarding security threats |
| [US11687528B2 (en)](/patent/US11687528B2/en) | 2021-01-25 | 2023-06-27 | OneTrust, LLC | Systems and methods for discovery, classification, and indexing of data in a native computing system |
| [US12259882B2 (en)](/patent/US12259882B2/en) | 2021-01-25 | 2025-03-25 | OneTrust, LLC | Systems and methods for discovery, classification, and indexing of data in a native computing system |
| [US11442906B2 (en)](/patent/US11442906B2/en) | 2021-02-04 | 2022-09-13 | OneTrust, LLC | Managing custom attributes for domain objects defined within microservices |
| [US12536329B2 (en)](/patent/US12536329B2/en) | 2021-02-08 | 2026-01-27 | OneTrust, LLC | Data processing systems and methods for anonymizing data samples in classification analysis |
| [US11494515B2 (en)](/patent/US11494515B2/en) | 2021-02-08 | 2022-11-08 | OneTrust, LLC | Data processing systems and methods for anonymizing data samples in classification analysis |
| [US11601464B2 (en)](/patent/US11601464B2/en) | 2021-02-10 | 2023-03-07 | OneTrust, LLC | Systems and methods for mitigating risks of third-party computing system functionality integration into a first-party computing system |
| [US12641108B2 (en)](/patent/US12641108B2/en) | 2021-02-10 | 2026-05-26 | OneTrust, LLC | Systems and methods for mitigating risks of third-party computing system functionality integration into a first-party computing system |
| [US11775348B2 (en)](/patent/US11775348B2/en) | 2021-02-17 | 2023-10-03 | OneTrust, LLC | Managing custom workflows for domain objects defined within microservices |
| [US11546661B2 (en)](/patent/US11546661B2/en) | 2021-02-18 | 2023-01-03 | OneTrust, LLC | Selective redaction of media content |
| [US11533315B2 (en)](/patent/US11533315B2/en) | 2021-03-08 | 2022-12-20 | OneTrust, LLC | Data transfer discovery and analysis systems and related methods |
| [US11438292B1 (en)](/patent/US11438292B1/en) \* | 2021-04-12 | 2022-09-06 | EMC IP Holding Company LLC | Method and apparatus for filtering undesired email messages |
| [US12028373B2 (en)](/patent/US12028373B2/en) | 2021-04-14 | 2024-07-02 | Bank Of America Corporation | Information security system and method for preventing communications from detected phishing domains |
| [US11562078B2 (en)](/patent/US11562078B2/en) | 2021-04-16 | 2023-01-24 | OneTrust, LLC | Assessing and managing computational risk involved with integrating third party computing functionality within a computing system |
| [US11816224B2 (en)](/patent/US11816224B2/en) | 2021-04-16 | 2023-11-14 | OneTrust, LLC | Assessing and managing computational risk involved with integrating third party computing functionality within a computing system |
| [US11544673B2 (en)](/patent/US11544673B2/en) \* | 2021-04-30 | 2023-01-03 | Oracle International Corporation | Email message receiving system in a cloud infrastructure |
| [US11164156B1 (en)](/patent/US11164156B1/en) \* | 2021-04-30 | 2021-11-02 | Oracle International Corporation | Email message receiving system in a cloud infrastructure |
| [US20220351143A1 (en)](/patent/US20220351143A1/en) \* | 2021-04-30 | 2022-11-03 | Oracle International Corporation | Email message receiving system in a cloud infrastructure |
| [US12289304B2 (en)](/patent/US12289304B2/en) | 2021-05-26 | 2025-04-29 | Bank Of America Corporation | Information security system and method for phishing threat prevention using tokens |
| [US11792224B2 (en)](/patent/US11792224B2/en) | 2021-05-26 | 2023-10-17 | Bank Of America Corporation | Information security system and method for phishing threat detection using tokens |
| [US11831661B2 (en)](/patent/US11831661B2/en) | 2021-06-03 | 2023-11-28 | Abnormal Security Corporation | Multi-tiered approach to payload detection for incoming communications |
| [US12153704B2 (en)](/patent/US12153704B2/en) | 2021-08-05 | 2024-11-26 | OneTrust, LLC | Computing platform for facilitating data exchange among computing environments |
| [US11620142B1 (en)](/patent/US11620142B1/en) | 2022-06-03 | 2023-04-04 | OneTrust, LLC | Generating and customizing user interfaces for demonstrating functions of interactive user environments |
| [US20240356969A1 (en)](/patent/US20240356969A1/en) \* | 2023-04-24 | 2024-10-24 | Cisco Technology, Inc. | Statistical modeling of email senders to detect business email compromise |
| [US20250300953A1 (en)](/patent/US20250300953A1/en) \* | 2023-11-13 | 2025-09-25 | Cisco Technology, Inc. | Detecting malicious email attachments using context-specific feature sets |
| [US12355716B2 (en)](/patent/US12355716B2/en) \* | 2023-11-13 | 2025-07-08 | Cisco Technology, Inc. | Detecting malicious email attachments using context-specific feature sets |
| [US20260052170A1 (en)](/patent/US20260052170A1/en) \* | 2024-08-13 | 2026-02-19 | Bank Of America Corporation | System and method for detection and prevention of computing device intrusion vectors using ai |

## Similar Documents

| Publication | Publication Date | Title |
| --- | --- | --- |
| [US12184662B2 (en)](/patent/US12184662B2/en) | 2024-12-31 | Message security assessment using sender identity profiles |
| [US9154514B1 (en)](/patent/US9154514B1/en) | 2015-10-06 | Systems and methods for electronic message analysis |
| [US12074850B2 (en)](/patent/US12074850B2/en) | 2024-08-27 | Mitigating communication risk by verifying a sender of a message |
| [US9501746B2 (en)](/patent/US9501746B2/en) | 2016-11-22 | Systems and methods for electronic message analysis |
| [US10715543B2 (en)](/patent/US10715543B2/en) | 2020-07-14 | Detecting computer security risk based on previously observed communications |
| [US8910279B2 (en)](/patent/US8910279B2/en) | 2014-12-09 | Reputation-based threat protection |
| [US9123027B2 (en)](/patent/US9123027B2/en) | 2015-09-01 | Social engineering protection appliance |
| [US9413716B2 (en)](/patent/US9413716B2/en) | 2016-08-09 | Securing email communications |
| [WO2007146696A2 (en)](/patent/WO2007146696A2/en) | 2007-12-21 | Systems and methods for identifying potentially malicious messages |
| [WO2007045049A1 (en)](/patent/WO2007045049A1/en) | 2007-04-26 | Electronic message authentication |
| [EP1825389A4 (en)](/patent/EP1825389A4/en) | 2009-01-21 | Email anti-phishing inspector |
| [US20240054214A1 (en)](/patent/US20240054214A1/en) | 2024-02-15 | Computerized system for autonomous detection of unauthorized access according to outbound addresses |
| [Sanchez et al.](/scholar/5805769104074355924) | 2010 | Understanding forgery properties of spam delivery paths |
| [US20240340259A1 (en)](/patent/US20240340259A1/en) | 2024-10-10 | Computerized system for perimeter interface for alias electronic addresses |
| [Dantu et al.](/scholar/13055851748346019707) | 2008 | Classification of phishers. |
| [Fuhrman](/scholar/3583046425541658728) | 2008 | Forensic value of backscatter from email spam |
| [Cook](/scholar/195268824115373605) | 2005 | Catching spam before it arrives |
| [Sibi Chakkaravarthy et al.](/scholar/11164297861100736457) | 0 | A Comprehensive Examination of Email Spoofing: Issues and Prospects for Email Security |
| [Limthanmaphon et al.](/scholar/7399925055323040824) | 2011 | Enhanced Email Spam Prevention through Sender Verification Dual Models |
| [Lin](/scholar/6541235332556239755) | 2005 | Detecting and filtering instant messaging spam: a global and also personalized approach |

## Legal Events

| Date | Code | Title | Description |
| --- | --- | --- | --- |
| 2012-11-05 | AS | Assignment | **Owner name**: OSATECH INC., MASSACHUSETTS  **Free format text**: ASSIGNMENT OF ASSIGNORS INTEREST;ASSIGNORS:PRAKASH, GAGAN;AGARWAL, RAVI;REEL/FRAME:029293/0433  **Effective date**: 20121029  **Owner name**: OSATECH, INC., MAINE  **Free format text**: ASSIGNMENT OF ASSIGNORS INTEREST;ASSIGNORS:PRAKASH, GAGAN;AGARWAL, RAVI;SIGNING DATES FROM 20121027 TO 20121029;REEL/FRAME:029238/0066 |
| 2013-08-20 | AS | Assignment | **Owner name**: ASTRA IDENTITY, INC., MASSACHUSETTS  **Free format text**: ASSIGNMENT OF ASSIGNORS INTEREST;ASSIGNOR:OSATECH, INC.;REEL/FRAME:031041/0354  **Effective date**: 20130818 |
| 2013-10-02 | STCF | Information on status: patent grant | **Free format text**: PATENTED CASE |
| 2017-03-03 | FPAY | Fee payment | **Year of fee payment**: 4 |
| 2018-04-17 | AS | Assignment | **Owner name**: VADE SDECURE SAS, FRANCE  **Free format text**: ASSIGNMENT OF ASSIGNORS INTEREST;ASSIGNOR:ASTRA IDENTITY, INC.;REEL/FRAME:045780/0001  **Effective date**: 20180314 |
| 2018-06-07 | AS | Assignment | **Owner name**: VADE SECURE SAS, FRANCE  **Free format text**: CORRECTIVE ASSIGNMENT TO CORRECT THE ASSIGNEE NAME PREVIOUSLY RECORDED AT REEL: 045780 FRAME: 0001. ASSIGNOR(S) HEREBY CONFIRMS THE ASSIGNMENT;ASSIGNOR:ASTRA IDENTITY, INC.;REEL/FRAME:046318/0001  **Effective date**: 20180314 |
| 2020-10-22 | MAFP | Maintenance fee payment | **Free format text**: PAYMENT OF MAINTENANCE FEE, 8TH YR, SMALL ENTITY (ORIGINAL EVENT CODE: M2552); ENTITY STATUS OF PATENT OWNER: SMALL ENTITY  **Year of fee payment**: 8 |
| 2022-03-03 | AS | Assignment | **Owner name**: VADE USA, INCORPORATED, CALIFORNIA  **Free format text**: CHANGE OF NAME;ASSIGNOR:VADE SECURE, INCORPORATED;REEL/FRAME:059164/0846  **Effective date**: 20220222 |
| 2025-04-01 | FEPP | Fee payment procedure | **Free format text**: ENTITY STATUS SET TO UNDISCOUNTED (ORIGINAL EVENT CODE: BIG.); ENTITY STATUS OF PATENT OWNER: LARGE ENTITY |
| 2025-04-01 | MAFP | Maintenance fee payment | **Free format text**: PAYMENT OF MAINTENANCE FEE, 12TH YEAR, LARGE ENTITY (ORIGINAL EVENT CODE: M1553); ENTITY STATUS OF PATENT OWNER: LARGE ENTITY  **Year of fee payment**: 12 |
