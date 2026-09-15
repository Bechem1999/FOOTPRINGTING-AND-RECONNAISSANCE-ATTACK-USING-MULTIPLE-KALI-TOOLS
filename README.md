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

# 🛠️ Tools Used
# Tool	          Purpose
whois	            Retrieves domain registration and ownership information
whatweb	          Identifies web technologies, CMS, plugins and server information
nslookup          Resolves domain names to IP addresses
curl	            Examines HTTP response headers
wafw00f	          Detects Web Application Firewalls
dnsrecon	        Enumerates DNS records and infrastructure
