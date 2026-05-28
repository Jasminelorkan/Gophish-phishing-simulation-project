# Phishing Simulation Lab - Gophish

## Project Overview
Controlled phishing simulation built to understand social engineering attack vectorsand measure target susceptibility.
Conducted ethically against self-owned test accounts in an isolated environment.

## Environment
- Platform: Kali Linux
- Tool: GoPhish v0.11+
- Targets: 2 self-owned test email accounts
- Campaigns: Spotify, Qhack

## LIVE Screenshots
![Gophish Login][login-screenshot.png]
![Dashboard][dashboard-screenshot.png] 
![Campaign Setup][campaign-screenshot.png]

## Attack Chain
1. Created phishing email templates
2. Built credential harvesting landing pages
3. Configured SMTP sending profiles
4. Launched campaigns against test accounts
5. Monitored results via GoPhish dashboard

## Results
| Metric            | Count | Rate  |
|-------------------|-------|-------|
| Emails Sent       | 2     | 100%  |
| Emails Opened     | 2     | 100%  |
| Links Clicked     | 2     | 100%  |
| Credentials Stolen| 2     | 100%  |

## Attack Timeline
Email sent → Link clicked → Credentials submitted in under 60 seconds.
Target OS and browser fingerprinted automatically by GoPhish.

## Key Learnings
- Urgency-based email templates 
  significantly increase click rates
- Landing page similarity to real site
  is critical for credential submission
- GoPhish captures OS, browser, and
  timestamp of every interaction
- Users rarely verify sender email 
  addresses before clicking

## Ethical Notice
This simulation was conducted entirelyagainst self-owned accounts in a controlledlab environment. These techniques must never be used without explicit written permission from the target organization.

## Terminal Commands Used
```bash
# Start Gophish
sudo gophish
# OR if downloaded version
chmod +x gophish && ./gophish
#Admin Panel
https://127.0.0.1:3333

