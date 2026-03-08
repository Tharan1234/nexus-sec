<div align="center">

```
███╗   ██╗███████╗██╗  ██╗██╗   ██╗███████╗      ███████╗███████╗ ██████╗
████╗  ██║██╔════╝╚██╗██╔╝██║   ██║██╔════╝      ██╔════╝██╔════╝██╔════╝
██╔██╗ ██║█████╗   ╚███╔╝ ██║   ██║███████╗█████╗███████╗█████╗  ██║
██║╚██╗██║██╔══╝   ██╔██╗ ██║   ██║╚════██║╚════╝╚════██║██╔══╝  ██║
██║ ╚████║███████╗██╔╝ ██╗╚██████╔╝███████║      ███████║███████╗╚██████╗
╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝ ╚═════╝ ╚══════╝      ╚══════╝╚══════╝ ╚═════╝
```

**// SECURITY INTELLIGENCE PLATFORM v3.0**

[![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20Mac-green?style=for-the-badge&logo=linux)](https://github.com/Tharan1234/nexus-sec)
[![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python)](https://python.org)
[![Flask](https://img.shields.io/badge/Backend-Flask-red?style=for-the-badge&logo=flask)](https://flask.palletsprojects.com)
[![Tools](https://img.shields.io/badge/Security%20Tools-100+-brightgreen?style=for-the-badge)](https://github.com/Tharan1234/nexus-sec)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active%20Development-orange?style=for-the-badge)](https://github.com/Tharan1234/nexus-sec)

> **Free. Open Source. Built by a Pentester. For Pentesters.**

[Features](#features) • [Installation](#installation) • [Tools](#tool-arsenal) • [Screenshots](#screenshots) • [Author](#author)

</div>

---

## What is NEXUS-SEC?

NEXUS-SEC is a free, open-source security intelligence platform that consolidates **100+ professional security tools** into a single, unified interface. Built by a penetration tester after years of frustration switching between dozens of tools during real engagements.

**The problem it solves:**
Every pentester knows the pain — Subfinder in one terminal, Nmap in another, Burp Suite open, manual report in Word, CVE lookup in browser. Context switching kills efficiency.

**NEXUS-SEC brings everything into one place:**
- One platform for the entire pentest workflow
- Automated PDF reports with CVSS scoring
- Clean dark UI built for real engagements
- 100% free — no paywalls, no subscriptions

---

## Features

| Feature | Description |
|---|---|
| **100+ Security Tools** | Recon, Web, Network, OSINT, Cloud, Vulnerability |
| **Automated Reporting** | Professional PDF reports with CVSS scoring for every finding |
| **Security Grading** | A-F grade with score out of 100 for every scan |
| **CVE Matching** | Automatic CVE detection based on detected software versions |
| **OSINT Intelligence** | LinkedIn, GitHub, DNS, subdomain enumeration |
| **Cloud Security** | AWS & Azure misconfiguration detection |
| **Real-time Scanning** | Live scan progress with severity-color-coded results |
| **Scan History** | Full history of all past scans with downloadable reports |
| **Multi-tool Parallel** | Run multiple tools simultaneously in one scan |

---

## Screenshots

### Tool Arsenal — 100+ Security Tools
![NEXUS-SEC Tool Arsenal](screenshots/tool-arsenal.png)

### Security Assessment Report
![NEXUS-SEC Report](screenshots/sample-report.png)

---

## Tool Arsenal

### Recon & OSINT
`Subfinder` `Amass` `Assetfinder` `Findomain` `Chaos` `DNSx` `ShuffleDNS` `PureDNS` `AltDNS` `Knockpy` `Recon-ng` `theHarvester` `SpiderFoot` `Maltego` `Photon Crawler` `GAU` `Wayback URLs` `Hakrawler` `Katana` `Meg` `Aquatone` `EyeWitness` `Gowitness` `crt.sh CT Logs` `Shodan` `Censys` `SecurityTrails` `LeakIX` `ZoomEye`

### Network
`Nmap` `Masscan` `RustScan` `Naabu` `ZMap` `Unicornscan` `Netdiscover` `ARP-Scan` `FPing` `Hping3`

### Web Vulnerability
`Nuclei` `Nikto` `WhatWeb` `Wappalyzer` `HTTPX` `FFUF` `Dirsearch` `Gobuster` `WFuzz` `Feroxbuster` `DIRB` `DirBuster` `Dalfox (XSS)` `SQLMap` `BuiltWith` `Nuclei Tech Detect`

### Cloud Security
- Subdomain takeover detection
- S3 bucket exposure analysis
- GitHub secret scanning
- CORS misconfiguration detection
- JWT token analysis & auth bypass
- AWS & Azure misconfiguration detection

### Reporting
- Automated PDF generation
- CVSS scoring per finding
- Executive summary
- Remediation roadmap
- Security grade (A-F) + score (0-100)

---

## Installation

### Requirements
- Python 3.8+
- Linux / macOS
- pip

### Quick Start

```bash
# Clone the repository
git clone https://github.com/Tharan1234/nexus-sec.git
cd nexus-sec

# Create virtual environment
python3 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run NEXUS-SEC
python app.py
```

Open your browser → `http://localhost:5000`

### Install Security Tools

```bash
# Install Go-based tools
go install github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest
go install github.com/projectdiscovery/nuclei/v3/cmd/nuclei@latest
go install github.com/projectdiscovery/naabu/v2/cmd/naabu@latest
go install github.com/projectdiscovery/httpx/cmd/httpx@latest

# Install system tools
sudo apt install nmap nikto dirb -y

# Install Python tools
pip install shodan requests dnspython
```

---

## Sample Report

NEXUS-SEC generates professional PDF security reports with:

```
TARGET: example.com
SECURITY GRADE: C (54/100)

FINDINGS:
├── CRITICAL (2)  → MongoDB exposed, API key in GitHub
├── HIGH    (5)  → TLS 1.0/1.1, Missing headers, XML-RPC
├── MEDIUM  (8)  → CSP missing, CORS wildcard, Cookies
├── LOW     (6)  → Version disclosure, Weak ciphers
└── INFO    (4)  → Technology stack, DNS records
```

---

## Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python / Flask |
| Frontend | HTML, CSS, JavaScript |
| Database | SQLite / PostgreSQL |
| PDF Generation | ReportLab |
| Security Tools | Nmap, Subfinder, Nuclei + 97 more |

---

## Roadmap

- [x] Port scanning (Nmap)
- [x] Subdomain enumeration (Subfinder)
- [x] SSL/TLS audit
- [x] HTTP header analysis
- [x] PDF report generation with CVSS scoring
- [x] 100+ tool arsenal UI
- [ ] Active Directory enumeration
- [ ] BloodHound integration
- [ ] Full nuclei integration
- [ ] Docker deployment
- [ ] API support

---

## Disclaimer

> NEXUS-SEC is built for **authorized security testing only**.
> Only scan systems you own or have explicit written permission to test.
> The author is not responsible for any misuse of this tool.
> All scans must comply with applicable laws and regulations.

---

## Author

**Tharani Tharan** — Penetration Tester & Security Engineer

- 4 Years VAPT Experience
- CEH Certified | OSCP In Progress (2026)
- 50+ Real-world Security Engagements
- Bengaluru, India

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/tharan-anandan-459860200)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-green?style=for-the-badge)](https://tharan.netlify.app)
[![Email](https://img.shields.io/badge/Email-Contact-red?style=for-the-badge&logo=gmail)](mailto:tharananandh19@gmail.com)

---

<div align="center">

**If NEXUS-SEC helped you — give it a ⭐ Star!**

*Built with 6 months of late nights by a pentester who needed this tool to exist.*

</div>
