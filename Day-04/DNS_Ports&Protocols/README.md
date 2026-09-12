# 🔐 Day 04 — DNS, Ports & Protocols

Part of my **100 Days of Cybersecurity** learning journey.

## 📚 Topics Covered

- DNS Fundamentals
- How DNS Resolution Works
- DNS Hierarchy
- DNS Records
- Network Ports
- Well-Known Ports
- Network Protocols
- TCP vs UDP
- Common Application Protocols
- DNS & Network Troubleshooting Commands

---

# 🌐 1. What is DNS?

DNS stands for **Domain Name System**.

It translates human-readable domain names into IP addresses.

Example:

google.com
↓
DNS Resolution
↓
IP Address
↓
Google Server

Without DNS, users would need to remember IP addresses instead of domain names.

---

# 🔄 2. Basic DNS Resolution

A simplified DNS lookup can be represented as:

Client
↓
DNS Resolver
↓
Root DNS Server
↓
TLD DNS Server
↓
Authoritative DNS Server
↓
IP Address
↓
Client

The client can then use that IP address to communicate with the destination server.

---

# 📋 3. Common DNS Records

| Record | Purpose |
|---|---|
| A | Maps a domain to an IPv4 address |
| AAAA | Maps a domain to an IPv6 address |
| CNAME | Creates an alias for another domain |
| MX | Specifies mail servers |
| NS | Specifies authoritative name servers |
| TXT | Stores text information used for various purposes |

---

# 🔢 4. What is a Port?

A port is a logical endpoint used by network services.

An IP address identifies the host/interface,
while the port helps identify the service endpoint.

Example:

192.168.1.10:443

IP Address:
192.168.1.10

Port:
443

Protocol:
HTTPS

---

# 🔐 5. Common Ports

| Port | Service | Purpose |
|---:|---|---|
| 20/21 | FTP | File Transfer |
| 22 | SSH | Secure Remote Access |
| 23 | Telnet | Remote Access |
| 25 | SMTP | Email Transfer |
| 53 | DNS | Domain Resolution |
| 80 | HTTP | Web Traffic |
| 110 | POP3 | Email Retrieval |
| 143 | IMAP | Email Access |
| 443 | HTTPS | Secure Web Traffic |
| 3389 | RDP | Remote Desktop |

---

# 🔗 6. What is a Network Protocol?

A protocol is a set of rules that defines how systems communicate.

Examples:

- HTTP
- HTTPS
- DNS
- SSH
- FTP
- SFTP
- SMTP
- IMAP
- TCP
- UDP
- DHCP
- ARP

---

# ⚡ 7. TCP vs UDP

## TCP

Transmission Control Protocol.

Characteristics:

- Connection-oriented
- Reliable delivery
- Ordered communication
- Error checking and retransmission

Examples:
- HTTPS
- SSH
- FTP

## UDP

User Datagram Protocol.

Characteristics:

- Connectionless
- Lower overhead
- No guarantee of delivery
- Useful when speed is important

Examples:
- DNS queries
- Streaming
- Online gaming
- Voice/video applications

---

# 🧪 8. Hands-on Practice

## DNS Lookup

Windows/Linux/macOS:

```bash
nslookup google.com
