# Private Mail Server
[![DEMO](https://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](https://www.youtube.com/watch?v=Qn7MipYrbAk)

## Project Overview
A mail server configured with Postfix, Dovecot, Amavisd-new, SpamAssassin, and ClamAV. This robust infrastructure prioritizes your privacy and security, ensuring every email is shielded from prying eyes and malicious threats.

### Tools Used
- **Postfix**: Chosen for its reliability and robust performance as a Mail Transfer Agent (MTA).
- **Dovecot**: Selected for handling IMAP and POP3 services due to its security and ease of use.
- **Amavisd**, **SpamAssassin**, **ClamAV**: Integrated for email filtering and antivirus protection, providing a comprehensive security solution.
- **SPF**, **DKIM**, **DMARC**: Implemented for email authentication to enhance email security and prevent spoofing.

## Installation

### Operating System
- **Debian 12**

## Configuration Details

### Overview
- Ensure that SMTP ports are unblocked by the hosting service
- A dedicated IP with a good reputation.

### Key Configurations
- **SSL/TLS Setup**: SSL/TLS certificates were generated using Certbot to secure mail transmission.
- Example configuration files are not provided as this project serves as a showcase.

## Security Measures

### SSL/TLS Setup
- SSL/TLS certificates were generated using Certbot to ensure secure mail transmission.
![alt text](https://i.imgur.com/4FWMvmY.png)

## SPF, DKIM, and DMARC
DNS Records
![alt text](https://i.imgur.com/roH1RL1.png)

### Overview
- **SPF (Sender Policy Framework)**: SPF helps prevent email spoofing by allowing the domain owner to specify which mail servers are permitted to send emails on behalf of their domain.
- **DKIM (DomainKeys Identified Mail)**: DKIM adds a digital signature to emails, enabling the recipient’s server to verify that the email was indeed sent by the claimed domain and that it hasn't been altered during transit.
- **DMARC (Domain-based Message Authentication, Reporting, and Conformance)**: DMARC builds on SPF and DKIM, allowing domain owners to define how receiving mail servers should handle emails that fail SPF or DKIM checks. It also provides a way for domain owners to receive reports on email authentication.

These protocols work together to enhance email security, protect against phishing and spoofing, and improve the overall deliverability of legitimate emails.

