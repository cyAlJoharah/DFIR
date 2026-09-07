# Digital Forensics & Incident Response

This repository documents a series of case studies completed as part of the 
Incident Response Analysis training program - STC via Misk, covering Incident 
Triage & Containment, Digital Artifact Analysis, and Root Cause Analysis.

The goal of this repository is to document my hands-on approach to investigating 
security incidents, analyzing digital evidence, and developing evidence-based 
conclusions.

**Note**: This repository is an active draft. The overall structure, incident 
organization, and documentation are currently under development and subject to 
change.

## About Me

I'm AlJoharah AlQahtani, a Cybersecurity Diploma graduate and CompTIA Security+ 
certified professional with a strong interest in security analysis, particularly 
Digital Forensics and Incident Response.

This repository reflects my hands-on practice in analyzing evidence, investigating 
incidents, and applying a structured DFIR mindset to real-world-inspired cases.

## Certification
Completion certificate for the training program this repository's case studies 
are drawn from.

[Incident Response Analysis – STC via Misk](./Certificate_IR_Analysis_STC_Misk.pdf)


## Cases

## **Case 01 — Proxy Analysis**

Triage of Blue Coat proxy logs to investigate suspected phishing and account 
compromise for user `Fahad3315`.

Findings were circumstantial and inconclusive on compromise, highlighting the 
evidentiary gap between proxy telemetry and the claimed email-based attack.

**Tools:** Splunk

* [Report](./01_Proxy_Analysis_Report.pdf)
* [Raw Logs (CSV)](./01_Proxy_Analysis_Evidence.csv)


## **Case 02 — Phishing & Macro Analysis**

Forensic deconstruction of a carrier email (`.msg`) and macro-enabled attachments (`.xlsm`) to investigate an internal spear-phishing simulation. 

Findings conclusively identified an authorized internal simulation: low-level MAPI property interrogation verified direct internal MAPI/RPC store delivery (`PR_TRANSPORT_MESSAGE_HEADERS = None`), while cross-sample VBA reverse engineering confirmed an educational, non-destructive payload.

**Tools:** `oledump.py`, `extract-msg`, `binwalk`, `strings`

* [Report](./02_Phishing_and_Macro_Analysis_Report.pdf)
* [Analyzed Samples (ZIP, Password: infected)](./02_Phishing_and_Macro_Evidence/)


## Contact

[LinkedIn](https://www.linkedin.com/in/aljoharah-cyber) · [Email](mailto:cs.alqahtani@gmail.com) · [WhatsApp](https://wa.me/966530995052)
