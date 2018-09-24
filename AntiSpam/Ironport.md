Before jumping into logs, it's higly recommended to take a look on the mail flow done by the appliance.

Most of the information here provided, is based on Cisco official documentation located here [Mail Flow Documentation](https://www.cisco.com/c/en/us/td/docs/security/esa/esa11-1/user_guide/b_ESA_Admin_Guide_11_1/b_ESA_Admin_Guide_chapter_011.pdf)

## Mail Flow

Cisco split email flow in 3 phases, described below and 

Receiving Email Connections
1) Email Received 
SBRS
2) HAT - Host Access Table 
SPF/DKIM/DMARC
3) RAT - Recipient Access Table
4) Message Filters
Anti-Spam
Anti-Virus
AMP
Content Filters
Outbreak Filters

## Collecting logs

In order to collect logs via syslogs, you need to create subscriptions to each target log.
The log types are available in this link: [ESA Logs and Subscriptions](https://www.cisco.com/c/en/us/td/docs/security/esa/esa11-1/user_guide/b_ESA_Admin_Guide_11_1/b_ESA_Admin_Guide_11_1_chapter_0100111.pdf)


## Subscriptions and Log Types

The available log types are:

| Log Type  | Description | Pre-ATT&CK | What to monitor | Enable | Timestamp |
|-----------| ----------- | ---------- | --------------- | ------ | --------- |
| Text Mails | Contain details of email receiving, email delivery and bounces |---- | Message tracking, audit | default. Need additional configuration for attachment names | yes |
| Mail | --- | --- | --- | --- | yes |
| LDAP | --- | --- | --- | --- | yes |
| System | --- | --- | --- | --- | yes |
| Delivery | ---- | ---- | ---- | ---- | ---- |
| Bounce | ---- | ---- | ---- | ---- | ---- |
| Status | ---- | ---- | ---- | ---- | ---- |
| Domain Debug | ---- | ---- | ---- | ---- | ---- |
| Injection Debug | ---- | ---- | ---- | ---- | ---- |
| System | ---- | ---- | ---- | ---- | ---- |
| CLI Audit | ---- | ---- | ---- | ---- | ---- |
| FTP Server | ---- | ---- | ---- | ---- | ---- |
| HTTP | ---- | ---- | ---- | ---- | ---- |
| NTP | ---- | ---- | ---- | ---- | ---- |
| Scanning | ---- | ---- | ---- | ---- | ---- |
| Anti-Spam | ---- | ---- | ---- | ---- | ---- |
| Graymail | ---- | ---- | ---- | ---- | ---- |
| Anti-Virus | ---- | ---- | ---- | ---- | ---- |
| AMP Engine | ---- | ---- | ---- | ---- | ---- |
| Spam Quarantine | ---- | ---- | ---- | ---- | ---- |
| Spam Quarantine GUI | ---- | ---- | ---- | ---- | ---- |
| LDAP Debug | ---- | ---- | ---- | ---- | ---- |
| Safelist/Blocklist | ---- | ---- | ---- | ---- | ---- |
| Reporting | ---- | ---- | ---- | ---- | ---- |
| Reporting Query | ---- | ---- | ---- | ---- | ---- |
| Updater | ---- | ---- | ---- | ---- | ---- |
| Tracking | ---- | ---- | ---- | ---- | ---- |
| Authentication | ---- | ---- | ---- | ---- | ---- |
| Configuration History | ---- | ---- | ---- | ---- | ---- |


## Tips

Ironport Antivirus logs

When a virus is found, two log entries are generated. One with the malware signature that can be consulted on Talos Intelligence and other confirming message was dropped. (Validate conditions)

## Improvements

Ironport Antivirus logs

One good improvement would be having the hash of the samples on the log. Just remembering the AV engine on Ironport appliances are Sophos or McAfee. This [signature](https://www.sophos.com/en-us/threat-center/threat-analyses/viruses-and-spyware/CXmail~VBSDl-A.aspx), very common on spam doesn't give us useful information. 
