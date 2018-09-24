Before jumping into logs, it's higly recommended to take a look on the mail flow done by the appliance.

Most of the information here provided, is based on Cisco official documentation located here [Mail Flow Documentation](https://www.cisco.com/c/en/us/td/docs/security/esa/esa11-1/user_guide/b_ESA_Admin_Guide_11_1/b_ESA_Admin_Guide_chapter_011.pdf)

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

In order to collect logs via syslogs, you need to create subscriptions to each target log.
The log types are available in this link: [ESA Logs and Subscriptions](https://www.cisco.com/c/en/us/td/docs/security/esa/esa11-1/user_guide/b_ESA_Admin_Guide_11_1/b_ESA_Admin_Guide_11_1_chapter_0100111.pdf)
