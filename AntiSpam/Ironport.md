Before jumping into logs, it's higly recommended to take a look on the mail flow done by the appliance.

Most of the information here provided, is based on Cisco official documentation located here [Mail Flow Documentation](https://www.cisco.com/c/en/us/td/docs/security/esa/esa11-1/user_guide/b_ESA_Admin_Guide_11_1/b_ESA_Admin_Guide_chapter_011.pdf)

Receiving Email Connections
1) Email Received 
2) HAT - Host Access Table 
3) RAT - Recipient Access Table
4) 

Email -> SBRS -> HAT -> SPF/DKIM/DMARC -> RAT -> Message filters -> Anti-Spam -> Anti-Virus -> AMP -> Content Filters -> Outbreak Filters
