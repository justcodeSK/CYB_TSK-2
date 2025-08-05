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
- Link points to: `http://login-update.paypall-login.com` (not PayPal)
- Urgent language: "Your account will be suspended!"
- Grammar mistakes present "Microsoft account unusual signin activity" the account A wasent capitalized and microsoft dosenot send mails form a domain like "access-accsecurity" correct ones are "is microsoft.com, entra.microsoft.com and azure.com"
- Fake branding
- no valied domain found
- reply to mail the email user name ends with digits no valied company makes an email like that for reply purposes and the mail given is in capital "NO-REPLY@ACCESS-ACCSECURITY.COM".
- dkim (domain key identified mail) email message was not digitally signed with DomainKeys "dkim=none (message not signed)".
- They provided a random Domain name which is related to security thats all.
- they used microsoft smtp server id in their Header means must have been compromized.
- Senders IP -89.144.9.91 and has checked for black listed ip address from https://www.virustotal.com/gui/home/url may be its a newly generated Spoof mail/Phishing mail from new Hacker or used a compromised user.
- 

## Outcome
Gained practical experience in identifying phishing tactics, analyzing email headers, and understanding how social engineering is used in email-based attacks.

## Screenshots
- Header analysis result email analysis 1.png, 
- Email body
