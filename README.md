# Cybersecurity-task2

Phishing Email Analysis Report

Submitted by: Akhila Mohan R



Sample Email

- From: Bank Locker New Update <newsletter@mc.tracksmails.com>  
- To: akhilamohanr123@gmail.com  
- Subject**: "Do this work immediately, otherwise your bank locker may be sealed!"



 Header Analysis Summary

| Check | Result | Notes |

| SPF |  Pass | IP `216.117.134.156` is authorized by `mc.tracksmails.com` |
| DKIM |  Pass | Domain matched and signed |
| DMARC |  Missing/Not aligned | No visible result — possible red flag |
| Delivery Delay |  21 minutes | Delay in SMTP delivery suggests mass mailing or redirect |
| Domain Check |  Not a bank domain | `mc.tracksmails.com` is a marketing tracker, not a financial institution |



Phishing Indicators

1. Fake Sense of Urgency: "Do this work immediately…"
2. Suspicious Sender Domain: Email claims to be from a bank but sent by `mc.tracksmails.com`.
3. Marketing/Tracking Origin: Mass email tool disguised as official notice.
4. Lack of Personalization: Likely generic, not targeting just the user.
5. DMARC Not Aligned: Could be used to spoof bank branding.



Tools Used

- Google Header Analyzer  
- Manual Domain/IP Analysis  
- WHOIS for domain  
- Kali Linux Terminal Tools (`whois`, `host`, `dig`)



Conclusion

This email demonstrates phishing characteristics including impersonation of a bank, use of urgency, and use of third-party mass marketing platforms to send critical account messages. **It is not legitimate** and should be reported or marked as spam.


