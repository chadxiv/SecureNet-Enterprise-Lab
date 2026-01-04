# SecureNet: Layered Defense Architecture
A comprehensive enterprise security lab focused on defense-in-depth, centralized monitoring, and automated patch management.

**Project Impact:** Shifted to an open-source security stack, achieving an 85% risk reduction (exceeding commercial estimates) and exponentially improving ROI through automation.

## Network Architecture
<img width="1023" height="1152" alt="image" src="https://github.com/user-attachments/assets/9d707017-394c-4c77-a923-66fe6d851b7f" />


## 🛠️ Tech Stack
* **Firewall/Routing:** pfSense (Network Segmentation & VLANs)
* **SIEM/Monitoring:** Splunk (Centralized Log Analysis)
* **Identity & Updates:** Windows Server (AD & WSUS)
* **Automation:** Ansible (Patch Management)
* **Vulnerability Management:** Nessus
* **Infrastructure:** Ubuntu Servers (DMZ), Kali Linux (Adversarial Testing)

## 🏗️ Project Overview
This project simulates a corporate environment with segmented networks (DMZ, LAN, Management). The goal was to build a resilient infrastructure that can detect and mitigate common attack vectors.

### Key Features
- **Network Segmentation:** Isolated public-facing services in a DMZ using pfSense rules.
- **Automated Security:** Implemented Ansible playbooks for automated Linux patching.
- **Centralized Logging:** Configured Splunk to ingest logs from pfSense and Windows endpoints for real-time alerting.
- **Hardening:** Applied security benchmarks to Windows and Ubuntu systems to reduce the attack surface.

## Vulnerability Management: 
I used Nessus to identify critical SSL/TLS weaknesses and verified their remediation after hardening the DMZ servers.

First Scan
<img width="1943" height="1158" alt="image" src="https://github.com/user-attachments/assets/46a6287d-3c7a-404f-9972-c2b8579432e5" />


Second Scan
<img width="2015" height="1087" alt="image" src="https://github.com/user-attachments/assets/d39db441-b4d4-47e3-9f02-80367954ec19" />


## Security Monitoring (Splunk)
<img width="1508" height="1155" alt="image" src="https://github.com/user-attachments/assets/c42e41bc-86bd-4710-a237-f0061bbd8fba" />


## 🛡️ Methodology & Validation
Validated the architecture by performing:
1. **Nessus Scans:** Identified and remediated vulnerabilities.
2. **Adversarial Simulation:** Attempted lateral movement from the external network to test pfSense firewall rules.

> **Note:** All testing was performed in an isolated virtual lab environment. IP addresses shown in documentation (192.168.x.x) are non-routable internal addresses.

