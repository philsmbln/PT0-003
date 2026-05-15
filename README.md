# PT-003: Penetration Testing Study Notes

A comprehensive collection of notes and methodologies for the PT-003 curriculum, organized by the standard penetration testing lifecycle.

---

## 📑 Table of Contents
1. [Planning and Engagement]
2. [Information Gathering & Vulnerability Scanning]
3. [Network-Based Exploits]
4. [Wireless and RF Attacks]
5. [Web and Database Attacks]

---

## Chapter 1: Planning and Engagement
Focuses on the legal and strategic groundwork for a penetration test.

*   **Legal & Compliance**: Understanding Rules of Engagement (RoE), Regulatory Compliance (PCI-DSS, GDPR), and Impact Constraints.
*   **Standards & Frameworks**: MITRE ATT&CK, NIST SP 800-53, PTES, OSSTMM, and OWASP MASVS.
*   **Threat Modeling**: Utilizing frameworks like STRIDE (Microsoft), DREAD, and OCTAVE.
*   **Scoping**: Defining in-scope assets (IP ranges, Domains, APIs) and "hands-off" environments like Active Directory.

---

## Chapter 2: Information Gathering and Vulnerability Scanning
Methods for reconnaissance and identifying potential entry points.

*   **Passive Recon**: OSINT (Shodan, Censys, Google Dorking), Metadata analysis, and Cloud asset discovery.
*   **Active Recon**: Nmap scanning, WAF/Load Balancer detection, and Banner Grabbing.
*   **Vulnerability Management**: Prioritizing flaws using CVSS (severity) and EPSS (probability) scores.
*   **Scanning Types**: Credentialed vs. Non-credentialed, Discovery scans, and Full scans.

---

## Chapter 3: Network-Based Exploits
Attacks targeting network protocols and identity services.

*   **Name Resolution**: Exploiting LLMNR, NetBIOS (NBT-NS), and DNS/ARP poisoning.
*   **Insecure Protocols**: Exploiting SMB (EternalBlue), SNMPv1, SMTP, and FTP.
*   **Identity Attacks**: Pass-the-Hash, Kerberos ticket forgery, and MFA Fatigue.
*   **MITM (Man-in-the-Middle)**: SSL Stripping, Downgrade attacks, and Replay/Relay attacks.

---

## Chapter 4: Wireless and RF Attacks
Exploiting 802.11 (Wi-Fi) and other radio frequency technologies.

*   **Wi-Fi Exploits**: Evil-Twin/Karma attacks, Deauthentication, and Fragmentation attacks.
*   **Credential Harvesting**: Capturing handshakes and exploiting WPS Pin weaknesses.
*   **Other RF**: Bluetooth (Bluejacking/Bluesnarfing), RFID Cloning, and Jamming.

---

## Chapter 5: Web and Database Attacks
Targeting web applications and data storage.

*   **Injection**: SQLi (extracting/modifying data), HTML, Command, and Code injection.
*   **XSS & CSRF**: Stored/Reflected/DOM-based XSS and Cross-Site Request Forgery.
*   **Misconfigurations**: Directory Traversal, File Inclusion (LFI/RFI), and Insecure Direct Object References (IDOR).
*   **Authentication**: Session Hijacking, Clickjacking, and Cookie Manipulation.

---

## 🛠 Toolset Quick Reference
| Tool | Purpose |
| :--- | :--- |
| **Nmap / hping** | Network Scanning & Packet Crafting |
| **Wireshark / tcpdump** | Traffic Analysis & Sniffing |
| **Metasploit / MSFVenom** | Exploit Development & Payload Generation |
| **Aircrack-ng** | Wireless Security Auditing |
| **Hydra / John the Ripper** | Brute-forcing & Password Cracking |
| **Burp Suite** | Web Application Proxy & Testing |

---
*Notes for PT-003 Exam Preparation*