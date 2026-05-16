# Answer Sheet

## 1. Sample-1000.eml:

<img width="1850" height="806" alt="Screenshot 2026-05-15 113804" src="https://github.com/user-attachments/assets/14c94f69-7261-4675-9e17-cc62f0e4fa04" />

### Translation:

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

  - The email contains a suspicious PDF attachment named `csWuYjyqO2IR.pdf`.

- Grammar or spelling issues:

  <img width="269" height="96" alt="image" src="https://github.com/user-attachments/assets/3eaa0cfb-9d1a-4052-a7dd-9385dbdc257f" />

  - The email contains a spelling error: “créito” instead of “crédito.”
  - Minor grammatical inconsistencies suggest the message may not have been professionally written.

### URL Analysis
- The email has no URLs.

### Attachments Analysi
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

## 2. Sample-1001.eml:

<img width="1853" height="796" alt="image" src="https://github.com/user-attachments/assets/7b9f61f1-5770-4318-bd90-164e86b82217" />

### Basic Information

<img width="1667" height="493" alt="image" src="https://github.com/user-attachments/assets/093bdc20-8f68-4888-b7dc-c9c451859487" />

- **Subject: Microsoft account unusual signin activity**  
- **From: Microsoft account team, _<no-reply[@]access-accsecurity[.]com>**  
- **Reply-To: solutionteamrecognizd02@gmail.com**  
- **Date: Thu, 27 Jul 2023 07:40:03 +0000**  
- **Return-Path: bounce@nonkfrgr.co.uk**

### Header Analysis

<img width="608" height="243" alt="image" src="https://github.com/user-attachments/assets/26295833-07ec-45dc-ba06-1003c3f51afa" />

<img width="699" height="183" alt="image" src="https://github.com/user-attachments/assets/f2bd2c8e-2ad2-4fe7-8343-22a0b77e6273" />

<img width="809" height="513" alt="image" src="https://github.com/user-attachments/assets/8b590e5b-ce5d-4bf5-a1d7-f6b04e914c65" />

- SPF:
  - Fail / None — `nonkfrgr[.]co[.]uk` does not designate permitted sender hosts.
  - The sender IP address `89.144.9.87` was not authorized to send email on behalf of the domain.

- DKIM:
  - None — the message was not DKIM signed.
  - No valid cryptographic signature was present to verify message authenticity.

- DMARC:
  - Permerror — DMARC validation failed due to authentication issues and domain misalignment.
  - The email failed proper sender verification checks.

- Received chain observations:
  - The email passed through multiple Microsoft Outlook and Exchange protection servers.
  - The originating sending server appears to be `nonkfrgr[.]co[.]uk`.
  
- Originating IP address:
  - The originating IP address `89.144.9.87` appears to be from Germany and not from Microsoft.

### Phishing Indicators

- Suspicious sender domain:
  - The sender domain `access-accsecurity[.]com` impersonates Microsoft but is not an official Microsoft domain.
  - The originating server `nonkfrgr[.]co[.]uk` is suspicious and unrelated to legitimate Microsoft mail infrastructure.

- Reply-To mismatch:
  - The email directs replies to: `solutionteamrecognizd02[@]gmail[.]com`
  - Microsoft security alerts would not use a free Gmail address for support or incident response.

- Urgent or threatening language:
  - The subject line: "Microsoft account unusual signin activity"
    - attempts to create fear and urgency by implying unauthorized account access.
  - The email pressures the victim into reacting quickly to supposed suspicious activity.

- Suspicious attachment:
  - The email contains unusually large embedded content and may include malicious HTML or credential-harvesting components.

- Suspicious links:
  - The HTML content includes a suspicious mailto link: `mailto:solutionteamrecognizd02[@]gmail[.]com`
  - The message encourages victims to contact a non-Microsoft Gmail account.

- Spoofed branding/company:
  - The email impersonates Microsoft account security notifications using fake branding and unofficial domains.
  - The HTML formatting attempts to mimic legitimate Microsoft security alert templates.

- Grammar or spelling issues:
  - The phrase: `Unusual sign.in activity`
    - contains improper punctuation and formatting.
  - The Reply-To address contains the misspelled word: `recognizd`
  - Legitimate Microsoft notifications are typically professionally written and free of these errors.

### URL Analysis

<img width="1022" height="233" alt="image" src="https://github.com/user-attachments/assets/ea8bfb47-c63c-4657-afd4-b4418141f353" />

<img width="925" height="285" alt="image" src="https://github.com/user-attachments/assets/4215d7bc-d0df-470d-8403-4854ad1dcd8e" />


- The email contains a “Report User” button; however, instead of redirecting users to a legitimate :contentReference[oaicite:0]{index=0} support page, it uses a suspicious `mailto:` link directed to:
  `solutionteamrecognizd02[@]gmail.com`
- This strongly suggests phishing activity. The domain or infrastructure associated with the campaign has likely already been reported and taken down.


- We used a tool called `eico.py` to extract artifacts and indicators from the email. During analysis, we identified a suspicious URL embedded within the message:
  `http://thebandalisty[.]com/track/o39473XgziG18708448HxBA1821750yoR33736gMed176`
  -  After scanning the URL with security analysis tools, it was identified as malicious.
- We also attempted to perform dynamic analysis using Hybrid Analysis. However, the phishing domain and associated infrastructure appeared to have already been taken offline, which is common with older phishing campaigns.

### Attachment Analysis
- There are no attachments

### IOC (Indicators of Compromise)
- Domains:
  - access-accsecurity[.]com
  - nonkfrgr[.]co[.]uk
  - thebandalisty[.]com

- IP Addresses:
  - 89.144.9.87

- URLs:
  - `http://thebandalisty[.]com/track/o39473XgziG18708448HxBA1821750yoR33736gMed176`

- Email Addresses:
  - no-reply[@]access-accsecurity[.]com
  - solutionteamrecognizd02[@]gmail[.]com

### Social Engineering Techniques
- Urgency:
  - The email attempts to pressure the victim into taking immediate action by claiming there was unusual sign-in activity on their Microsoft account.

- Fear:
  - The message creates fear by suggesting the account may have been compromised or accessed without authorization.

- Authority impersonation:
  - The email contains a “Report User” button; however, instead of redirecting users to a legitimate Microsoft support page, it uses a suspicious `mailto:` link directed to:
  `solutionteamrecognizd02[@]gmail[.]com`

- Account security scare tactics:
  - The email uses security-related language and fake account alerts to manipulate the victim into responding quickly without carefully verifying the message.

- Credential harvesting:
  - The phishing email likely attempts to trick users into providing account credentials or sensitive information through malicious links or attacker-controlled communication channels.

- Brand impersonation:
  - The email copies Microsoft branding, formatting, and account security messaging to make the phishing campaign appear authentic.

### Final Verdict
- **Classification:** Phishing 

## 3. Sample-1006.eml:

<img width="658" height="465" alt="image" src="https://github.com/user-attachments/assets/6dc633ca-1c7b-4e82-a7f5-76340243181f" />

### Basic Information

<img width="1038" height="554" alt="image" src="https://github.com/user-attachments/assets/4ae3227b-2cb3-48c5-beb4-37b79e19521c" />

- **Subject: Attention:I am Diplomatic agent Mr.Wood Forest**  
- **From: Mr.Wood Forest**  
- **Reply-To: mywoodforestbiz[.]7[@]gmail[.]com**  
- **Date: Sat, 29 Jul 2023 13:03:39 -0700**  
- **Return-Path: nemani[.]tukunia@postfiji[.]com[.]fj**

### Header Analysis

<img width="561" height="69" alt="image" src="https://github.com/user-attachments/assets/e6f25abe-0523-4cd6-84ee-27bd41fe34aa" />

<img width="782" height="630" alt="image" src="https://github.com/user-attachments/assets/05e694cb-3ac4-49fe-8590-bb7908c4b2ab" />

<img width="791" height="629" alt="image" src="https://github.com/user-attachments/assets/d24f0caa-4280-4702-86f9-4c0975e01000" />

- SPF: Fail — postfiji[.]com[.]fj did not authorize 109.202.24.52 to send email on its behalf.
- DKIM: None — the message was not digitally signed, so the sender’s identity could not be verified.
- DMARC: None — no DMARC validation/alignment was present for the domain.
- Received chain observations:
  - Email originated from 85.208.139.60
  - Relayed through 54upr[.]rosreestr[.]ru (85.208.139.60)
  - Claimed sender domain was postfiji[.]com[.]fj
  - Reply-To redirected to mywoodforestbiz[.]7[@]gmail[.]com
  - Passed through legitimate Microsoft Outlook/Office365 mail servers afterward
  - Multiple spoofing indicators suggest phishing/scam activity
  - Russian relay server and mismatched Fiji sender domain are suspicious
- Originating IP address: 85.208.139.60

### Phishing Indicators

- Suspicious sender identity
  - The sender claims to be **"Diplomatic agent Mr.Wood Forest"** and also an **"IMF AGENT"**.
  - These titles are not verifiable and are inconsistent with real diplomatic or IMF communication procedures.
  - The use of a personal Gmail address (`mywoodforestbiz[.]7[@]gmail[.]com`) is not legitimate for any official organization.

- Fraudulent financial claim
  - The email claims:
    - “consignment box of funds sum of $10.5 million USD”
  - This is a hallmark of an **advance-fee scam**
  - Legitimate financial institutions do not deliver cash via personal consignment or airport pickup.

- Urgency and pressure tactics
  - Phrases such as:
    - “Please hurry up”
    - “I do not want to deliver to a wrong destination”
  - These are designed to force quick action without verification.
  - This is a common **social engineering technique**.

- Suspicious contact method
  - Contact Email: `mywoodforestbiz[.]7[@]gmail[.]com`
  - Legitimate government, IMF, or diplomatic entities do not use Gmail for official transactions or fund delivery coordination.

- Personal information harvesting (PII theft attempt)
  - The email requests:
    - home address
    - current cell phone number
  - This is an attempt to collect **sensitive personal data** for fraud or further targeting.

- Implausible scenario
  - The claim of being at an airport with millions in cash is unrealistic.
  - International financial transfers do not occur through physical cash delivery at airports.

- Authority impersonation
  - Uses fake authority figures:
    - “Diplomatic agent”
    - “IMF AGENT”
  - These are used to create false trust and legitimacy.

- Lack of professionalism and structure
  - Informal writing style
  - Grammar inconsistencies
  - Lack of official formatting or domain usage
  - Legitimate international communications follow strict formal standards

- Advance-fee scam pattern
  - The message follows a known scam pattern:
    - Promise of large sum of money
    - Request for personal details
    - Implicit future fraud steps (fees, clearance, etc.)

- No official infrastructure
  - No government domain
  - No IMF domain
  - No verified organizational email system
  - All communication routed through a single Gmail account controlled by
 
### URL Analysis
- No URLs

### Attachment Analysis
- No Attachments

### IOC (Indicators of Compromise)
- Domains:
  - 54upr.rosreestr.ru

- IP Addresses:
  - 109.202.24.52
  - 85.208.139.60

- URLs:
  - None

- Attachments:
  - None 

- Email Addresses:
  - mywoodforestbiz[.]7[@]gmail[.]com
  - nemani[.]tukunia@postfiji[.]com[.]fj
 
### Social Engineering Techniques

- Authority impersonation:
  - The sender claims to be a “Diplomatic agent” and “IMF AGENT.”
  - This is used to create false legitimacy and pressure the victim into compliance.

- Fake financial reward (advance-fee scam):
  - The message promises “$10.5 million USD” in a consignment box.
  - This is designed to lure victims with unrealistic financial gain.

- Urgency and time pressure:
  - Phrases like “Please hurry up” and “I am at the airport right now” are used.
  - This discourages critical thinking and pushes immediate action.

- Fear of loss/mistake framing:
  - “I do not want to deliver to the wrong destination area.”
  - This creates anxiety that the victim might miss out or cause an error.

- Information harvesting (data extraction):
  - Requests for:
    - home address
    - current cell phone number
  - This is used to collect personally identifiable information (PII) for fraud.

- Direct contact manipulation:
  - Forces communication through a personal Gmail account (`mywoodforestbiz.7@gmail.com`).
  - Bypasses official channels to maintain control over the victim interaction.

- False sense of exclusivity:
  - The message implies the recipient is the intended beneficiary of a special delivery.
  - This increases trust and reduces skepticism.

- Urgent physical presence claim:
  - “I have just arrived… at the airport right now.”
  - Creates perceived immediacy and realism to pressure a quick response.

- Trust exploitation through official-sounding terms:
  - Uses terms like “consignment box,” “funds,” and “delivery.”
  - Mimics legitimate financial/legal processes to appear credible.

### Final Verdict
- **Classification:** Phishing 
