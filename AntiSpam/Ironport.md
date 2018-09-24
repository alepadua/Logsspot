Before jumping into logs, it's higly recommended to take a look on the mail flow done by the appliance.

Most of the information here provided, is based on Cisco official documentation located here [Mail Flow Documentation](https://www.cisco.com/c/en/us/td/docs/security/esa/esa11-1/user_guide/b_ESA_Admin_Guide_11_1/b_ESA_Admin_Guide_chapter_011.pdf)

##Mail Flow

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

##Collecting logs

In order to collect logs via syslogs, you need to create subscriptions to each target log.
The log types are available in this link: [ESA Logs and Subscriptions](https://www.cisco.com/c/en/us/td/docs/security/esa/esa11-1/user_guide/b_ESA_Admin_Guide_11_1/b_ESA_Admin_Guide_11_1_chapter_0100111.pdf)


##Subscriptions and Log Types

The available log types are:

| Log Type  | Description | Pre-ATT&CK | What to monitor | Enable | Timestamp |
|-----------| ----------- | ---------- | --------------- | ------ | --------- |
| Text Mails | ---- |---- |---- |---- | yes |
| Mail | --- | --- | --- | --- | yes |
| LDAP | --- | --- | --- | --- | yes |
| System | --- | --- | --- | --- | yes |
| --- |--- | --- | --- | --- | --- | yes |



-Delivery Logs
-Bounce Logs
-Status Logs
-Domain Debug Logs
-Injection Debug Logs
-System Logs
-CLI Audit Logs
-FTP Server Logs
-HTTP Logs
-NTP Logs
-Scanning Logs
-Anti-Spam Logs
-Graymail Logs
-Anti-Virus Logs
-AMP Engine Logs
-Spam Quarantine Logs
-Spam Quarantine GUI Logs
-LDAP Debug Logs
-Safelist/Blocklist Logs
-Reporting Logs
-Reporting Query Logs
-Updater Logs
-tanding Tracking Logs
-Authentication Logs
-Configuration History Logs
