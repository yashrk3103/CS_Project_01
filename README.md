# 🔒 Vulnerability Scan Using Nessus Essentials – Task 3

This repository documents the vulnerability assessment conducted using **Nessus Essentials** as part of the Cyber Security Internship Task 3.

## 🎯 Scan Target

- **Target IPs:** `192.168.1.1`, `192.168.1.2`
- **Scanner IP:** `192.168.1.18`
- **Scan Type:** Basic Network Scan
- **Tool Used:** [Nessus Essentials](https://www.tenable.com/products/nessus/nessus-essentials)
- **OS Scanned:** Linux Kernel 2.6 and Linux Kernel 3.1

---

## 📝 Deliverables

- ✅ **Screen Recording** of Full Scanning Process (stored in `/recording/`)
- ✅ **Nessus Report** (PDF export in `/report/`)
- ✅ **README** file with answers to key interview questions

---

## 📊 Summary of Findings

| IP Address     | Critical | High | Medium | Low | Info |
|----------------|----------|------|--------|-----|------|
| 192.168.1.1    | 0        | 1    | 4      | 1   | 30   |
| 192.168.1.2    | 0        | 1    | 4      | 1   | 35   |

🛠 **Common Issues Identified:**
- SSL/TLS protocol vulnerabilities (e.g., TLS 1.0/1.1 support)
- Weak or expired SSL certificates
- DNS cache snooping
- ICMP timestamp disclosure
- Missing HSTS headers

---

## 🎥 Scanning Process

The complete vulnerability scan process — from launching Nessus, configuring the targets, to analyzing results — has been screen-recorded.  
You can find it under the `/recording/` directory as a `.mp4` file.

---

## 🔐 Interview Questions & Answers

### 1. What is vulnerability scanning?
Vulnerability scanning is the process of automatically detecting security weaknesses in systems, networks, or applications using tools like Nessus or OpenVAS.

---

### 2. Difference between vulnerability scanning and penetration testing?

| Category              | Vulnerability Scanning                  | Penetration Testing                      |
|----------------------|------------------------------------------|------------------------------------------|
| Method               | Automated                                | Manual/Semi-automated                    |
| Purpose              | Detect known vulnerabilities             | Exploit vulnerabilities to test security |
| Tools Used           | Nessus, OpenVAS                          | Metasploit, Burp Suite, etc.             |
| Depth                | Surface-level                            | In-depth                                |

---

### 3. What are some common vulnerabilities in personal computers?

- Outdated software
- Weak/default passwords
- SSL/TLS misconfigurations
- ICMP timestamp responses
- Insecure DNS server setups

---

### 4. How do scanners detect vulnerabilities?

By:
- Banner grabbing
- Port scanning
- Comparing system configs against known CVEs
- Using plugin feeds (like Nessus plugins)

---

### 5. What is CVSS?

**CVSS (Common Vulnerability Scoring System)** is a standard used to rate the severity of vulnerabilities, ranging from 0 (low) to 10 (critical). It considers exploitability, impact, and environmental metrics.

---

### 6. How often should vulnerability scans be performed?

- Monthly or quarterly (for regular IT systems)
- After significant updates or new deployments
- Weekly/daily (for critical infrastructures)

---

### 7. What is a false positive in vulnerability scanning?

A **false positive** occurs when a scanner reports a vulnerability that doesn't actually exist or is not exploitable in the environment being scanned.

---

### 8. How do you prioritize vulnerabilities?

- Based on **CVSS score**
- **Asset criticality** (is it public-facing? core infrastructure?)
- **Exploit availability**
- **Business impact** of the vulnerability

---


