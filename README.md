# 🔐 MyHackingNotes | Cybersecurity Knowledge Base

[![GitHub Last Commit](https://img.shields.io/github/last-commit/Majeed-GitHub/MyHackingNotes?label=Last%20Update&style=flat-square)](https://github.com/Majeed-GitHub/MyHackingNotes)
[![License](https://img.shields.io/badge/License-MIT-blueviolet?style=flat-square)](LICENSE)

**Practical penetration testing documentation** from TryHackMe & HackTheBox labs.  
**Structured Notes:** [📚 GitBook Version](https://jesusgavancho.gitbook.io/writeups/)

---

## 🗂️ Table of Contents
1. [Focus Areas](#-focus-areas)
2. [Repository Structure](#-repository-structure)
3. [Key Techniques](#-key-techniques)
4. [Getting Started](#-getting-started)
5. [Contribution Guide](#-contribution-guide)
6. [Legal Notice](#-legal-notice)
7. [License](#-license)

---

## 🎯 Focus Areas

### 🔥 Offensive Security
- **Privilege Escalation**  
  Linux/Windows escalation paths
- **Web Exploitation**  
  OWASP Top 10 vulnerabilities
- **AD Attacks**  
  Kerberoasting, Golden Tickets

### 🛡️ Defensive Security
- **Threat Hunting**  
  Sigma rules & detection logic
- **Forensics**  
  Memory analysis with Volatility
- **SIEM**  
  Splunk queries & alert configurations

### ⚙️ Tooling
- Nmap scripting engine
- Metasploit module development
- Burp Suite extensions

---

## 📂 Repository Structure
```text
MyHackingNotes/
├── Linux/
│   ├── Privilege_Escalation/
│   └── Kernel_Exploits/
├── Windows/
│   ├── AD_Attacks/
│   └── Registry_Abuse/
├── Web/
│   ├── SSRF/
│   └── XSS/
└── Tools/
    ├── Custom_Scripts/
    └── Cheatsheets/
```

---

## 🔑 Key Techniques
1. **Active Directory Compromise**  
   [`AD Certificate Templates.md`](Linux/AD_Attacks/AD_Certificate_Templates.md) - ESC1-ESC8 exploitation
2. **Linux Privilege Escalation**  
   [`Dirty Pipe.md`](Linux/Kernel_Exploits/Dirty_Pipe.md) - CVE-2022-0847 walkthrough
3. **Web Application Attacks**  
   [`SSRF.md`](Web/SSRF/SSRF_Exploitation.md) - Cloud metadata API exploitation

---

## 🚀 Getting Started
```bash
# Clone repository
git clone https://github.com/Majeed-GitHub/MyHackingNotes.git

# Search Windows techniques
grep -ri "windows" ./Windows/

# Find recent CVEs
find . -name "CVE-*" -mtime -30
```

**Recommended Tool Stack**:
```bash
pip install pwntools requests
sudo apt install seclists exploitdb
```

---

## 🤝 Contribution Guide
### Requirements
- Validate in isolated environments
- Anonymize lab IPs (10.10.x.x format)
- Reference MITRE ATT&CK framework

### Template
```markdown
## TTP: [Technique Name]
**ATT&CK ID**: [TXXXX]  
**Platform**: Windows/Linux/Web

### Execution Chain:
1. Initial Access:  
2. Privilege Escalation:  
3. Defense Evasion:

### Detection:
- Sigma Rule:  
- YARA Signature:
```

---

## ⚠️ Legal Notice
> **Warning**: Contains sensitive security information.  
> **Authorized Use Only** for:
> - ✅ Authorized penetration tests  
> - ✅ CTF competitions  
> - ✅ Academic research  
>
> **Strictly Prohibited**:  
> ❌ Unauthorized network scanning  
> ❌ Real-world exploitation  
> ❌ Malicious activities  

---

## 📜 License
Open-source under [MIT License](LICENSE)
```
