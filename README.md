# Phishing Email Analysis - Cybersecurity Internship

## Objective
To identify phishing characteristics in a suspicious email.

## Tools Used
- Kali Linux (VM) used for safe use of malicious mail urls and attachments in mail.
- MXToolbox Header Analyzer https://mxtoolbox.com/
- VirusTotal https://www.virustotal.com/gui/home/url
- Google Admin Toolbox https://toolbox.googleapps.com/apps/messageheader/analyzeheader
- EML Analyzer https://eml-analyzer.herokuapp.com/
- URLScan https://urlscan.io/

## Key Findings of sample 1039(some screen shorts are used to learn with other samples i will provide the samples i used in the same repository)
- Spoofed email: `no-reply@access-accsecurity.com`, ''
- Header shows mismatched IP and sending domain
- Message ID foun- 	<2f661a40-f9bc-43ee-a7a8-7fc67e7b8128@VI1EUR02FT049.eop-EUR02.prod.protection.outlook.com>
- Grammar mistakes present "Microsoft account unusual signin activity" the account A wasent capitalized and microsoft dosenot send mails form a domain like "access-accsecurity" correct ones are "is microsoft.com, entra.microsoft.com and azure.com"
- Fake branding
- no valied domain found
- reply to mail the email user name ends with digits no valied company makes an email like that for reply purposes and the mail given is in capital "NO-REPLY@ACCESS-ACCSECURITY.COM".
- dkim (domain key identified mail) email message was not digitally signed with DomainKeys "dkim=none (message not signed)".
- They provided a random Domain name which is related to security thats all.
- they used microsoft smtp server id in their Header means must have been compromized.
- Senders IP -89.144.9.91 and has checked for black listed ip address from https://www.virustotal.com/gui/home/url may be its a newly generated Spoof mail/Phishing mail from new Hacker or used a compromised user.
- The mail hase no urgent or threatening language but was a Triggerring one unaware users could have been a Victum to this mail.
- The Language and Grammer used was clearly unproffessional hence can be identified as a Phishing mail "A user from Russia/Moscow just logged into your account from a new device, If this wasn't you, please report the user. If this was you, we'll trust similar activity in the future.".
- Mainly the Extracted ipaddress (103.225.77.255) is an INDIAN orgin hence its clear that its not from Russia/Moscow.
- Date Found in Header `Mon, 31 Jul 2023 01:49:22 +0000` The timestamp appears valid, but if it differs significantly from the received time, it may indicate spoofing.
- Found that the URL attached to email is an Phishing URL which is black listed by 3 defender or security applications.

## Outcome
Gained practical experience in identifying phishing tactics, analyzing email headers, and understanding how social engineering is used in email-based attacks.

## Screenshots
- Header analysis result `email analysis 1.png`
  `email analysis 1.png`
  `email analysis 2.png`
  `email analysis 3.png`
- Email body- Attached in repository.
