# Phishing Email Analysis - Cybersecurity Internship

## Objective
To identify phishing characteristics in a suspicious email.

## Tools Used
- Kali Linux (VM) used for safe use of malicious mail URLs and attachments in mail.
- MXToolbox Header Analyzer https://mxtoolbox.com/
- VirusTotal https://www.virustotal.com/gui/home/url
- Google Admin Toolbox https://toolbox.googleapps.com/apps/messageheader/analyzeheader
- EML Analyzer https://eml-analyzer.herokuapp.com/
- URLScan https://urlscan.io/

## Key Findings of sample 1039(some screenshots are used to learn with other samples i will provide the samples i used in the same repository)
- Spoofed email: `no-reply@access-accsecurity.com`, ''
- Header shows mismatched IP and sending domain
- Message ID found- 	<2f661a40-f9bc-43ee-a7a8-7fc67e7b8128@VI1EUR02FT049.eop-EUR02.prod.protection.outlook.com>
- Grammar mistakes present "Microsoft account unusual sign-in activity" the account A wasn't capitalized and Microsoft does not send mails from a domain like "access-accsecurity" correct ones are "is microsoft.com, entra.microsoft.com and azure.com"
- Fake branding
- no valid domain found
- reply to mail the email user name ends with digits no valid company makes an email like that for reply purposes and the mail given is in capital "NO-REPLY@ACCESS-ACCSECURITY.COM".
- dkim (domain key identified mail) email message was not digitally signed with DomainKeys "dkim=none (message not signed)".
- They provided a random Domain name which is related to security that's all.
- they used Microsoft SMTP server id in their Header means must have been compromised.
- Senders IP -89.144.9.91 and has checked for blacklisted IP address from https://www.virustotal.com/gui/home/url may be it's a newly generated Spoof mail/Phishing mail from new Hacker or used a compromised user.
- The mail has no urgent or threatening language but was a Triggering one unaware users could have been a Victim to this mail.
- The Language and Grammar used was clearly unprofessional hence can be identified as a Phishing mail "A user from Russia/Moscow just logged into your account from a new device, If this wasn't you, please report the user. If this was you, we'll trust similar activity in the future.".
- Mainly the Extracted IP address (103.225.77.255) is an INDIAN origin hence it's clear that it's not from Russia/Moscow.
- Date Found in Header `Mon, 31 Jul 2023 01:49:22 +0000` The timestamp appears valid, but if it differs significantly from the received time, it may indicate spoofing.
- Found that the URL attached to email is a Phishing URL which is blacklisted by 3 defender or security applications.

## Outcome
Gained practical experience in identifying phishing tactics, analyzing email headers, and understanding how social engineering is used in email-based attacks.
##Personal Opinion
- EML Analyzer and VirusTotal are much better tools than others, Google Admin Lookups are also good.
## Screenshots
- Header analysis result `email analysis 1.png`
  `email analysis 1.png`
  `email analysis 2.png`
  `email analysis 3.png`
- Email body- Attached in repository.
