<div align="center">

<img src="./assets/ChellTools.png" width="110" alt="ChellSpace Logo" />

# CHELL HORUS
### Advanced Web Security & Vulnerability Audit Engine
**Author: Marchell Adi Pratama • ChellSpace Security Labs**

[![Visitors](https://komarev.com/ghpvc/?username=MarchellProGit-ChellHorus&color=0080FF&style=for-the-badge&label=VISITORS)](https://github.com/MarchellProGit/ChellHorus)
[![Repo Size](https://img.shields.io/github/repo-size/MarchellProGit/ChellHorus?style=for-the-badge&color=38BDF8)](https://github.com/MarchellProGit/ChellHorus)
[![Build](https://img.shields.io/badge/Build-v1.0.0--PROD-00F0FF?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/MarchellProGit/ChellHorus/releases)
[![Platform](https://img.shields.io/badge/Platform-Windows_10%2F11_x64-38BDF8?style=for-the-badge&logo=windows11&logoColor=white)](https://github.com/MarchellProGit/ChellHorus/releases)
[![License](https://img.shields.io/badge/License-Proprietary_EULA-38BDF8?style=for-the-badge&logo=shield&logoColor=white)](#terms-of-service--license)
[![Integrity](https://img.shields.io/badge/Security-SHA256_Verified-10B981?style=for-the-badge&logo=security&logoColor=white)](#security--integrity)

---

</div>

## Executive Summary

**ChellHorus** is an enterprise-grade multi-threaded web security scanner, reconnaissance suite, and vulnerability audit engine built for penetration testers, security researchers, and DevOps engineers.

Engineered with asynchronous payload mutation, multi-threaded port scanning, subdomain enumeration, SSL/TLS handshake verification, dynamic vulnerability scoring (CVSS v3.1 & CWE cataloging), and automated ReportLab PDF report generation, ChellHorus serves as a core security audit module within the ChellSpace desktop security ecosystem.

---

## Authentication & Access Protocol

> **Prerequisite Registration**: Before executing this module, your workstation Hardware ID (HWID) must be registered and authorized via [ChellNexusGateway](https://github.com/MarchellProGit/ChellNexusGateway).

### Step 1: Workstation Registration via Nexus Gateway
1. Download and launch [ChellNexusGateway](https://github.com/MarchellProGit/ChellNexusGateway/releases).
2. Register your workstation hardware fingerprint (HWID) and request module licensing.
3. Verify that your account profile contains active authorization for the `HORUS_SCANNER` module.

### Step 2: Module Execution & License Verification
1. Download `ChellHorus_ChellSpace.exe` from the official [Releases](https://github.com/MarchellProGit/ChellHorus/releases) page.
2. Enter your System Access Key (`SOLI DEO GLORIA`) in the authentication prompt.
3. The system validates your HWID and `HORUS_SCANNER` entitlement against the cloud database.
4. Upon successful verification (`ACCESS GRANTED`), the main security workstation console will initialize automatically.

---

## Key Features

- **[ ✦ ] Reconnaissance & Intelligence**: Active banner grabbing, security header validation, DNS record lookup (`A`, `MX`, `NS`, `TXT`, `SOA`, `AAAA`), and domain structure extraction.
- **[ ✦ ] Subdomain Brute-Forcing**: High-concurrency threaded subdomain discovery using optimized DNS resolvers.
- **[ ✦ ] Port & Service Scanner**: Multi-threaded socket scanner mapping open ports, active services, and banner responses across standard ports.
- **[ ✦ ] Tech Stack Fingerprinting**: Automated CMS, web server, and backend framework detection (WordPress, Django, Laravel, React, Vue, Nginx, Apache).
- **[ ✦ ] Content & Asset Discovery**: Automated indexing of `robots.txt`, `sitemap.xml`, exposed `.git`/`.env` repositories, and API endpoints.
- **[ ✦ ] Payload Fuzzer & Vulnerability Matrix**: Advanced fuzzer detecting SQL Injection, XSS, LFI, Command Injection, SSRF, and SSTI with intelligent payload mutations.
- **[ ✦ ] SSL/TLS Security Audit**: Comprehensive certificate expiration tracking, cipher strength evaluation, and protocol compliance checking.
- **[ ✦ ] Real-Time Visual Analytics**: Embedded Matplotlib vulnerability breakdown charts, risk metrics gauge (CVSS 0.0 - 10.0), and execution timeline analytics.
- **[ ✦ ] Multi-Format Report Generator**: Automated PDF audit report synthesis (ReportLab), JSON data exports, and CSV table extractions.

---

## System Architecture

```text
+-----------------------+      +------------------------+      +------------------------+
| Audit Console         | ---> | Payload Fuzzer &       | ---> | Target Infrastructure  |
| (ChellHorus.exe)      |      | Concurrency Engine     |      | (Web / API / Network)  |
+-----------------------+      +------------------------+      +------------------------+
            |                               |
            v                               v
+-----------------------+      +------------------------+
| License Verification  |      | Analytics & Reporting  |
| (Supabase Cloud API)  |      | (PDF / JSON / SQLite)  |
+-----------------------+      +------------------------+
```

---

## Technical Specifications

| Core Attribute | Implementation Details | Rating |
| :--- | :--- | :---: |
| **Concurrency Model** | ThreadPoolExecutor supporting up to 200 parallel workers | Critical |
| **GUI Framework** | CustomTkinter dark cyber theme (`#00F0FF` accent) | High |
| **Vulnerability Scoring** | Dynamic CVSS v3.1 calculator & CWE ID cataloging | Critical |
| **Data Persistence** | SQLite connection pool with WAL journal mode | High |
| **Report Generation** | Automated ReportLab PDF & JSON/CSV exporter | High |
| **License Validation** | REST API HWID authentication against Supabase cloud | Critical |

---
## System Requirements

| Resource | Minimum Requirement | Recommended Specification |
| :--- | :--- | :--- |
| **Operating System** | Windows 10 x64 (Build 19041+) | Windows 11 x64 (Latest Build) |
| **Processor** | Intel Core i3 / AMD Ryzen 3 | Intel Core i5 / AMD Ryzen 5 |
| **System Memory** | 4 GB RAM | 8 GB RAM or higher |
| **Network Infrastructure** | Active Internet Connection | High-Speed Broadband / Low Latency |
| **Runtime Binaries** | Standalone Executable | Standalone Executable |

---

## Binary Release Distribution

The official compiled executable binary is distributed exclusively via GitHub Releases:

- **Official Release Download**: [ChellHorus_ChellSpace.exe (v1.0.0-PROD)](https://github.com/MarchellProGit/ChellHorus/releases/tag/v1.0.0)

---

## Security & Integrity Verification

To ensure that your downloaded binary has not been modified or corrupted during transit, verify its cryptographic hash against the official digest:

```text
File Name : ChellHorus_ChellSpace.exe
Algorithm : SHA-256
Checksum  : 832944176ba667d48c7349a393bbb627dbfdd8fe40b70512003b12aa5683f98b
Status    : Verified Clean (ChellSpace Security Labs)
```

---

## Terms of Service & License

Copyright (C) 2026 Marchell Adi Pratama • ChellSpace Ecosystem. All Rights Reserved.

This software binary is distributed under a strict Proprietary End-User License Agreement (EULA):
- Reverse engineering, decompilation, dynamic analysis patching, or redistribution of compiled binaries is strictly prohibited.
- Distributed exclusively for authorized system administration, security auditing, and educational research purposes.

---

<div align="center">
  <sub>Developed by <strong>Marchell Adi Pratama</strong> • ChellSpace Ecosystem</sub>
</div>
