# OSCP Practice Reports & Walkthroughs

A collection of penetration testing practice reports, machine walkthroughs, and technical notes created while preparing for the **Offensive Security Certified Professional (OSCP)** certification.

The goal of this repository is to document practical penetration testing methodology, improve technical writing, and create a reference for common techniques encountered during OSCP-style engagements.

> **Disclaimer:** This repository is an independent educational project and is not affiliated with, endorsed by, or sponsored by Offensive Security. All content is based on intentionally vulnerable practice machines, labs, CTFs, and personal research.

---

## 🎯 Purpose

This repository serves as a personal knowledge base and portfolio demonstrating practical penetration testing skills.

The reports focus on the complete penetration testing process, including:

* Reconnaissance
* Enumeration
* Vulnerability identification
* Initial access
* Exploitation
* Privilege escalation
* Credential discovery
* Lateral movement
* Post-exploitation
* Proof of concept development
* Documentation and reporting

The emphasis is on **understanding methodology rather than simply obtaining flags or shells**.

---

## 📂 Repository Structure

```text
.
├── machines/
│   ├── machine-name/
│   │   ├── README.md
│   │   ├── enumeration.md
│   │   ├── exploitation.md
│   │   ├── privilege-escalation.md
│   │   └── images/
│   │
│   └── another-machine/
│       └── ...
│
├── notes/
│   ├── enumeration/
│   ├── privilege-escalation/
│   ├── web/
│   ├── linux/
│   └── windows/
│
├── cheatsheets/
│   ├── linux.md
│   ├── windows.md
│   ├── web.md
│   └── enumeration.md
│
└── README.md
```

The structure may evolve as additional machines and techniques are documented.

---

## 🖥️ Practice Machines

Each machine is documented using a methodology similar to a professional penetration testing engagement.

Typical reports include:

1. **Target identification**
2. **Reconnaissance**
3. **Port and service enumeration**
4. **Web application enumeration**
5. **Vulnerability analysis**
6. **Initial foothold**
7. **Privilege escalation**
8. **Proof of compromise**
9. **Lessons learned**

Example:

```text
machines/
└── example-machine/
    ├── README.md
    ├── enumeration.md
    ├── exploitation.md
    ├── privilege-escalation.md
    └── images/
```

---

## 🔎 Methodology

The general workflow used throughout these reports follows a penetration testing methodology:

```text
Reconnaissance
      │
      ▼
Enumeration
      │
      ▼
Vulnerability Identification
      │
      ▼
Initial Access
      │
      ▼
Privilege Escalation
      │
      ▼
Post-Exploitation
      │
      ▼
Documentation
```

Tools and techniques may vary depending on the target.

Common areas of investigation include:

### Network Enumeration

* Nmap
* RustScan
* Netcat
* SMB enumeration
* LDAP enumeration
* SNMP enumeration
* DNS enumeration

### Web Enumeration

* Gobuster
* Feroxbuster
* ffuf
* Burp Suite
* Nikto
* Manual application analysis

### Linux Privilege Escalation

* SUID binaries
* Linux capabilities
* Cron jobs
* `sudo`
* Writable files/directories
* PATH manipulation
* Kernel vulnerabilities
* Credential discovery

### Windows Privilege Escalation

* Windows services
* Scheduled tasks
* Token privileges
* Registry enumeration
* Unquoted service paths
* Weak service permissions
* Stored credentials
* PowerShell

### Active Directory

* SMB/LDAP enumeration
* Kerberos
* BloodHound
* Credential attacks
* Password spraying
* Kerberoasting
* AS-REP roasting
* ACL abuse
* Lateral movement

---

## 📝 Report Philosophy

The reports are intended to document **how and why** an attack works.

Where possible, each walkthrough explains:

> **What was discovered → Why it mattered → How it was exploited → What was gained → How the attack could be prevented**

Commands are included alongside explanations rather than simply presenting a list of commands to execute.

---

## ⚠️ Spoilers

**Machine walkthroughs contain complete solutions.**

If you are using these machines for your own practice, consider attempting the machine independently before reading the corresponding report.

A recommended workflow is:

```text
Attempt machine
      ↓
Perform enumeration
      ↓
Develop attack hypotheses
      ↓
Attempt exploitation
      ↓
Document findings
      ↓
Review walkthrough if stuck
      ↓
Reproduce the attack
      ↓
Document lessons learned
```

---

## 🎓 OSCP Preparation

This repository is intended to support preparation for the OSCP by providing additional practice with:

* Enumeration
* Manual exploitation
* Privilege escalation
* Active Directory
* Web application testing
* Shell stabilization
* Password and credential attacks
* Pivoting
* Troubleshooting
* Technical documentation

The material should be considered a **supplement to hands-on lab practice**, not a replacement for official training or labs.

---

## 🛠️ Tools

Tools commonly used throughout the repository include:

| Category             | Tools                                   |
| -------------------- | --------------------------------------- |
| Reconnaissance       | Nmap, RustScan                          |
| Web                  | Burp Suite, Gobuster, Feroxbuster, ffuf |
| Exploitation         | Metasploit, SearchSploit                |
| Windows              | PowerShell, Impacket                    |
| Active Directory     | BloodHound, NetExec, Impacket           |
| Password Attacks     | Hashcat, John the Ripper                |
| Privilege Escalation | LinPEAS, WinPEAS, manual enumeration    |
| Shells               | Netcat, Socat                           |
| Documentation        | Markdown, Obsidian                      |

The specific tools used will depend on the target and engagement.

---

## ⚖️ Legal & Ethical Use

All techniques documented in this repository are intended for **authorized security testing and educational purposes only**.

Only use these techniques against systems that you own or have explicit permission to test.

Do not use the information in this repository to access, compromise, modify, or disrupt systems without authorization.

The author assumes no responsibility for misuse of the information contained within this repository.

---

## 📚 Learning Resources

This repository is intended to complement hands-on security training and intentionally vulnerable environments.

Recommended areas of study include:

* Network penetration testing
* Web application security
* Linux security
* Windows security
* Active Directory
* Privilege escalation
* Exploit development fundamentals
* Security reporting

---

## 🚧 Roadmap

Planned additions include:

* [ ] Additional Linux machines
* [ ] Additional Windows machines
* [ ] Active Directory attack paths
* [ ] Web application assessments
* [ ] Privilege escalation cheat sheets
* [ ] Enumeration cheat sheets
* [ ] PowerShell notes
* [ ] Bash notes
* [ ] Custom enumeration scripts
* [ ] Professional-style penetration testing reports
* [ ] OSCP methodology notes

---

## 👤 About

This repository is maintained as part of my ongoing development in offensive security and penetration testing.

My current focus includes:

* Penetration Testing
* Red Team Operations
* Network Security
* Web Application Security
* Active Directory Security
* Offensive Security Methodology

I currently hold the **eJPT** certification and am working toward the **OSCP**.

---

## ⭐ Disclaimer

**OSCP®** is a registered trademark of Offensive Security Services, LLC.

This repository is an independent project and is not affiliated with or endorsed by Offensive Security.

---

## 📜 License

Unless otherwise specified, the original content in this repository is provided for educational purposes.

Third-party tools, documentation, screenshots, and other materials remain the property of their respective owners and are subject to their respective licenses.
