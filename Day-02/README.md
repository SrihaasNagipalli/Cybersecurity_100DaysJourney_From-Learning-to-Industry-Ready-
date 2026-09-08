# Day 02 —: Cybersecurity Fundamentals

**Date:** 2026-09-08
**Series:** 100 Days of Cybersecurity — From Learning to Industry Ready
**Author:** Srihaas Nagipalli | [@srihaas_winny](https://www.instagram.com/srihaas_winny/)

---

## Q1. Qualities of a Hacker

| # | Quality | Description |
|---|---------|-------------|
| 1 | **Curiosity** | Constantly asks "how does this work?" and explores the unknown |
| 2 | **Problem-Solving** | Approaches complex challenges with creative, lateral thinking |
| 3 | **Technical Depth** | Deep understanding of networks, OS, code, and protocols |
| 4 | **Persistence** | Never gives up; tries different attack vectors |
| 5 | **Continuous Learning** | The threat landscape evolves daily — keeps pace |
| 6 | **Attention to Detail** | Small misconfigurations lead to major vulnerabilities |
| 7 | **Ethical Mindset** | Clear moral compass; respects scope and authorization |
| 8 | **Adaptability** | Pivots approach when initial methods fail |
| 9 | **Analytical Thinking** | Connects disparate data to form a full picture |
| 10 | **Communication** | Translates technical findings for all audiences |
| 11 | **Patience** | Reconnaissance takes hours or days of careful observation |
| 12 | **Creativity** | Finds attack vectors that automated tools miss |

---

## Q2. 10 Categories of Hackers

### 1. White Hat (Ethical Hacker)
- **Authorization:** Fully authorized
- **Intent:** Protect and improve security posture
- **Methods:** Penetration testing, vulnerability assessment, code review
- **Examples:** Security consultants, bug bounty hunters, red teamers
- **Legal status:** Completely legal under written agreement

### 2. Black Hat Hacker
- **Authorization:** Unauthorized
- **Intent:** Personal/financial gain, data theft, disruption
- **Methods:** Ransomware, phishing, zero-days, credential stuffing
- **Legal status:** Criminal in all jurisdictions

### 3. Grey Hat Hacker
- **Authorization:** Usually unauthorized (no malicious intent)
- **Intent:** Discovery; often discloses findings to vendors afterward
- **Legal status:** Legally ambiguous — unauthorized access is still a crime

### 4. Hacktivist
- **Authorization:** Unauthorized
- **Intent:** Ideological, political, or social causes
- **Methods:** DDoS attacks, website defacement, data leaks
- **Examples:** Anonymous, LulzSec

### 5. Nation-State Actor (APT)
- **Authorization:** Government-sanctioned
- **Intent:** Espionage, intelligence gathering, sabotage
- **Methods:** Zero-days, supply chain attacks, long-term persistence
- **Examples:** APT28 (Russia), Lazarus Group (North Korea), APT41 (China)

### 6. Script Kiddie
- **Authorization:** Unauthorized
- **Intent:** Recognition, mischief, opportunism
- **Skill level:** Low — uses pre-built tools without understanding them
- **Methods:** Metasploit scripts, DDoS tools, exploit kits

### 7. Insider Threat
- **Authorization:** Authorized (legitimate access misused)
- **Intent:** Financial gain, revenge, coercion, or accidental
- **Types:** Malicious, negligent, and compromised insiders
- **Methods:** Data exfiltration, sabotage, credential sharing

### 8. Cybercriminal
- **Authorization:** Unauthorized
- **Intent:** Financial gain
- **Methods:** Banking trojans, Business Email Compromise (BEC), card skimming
- **Examples:** Organized crime syndicates, carding forums

### 9. Bug Bounty Hunter
- **Authorization:** Authorized within program scope
- **Intent:** Responsible disclosure and financial reward
- **Platforms:** HackerOne, Bugcrowd, Intigriti
- **Legal status:** Fully legal within disclosed scope

### 10. Red Team Operator
- **Authorization:** Fully authorized under Rules of Engagement (RoE)
- **Intent:** Simulate real-world attacks to test organizational defenses
- **Methods:** Full adversary simulation — network, physical, social engineering
- **Legal status:** Completely legal; governed by formal contracts

---

## Q3. Types of Servers — Advantages, Disadvantages, Limitations & Usage

### 1. Web Server
| Aspect | Detail |
|--------|--------|
| **Examples** | Apache, Nginx, Microsoft IIS |
| **Advantages** | Scalable, widely supported, serves static and dynamic content |
| **Disadvantages** | Prime attack target (XSS, SQLi); resource-intensive at scale |
| **Limitations** | Performance degrades without load balancing |
| **Usage** | Websites, REST APIs, web applications |

### 2. Mail Server
| Aspect | Detail |
|--------|--------|
| **Examples** | Microsoft Exchange, Postfix, Sendmail |
| **Advantages** | Centralized communication management |
| **Disadvantages** | Target for phishing, spam, credential attacks |
| **Limitations** | Requires SPF, DKIM, DMARC to prevent spoofing |
| **Usage** | Corporate email, transactional messages |

### 3. Database Server
| Aspect | Detail |
|--------|--------|
| **Examples** | MySQL, PostgreSQL, MongoDB, MSSQL |
| **Advantages** | Centralized data management, concurrent access, query optimization |
| **Disadvantages** | SQL injection risk if not hardened; single point of failure |
| **Limitations** | Performance bottlenecks with unoptimized queries |
| **Usage** | Application backends, data warehouses, analytics |

### 4. File Server
| Aspect | Detail |
|--------|--------|
| **Protocols** | SMB/CIFS (Windows), NFS (Linux), FTP/SFTP |
| **Advantages** | Centralized backups, access control, file versioning |
| **Disadvantages** | SMB vulnerabilities (EternalBlue); ransomware primary target |
| **Limitations** | Network bandwidth constraints on large transfers |
| **Usage** | Corporate file sharing, backup storage |

### 5. DNS Server
| Aspect | Detail |
|--------|--------|
| **Examples** | BIND, Microsoft DNS, Cloudflare 1.1.1.1 |
| **Advantages** | Enables human-readable addressing; caching speeds resolution |
| **Disadvantages** | DNS poisoning, DNS amplification DDoS attacks |
| **Limitations** | Cache poisoning if DNSSEC not configured |
| **Usage** | Name resolution for every internet connection |

### 6. Proxy Server
| Aspect | Detail |
|--------|--------|
| **Types** | Forward proxy, Reverse proxy, Transparent proxy |
| **Advantages** | Caching, anonymity, content filtering, load balancing |
| **Disadvantages** | Single point of failure; misconfig can expose internal network |
| **Limitations** | HTTPS traffic limits deep inspection without SSL interception |
| **Usage** | Corporate web filtering, CDN, anonymization |

### 7. Application Server
| Aspect | Detail |
|--------|--------|
| **Examples** | Apache Tomcat, JBoss, WebSphere, Node.js |
| **Advantages** | Separates business logic from data layer; supports microservices |
| **Disadvantages** | Deserialization vulnerabilities; complex attack surface |
| **Limitations** | High resource consumption; complex deployment |
| **Usage** | Enterprise apps, e-commerce, ERP systems |

### 8. Authentication Server
| Aspect | Detail |
|--------|--------|
| **Protocols** | LDAP, RADIUS, Kerberos, SAML, OAuth 2.0 |
| **Examples** | Microsoft Active Directory, FreeIPA, Okta |
| **Advantages** | Centralized identity management, SSO capability |
| **Disadvantages** | Critical target — compromise grants access to everything |
| **Limitations** | Vulnerable to Kerberoasting, Pass-the-Hash on misconfigured setups |
| **Usage** | Enterprise login, VPN access, cloud identity management |

---

## Q4. Types of Penetration Testing & Roles/Responsibilities

### Types of Penetration Testing

| Type | Scope | Common Methods |
|------|-------|---------------|
| **Network Pentesting** | Internal/external network infrastructure | Port scanning, service enumeration, firewall bypass |
| **Web Application Testing** | Web apps and APIs | OWASP Top 10, SQLi, XSS, IDOR, SSRF |
| **Mobile App Testing** | iOS and Android applications | Reverse engineering, traffic interception |
| **Social Engineering** | The human layer | Phishing, vishing, pretexting, USB drops |
| **Physical Pentesting** | Physical access controls | Tailgating, lock picking, badge cloning |
| **Wireless Testing** | WiFi, Bluetooth, RFID | WPA2 cracking, evil twin AP |
| **Cloud Pentesting** | AWS, Azure, GCP environments | IAM misconfig, S3 bucket enumeration |
| **API Security Testing** | REST, GraphQL, SOAP endpoints | Broken auth, excessive data exposure, injection |
| **IoT Testing** | Connected devices | Firmware analysis, default credentials |
| **Red Team Assessment** | Full organization (covert) | Combined network + physical + social engineering |

### Roles and Responsibilities of a Penetration Tester

1. **Scope Definition** — Define engagement targets and Rules of Engagement (RoE)
2. **Reconnaissance** — Passive/active OSINT, DNS enumeration, port scanning
3. **Vulnerability Assessment** — Identify and document vulnerabilities
4. **Exploitation** — Prove impact by successfully exploiting findings
5. **Post-Exploitation** — Privilege escalation, lateral movement, data access
6. **Evidence Collection** — Screenshots, logs, and proof-of-concept documentation
7. **Report Writing** — Executive summary + detailed technical report with CVSS scores
8. **Remediation Guidance** — Recommend specific fixes and security controls
9. **Re-testing** — Verify reported vulnerabilities have been remediated

---

## Resources
- [OWASP Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [PTES — Penetration Testing Execution Standard](http://www.pentest-standard.org)
- [TryHackMe — Beginner Path](https://tryhackme.com/path/outline/beginner)
- [HackTheBox](https://hackthebox.com) | [CISA Resources](https://www.cisa.gov)
