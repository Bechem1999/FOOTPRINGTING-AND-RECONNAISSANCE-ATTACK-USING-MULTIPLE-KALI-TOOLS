<div align="center">

# 🔎 FOOTPRINTING & RECONNAISSANCE

### Multiple Kali Linux Tools | Cybersecurity & Ethical Hacking

[![Kali Linux](https://img.shields.io/badge/Kali_Linux-Security_Lab-557C94?logo=kalilinux&logoColor=white)](#)
[![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Reconnaissance-0A66C2)](#)
[![Ethical Hacking](https://img.shields.io/badge/Ethical_Hacking-Authorized_Testing-DC143C)](#)
[![Linux](https://img.shields.io/badge/Linux-Command_Line-FCC624?logo=linux&logoColor=black)](#)
[![WHOIS](https://img.shields.io/badge/WHOIS-Domain_Reconnaissance-2E8B57)](#)
[![WhatWeb](https://img.shields.io/badge/WhatWeb-Web_Fingerprinting-8A2BE2)](#)
[![DNS](https://img.shields.io/badge/DNS-Enumeration-008B8B)](#)
[![HTTP](https://img.shields.io/badge/HTTP-Header_Analysis-FF8C00)](#)
[![WAF](https://img.shields.io/badge/WAF-Detection-B22222)](#)
[![DNSRecon](https://img.shields.io/badge/DNSRecon-DNS_Records-4682B4)](#)
[![GitHub](https://img.shields.io/badge/GitHub-Project_Documentation-181717?logo=github&logoColor=white)](#)

</div>

# 📖 Project Overview

This repository documents a practical footprinting and reconnaissance exercise conducted using multiple tools available in Kali Linux.

The purpose of the exercise was to understand how publicly accessible information can be collected from a web target and combined to develop an initial picture of its domain, DNS infrastructure, web technologies, HTTP configuration, and defensive controls.

The exercise follows a six-tool reconnaissance workflow using:

WHOIS → WhatWeb → Nslookup → Curl → Wafw00f → Dnsrecon

The project briefly describes reconnaissance as an initial stage of security assessment and emphasizes careful documentation of the information collected

# 🎯 Objectives

The assessment was designed to:

Identify publicly available domain registration information
Fingerprint technologies used by a web application
Resolve a domain name to an IP address
Analyse HTTP response headers
Identify whether a Web Application Firewall is present
Enumerate publicly available DNS records
Document reconnaissance results for further analysis

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| `whois` | Retrieves domain registration and ownership information |
| `whatweb` | Identifies web technologies, CMS, plugins and server information |
| `nslookup` | Resolves domain names to IP addresses |
| `curl` | Examines HTTP response headers |
| `wafw00f` | Detects Web Application Firewalls |
| `dnsrecon` | Enumerates DNS records and infrastructure |

## 🧠 Skills Demonstrated

| Category | Skills |
|---|---|
| 🐧 **Linux** | Kali Linux, Linux terminal, command-line operations |
| 🔎 **Reconnaissance** | Footprinting, passive information gathering, target profiling |
| 🌐 **DNS Analysis** | Domain resolution, DNS records, name servers, mail records |
| 🕸️ **Web Reconnaissance** | Web technology fingerprinting and HTTP analysis |
| 🛡️ **WAF Analysis** | Web Application Firewall detection |
| 📊 **Technical Analysis** | Output interpretation, evidence collection and documentation |
| 📝 **Reporting** | Screenshots, saved outputs and structured technical reporting |
| ⚖️ **Ethical Hacking** | Authorized reconnaissance and controlled security testing |

## 🔬 Methodology


                 TARGET DOMAIN
                       │
                       ▼
                  ┌─────────┐
                  │  WHOIS  │
                  └────┬────┘
                       ▼
                 ┌───────────┐
                 │  WHATWEB  │
                 └─────┬─────┘
                       ▼
                 ┌───────────┐
                 │ NSLOOKUP  │
                 └─────┬─────┘
                       ▼
                 ┌───────────┐
                 │   CURL    │
                 └─────┬─────┘
                       ▼
                 ┌───────────┐
                 │ WAFW00F   │
                 └─────┬─────┘
                       ▼
                 ┌───────────┐
                 │ DNSRECON  │
                 └─────┬─────┘
                       ▼
             RECONNAISSANCE PROFILE

# 🧪 Lab Environment

**Operating System:** Kali Linux  
**Assessment Type:** Footprinting / Reconnaissance  
**Target:** Authorized training/lab domain  
**Purpose:** Educational cybersecurity and ethical hacking


# 🔹Task 1: WHOIS Enumeration

# Objective

Obtain publicly available domain registration information, including registrar information, registration dates and name servers.

Command
# whois <target-domain>
Information Gathered

WHOIS can provide information such as:

- Domain registrar
- Registration date
- Expiration date
- Name servers
- Domain status
- Administrative or technical information where publicly available

<img width="1317" height="805" alt="whois" src="https://github.com/user-attachments/assets/7e8f0030-0df0-4807-af2f-20bb307ebda4" />

# 🔹 Task 2: Web Technology Fingerprinting with WhatWeb
# Objective

Identify technologies used by the target website.

Command
whatweb <target-domain>
Information Gathered

WhatWeb can help identify:

- Web server technologies
- Content Management Systems
- Plugins
- Frameworks
- Software versions
- IP-related information
- Other publicly exposed technologies

  <img width="1287" height="252" alt="whatweb command" src="https://github.com/user-attachments/assets/5a3bb2dd-5ac8-4c07-8c51-bf6e54519686" />
