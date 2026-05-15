# Answer Sheet

## 1. Sample-1000.eml:

<img width="1850" height="806" alt="Screenshot 2026-05-15 113804" src="https://github.com/user-attachments/assets/14c94f69-7261-4675-9e17-cc62f0e4fa04" />

###Translation:
[BB] - Your balance has been released - Code: 11084339647130851921

From: prestonconstance587[@]gmail[.]com
To: phishing@pot

IRPF Release - 6NwlyfzWcsNerv0

Dear customer,

Balance available for credit into your account.

More information in the attachment.

Protocol: 4793122145117905827; 05:59:01 PM

### Basic Information
<img width="1177" height="238" alt="Screenshot 2026-05-15 115447" src="https://github.com/user-attachments/assets/fd994c60-0440-4edc-ba00-7d86860f37c8" />

- **Subject: IRPF Release - 6NwlyfzWcsNerv0**  
- **From: prestonconstance587[@]gmail[.]com**  
- **Reply-To: None**  
- **Date: Wed, 26 Jul. 2023, 17:59:01**  
- **Return-Path: prestonconstance587[@]gmail[.]com**

### Header Analysis
- SPF: Pass — sender IP 209.85.160.178 authorized to send mail for gmail.com
- DKIM: Pass — DKIM signature verified successfully for gmail.com
- DMARC: Pass — DMARC validation passed for gmail.com
- Received chain observations:
  - Email passed through multiple Microsoft Outlook protection servers.
  - Message was received by smtp.gmail.com from host "a3.domain".
  - The hostname "a3.domain" appears generic and potentially suspicious.
  - The email used authenticated Gmail infrastructure despite suspicious relay behavior.
- Originating IP address: 20.97.213.223

### Phishing Indicators
- Suspicious sender domain:
  - The email appears to originate from the hostname "a3.domain," which is unusually generic and does not resemble a legitimate banking or corporate mail server.
  - The sender used Gmail.com infrastructure while impersonating a financial-related notification, which is suspicious behavior commonly seen in phishing campaigns.
- Suspicious attachment:

  <img width="360" height="73" alt="image" src="https://github.com/user-attachments/assets/868a8189-83a7-4b25-bf0e-4397d69cc75a" />

  -   The email contains a suspicious PDF attachment named `csWuYjyqO2IR.pdf`.

- Grammar or spelling issues:

  <img width="269" height="96" alt="image" src="https://github.com/user-attachments/assets/3eaa0cfb-9d1a-4052-a7dd-9385dbdc257f" />

  - The email contains a spelling error: “créito” instead of “crédito.”
  - Minor grammatical inconsistencies suggest the message may not have been professionally written.

### URLs
- The email has no URLs.
### Attachments
<img width="978" height="37" alt="image" src="https://github.com/user-attachments/assets/d35256b2-5ac7-49ca-bab9-4b2db0635545" />

<img width="954" height="746" alt="image" src="https://github.com/user-attachments/assets/d09f8f6f-f822-4251-9500-481d74e40c69" />

- A SHA-256 hash was generated from the attachment using the `sha256sum` command.
  
- The hash was analyzed using VirusTotal (https://www.virustotal.com/gui/home/upload) to determine whether the file was malicious.
  
- VirusTotal identified the PDF attachment as malicious and associated with phishing activity.
  
- The attachment appears to be designed to trick users into opening a phishing document or credential-harvesting payload.

### IOC (Indicators of Compromise)
- Domains:
  - gmail.com
  - a3.domain

- IP Addresses:
  - 20.97.213.223

- Hashes:
  - SHA-256: cfc5fbc759dcc599c8329dd94f9364394c7b1e875d6ff515c7337e00fb1f30cf

- Email Addresses:
  - prestonconstance587[@]gmail[.]com

### Social Engineering Techniques

- Authority impersonation:
  - The email appears to impersonate a financial or banking institution.

- Attachment-based malware:
  - The phishing email includes a malicious Trojan hidden as a PDF attachment.

### Final Verdict
- **Classification:** Phishing 
