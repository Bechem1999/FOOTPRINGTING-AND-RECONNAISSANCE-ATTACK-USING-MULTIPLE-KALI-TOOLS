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

# 🔹 Task 3: DNS Resolution with Nslookup
# Objective

Resolve the target domain name and identify its associated IP address.

Command
nslookup <target-domain>
Information Gathered

The command can reveal:

- Domain IP address
- DNS server information
- Address records
- Other DNS resolution details

  <img width="1367" height="147" alt="nslookup command" src="https://github.com/user-attachments/assets/1860dd36-559f-473c-a06f-f26507b0e0b6" />


# 🔹 Task 4: HTTP Header Analysis with Curl
# Objective

Inspect the HTTP response headers returned by the target web server.

Command
curl -I https://<target-domain>
Information Gathered

HTTP headers may reveal information such as:

- HTTP status codes
- Server information
- Cookies
- Redirects
- Caching behaviour
- Security-related headers
- Publicly exposed endpoints

  <img width="1387" height="235" alt="curl command" src="https://github.com/user-attachments/assets/07c874d4-7221-41d3-94f0-9245903ecd07" />

 # 🔹 Task 5: Web Application Firewall Detection
# Objective

Determine whether a Web Application Firewall (WAF) is protecting the target website.

Command
wafw00f <target-domain>
Information Gathered

Wafw00f attempts to identify whether a WAF is present and, where possible, identifies the WAF technology.

Understanding defensive controls is an important part of security assessment because it helps security professionals understand how web traffic is being filtered and protected. 

<img width="1022" height="252" alt="wafw00f command" src="https://github.com/user-attachments/assets/150680cb-13af-4c85-87f3-96aebc5d4d69" />

# 🔹 Task 6: DNS Enumeration with Dnsrecon
# Objective

Enumerate publicly available DNS records associated with the target domain.

Command
dnsrecon -d <target-domain>
Information Gathered

DNS reconnaissance can reveal:

- Name servers
- Mail servers
- A records
- TXT records
- SPF information
- SRV records
- Other publicly available DNS information

 # 🧠 Key Learning Outcomes

Through this project, I gained practical experience in:

- Performing domain reconnaissance
- Using Kali Linux reconnaissance tools
- Understanding DNS infrastructure
- Identifying web technologies
- Analysing HTTP response headers
- Detecting web application firewalls
- Interpreting publicly available information
- Documenting reconnaissance results
- Understanding how reconnaissance contributes to security assessments

  # 🔐 Security Perspective

Footprinting demonstrates how much information an organization can unintentionally expose through publicly accessible services.

From a defensive cybersecurity perspective, the same techniques can be used to audit an organization's external footprint and identify information that could potentially assist an attacker.

Reducing unnecessary information exposure can make later stages of an attack more difficult.

## ⚠️ Challenge Faced

During the reconnaissance exercises, I encountered a challenge when trying to **save the outputs generated by some of the Kali Linux reconnaissance tools into a `.txt` file** for proper documentation and later analysis. Although the commands were executing successfully in the terminal, I initially had difficulty understanding how to redirect and preserve their outputs in the required text format.

### 💡 How I Resolved It

I used my knowledge of **AI-assisted learning and troubleshooting** to understand the problem and identify the appropriate Linux output-redirection techniques. With this guidance, I learned how to use the `>` and `>>` operators to save command outputs directly into `.txt` files.

For example:

```bash
whois example.com > whois_output.txt
```

This saves the command output into a new text file.

For adding additional output without overwriting existing content:

```bash
whois example.com >> reconnaissance_results.txt
```

I also learned to combine the reconnaissance commands with output redirection so that the results could be systematically documented and reviewed later.

This experience helped me understand not only **how to solve the immediate problem**, but also how to independently troubleshoot Linux command-line challenges using AI as a learning and problem-solving assistant.

> **Key Lesson:** AI was used as a learning and troubleshooting aid, while the commands were tested and verified in my own Kali Linux lab environment.

<img width="1562" height="802" alt="output saved in a text file" src="https://github.com/user-attachments/assets/8c1bae30-452f-4052-932a-e7f4abbcb6f3" 

  # 🔐 Security & Ethical Use
This lab is strictly for education purposes only.

 # 👤 Author
  Atemlefac Nkafu Bechem
  
  Cybersecurity Engineer

LinkedIn: https://www.linkedin.com/in/atemlefac-nkafu-bechem-179987248

# 📌 Project Information
**Program Name:** Cybersecurity at Networkwalks | **Week:** 02 | **Project:** Footprinting and reconnaissance attack using multiple kali tools | **Repository:** GitHub


