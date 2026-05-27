# 🛡️ Phishing Email Detection & Awareness Report

![Track](https://img.shields.io/badge/Track-Cyber%20Security-blue)
![Task](https://img.shields.io/badge/Task-02-orange)
![Internship](https://img.shields.io/badge/Internship-Future%20Interns-yellow)
![Status](https://img.shields.io/badge/Status-Completed-green)

---

## 📌 About This Project

This project was completed as part of the **Future Interns Cyber Security Internship — Task 2 (2026)**.

It involves analyzing real phishing email samples, identifying phishing indicators,
classifying email risk levels, and producing a professional awareness report
that can be used by employees and organizations to protect against phishing attacks.

> ⚠️ This is purely defensive security education — no hacking or illegal activity involved.

---

## 🎯 Objective

- Analyze real phishing email samples collected from public repositories
- Identify common phishing indicators in headers, body, and URLs
- Classify each email by risk level (Safe / Suspicious / Phishing)
- Explain how phishing attacks work in simple, non-technical language
- Create a professional awareness report with prevention guidelines

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| Kali Linux — `grep` | Extract headers and URLs from raw .eml files |
| Kali Linux — `dig` | DNS/SPF/DKIM/DMARC record lookup |
| Kali Linux — `whois` | IP and domain investigation |
| MXToolbox | Professional email header analysis |
| VirusTotal | URL and IP reputation scanning |
| URLScan.io | Safe URL inspection and DNS check |
| WHOIS (whois.com) | Domain registration date and owner lookup |
| MS Word + PDF | Professional report creation |

---

## 🔍 Analysis Approach
Step 1 → Collected phishing .eml samples from public GitHub repositories
Step 2 → Extracted raw email headers using grep in Kali Linux terminal
Step 3 → Analyzed headers using MXToolbox (SPF, DKIM, DMARC results)
Step 4 → Performed DNS lookups using dig to verify authentication records
Step 5 → Investigated sender domains and IPs using whois and WHOIS website
Step 6 → Extracted and scanned URLs safely using VirusTotal and URLScan.io
Step 7 → Identified phishing indicators using a structured 10-point checklist
Step 8 → Classified each email by risk level based on confirmed indicators
Step 9 → Documented all findings in a professional PDF report

---

## 📁 Folder Structure
FUTURE_CS_02/
│
├── 📁 samples/             → Raw phishing email files analyzed (.eml)
│     ├── sample1.eml       → Fake Fax Notification (MetroFax Scam)
│     ├── sample2.eml       → Fake Voicemail Notification
│     └── sample3.txt       → Account Suspension Warning
│
├── 📁 analysis/            → Extracted findings from each sample
│     ├── sample1_headers.txt
│     ├── sample1_dns.txt
│     ├── sample1_urls.txt
│     ├── sample1_indicators.txt
│     ├── sample2_headers.txt
│     ├── sample2_dns.txt
│     ├── sample2_whois_ip.txt
│     ├── sample2_urls.txt
│     └── sample2_indicators.txt
│
├── 📁 screenshots/         → Evidence screenshots from all tools
│     ├── sample1_mxtoolbox.png
│     ├── sample1_virustotal.png
│     ├── sample1_urlscan.png
│     ├── sample1_whois.png
│     ├── sample2_mxtoolbox.png
│     └── sample2_virustotal_ip.png
│
├── 📁 report/              → Final deliverable
│     └── Phishing_Awareness_Report_FutureInterns_2026.pdf
│
└── 📄 README.md            → Project overview (this file)

---

## 📊 Risk Classification Results

| Sample | Attack Type | Indicators Found | Classification |
|--------|------------|-----------------|----------------|
| Sample 1 | Fake Fax Notification (MetroFax) | 8/10 | 🚨 PHISHING |
| Sample 2 | Fake Voicemail + Malicious Attachment | 9/10 | 🚨 PHISHING |
| Sample 3 | Account Suspension Warning | 8/10 | 🚨 PHISHING |

---

## 🔎 Key Findings

### Sample 1 — Fake Fax Notification
- Sender: `attack@attacker.example.com`
- Impersonates MetroFax and SharePoint
- Malicious URL: `https://attacker.example.com/`
- To: Undisclosed recipients (mass phishing)
- No SPF or DKIM authentication configured

### Sample 2 — Fake Voicemail Notification
- SPF: FAILED | DKIM: NONE | DMARC: FAILED
- Unauthorized sender IP: 192.0.2.1 (reserved IP)
- Unicode tricks used to bypass spam filters
- Malicious attachment disguised as voicemail file
- Unfilled placeholder left in email body

### Sample 3 — Account Suspension Warning
- Urgency and fear-based language used
- Generic greeting: "Dear User"
- Reply-To points to .ru domain
- Credential harvesting via fake login page
- No SPF or DKIM records on sender domain

---

## 🚨 Phishing Indicators Checklist
[✔] Spoofed or fake sender domain
[✔] Failed SPF / DKIM / DMARC authentication
[✔] Urgency and fear-based language
[✔] Generic greeting (Dear User)
[✔] Suspicious or malicious URLs
[✔] Malicious attachments
[✔] Brand impersonation
[✔] Reply-To mismatch
[✔] Mass recipient list (Undisclosed recipients)
[✔] Unicode character tricks to bypass spam filters

---

## 🛡️ Prevention Tips
✔ Always verify the sender email domain before clicking
✔ Never click links in unexpected emails
✔ Enable Multi-Factor Authentication (MFA) on all accounts
✔ Report suspicious emails to your IT/security team
✔ Never download attachments from unknown senders
✔ Hover over links to preview the real destination URL
✔ Check for urgency — it is a manipulation tactic
✔ Never share OTPs or passwords over email or phone

---

## 📄 Deliverables

- ✅ Phishing Detection & Awareness Report (PDF)
- ✅ Raw phishing email samples (.eml files)
- ✅ Header, DNS, WHOIS, URL analysis files
- ✅ Evidence screenshots from all tools
- ✅ Structured indicator checklists per sample

---

## 🎓 Internship Details

| Detail | Info |
|--------|------|
| Organization | Future Interns |
| Track | Cyber Security |
| Track Code | CS |
| Task Number | 02 |
| Repository | FUTURE_CS_02 |
| Completed | May 2026 |

---

## 🔗 References

- [Phishing Mail Examples Repository](https://github.com/autinerd/phishing-mail-examples)
- [Phishing Pot Repository](https://github.com/rf-peixoto/phishing_pot)
- [MXToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- [VirusTotal](https://www.virustotal.com)
- [URLScan.io](https://urlscan.io)

---

*Report prepared as part of Future Interns Cyber Security Internship — Task 2 — May 2026*
