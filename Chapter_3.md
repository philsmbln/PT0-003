# Chapter 3: Network-Based Exploits

## Name Resolution Exploits
* **NETBIOS Name Service**
    * Part of NetBIOS-over-TCP.
    * Similar functionality to DNS but for local networks.
* **LLMNR (Link-Local Multicast Name Resolution)**
    * Protocol based on DNS packet format.
    * Allows IPv4 and IPv6 name resolution on the same local link.
* **DNS and ARP Poisoning**
    * Used to modify tables that control local connectivity on a network, redirecting traffic to malicious nodes.

## SMB Exploits (Windows Based)
* **Purpose:** SMB (Server Message Block) provides file and printer access, and remote service access.
* **Ports:** TCP ports 139 and 445.
* **History:** Some high-profile ransomware (e.g., **EternalBlue**, **WannaCry**) use SMB vulnerabilities to propagate through networks.

## SNMP Exploits
* **Purpose:** Query and manage IP devices.
* **Vulnerability:** Multiple versions exist; **SNMPv1** is considered highly insecure as it lacks robust authentication.

## SMTP Exploits
* **Purpose:** Standard protocol for email.
* **Attack Vectors:** Open relay, local relay, phishing, and spam.

## FTP Exploits
* **Vulnerability:** Overall insecure protocol for transferring files.
* **Lack of Encryption:** Does not encrypt data transfers or credentials.
* **Data Exfiltration:** Easily leveraged by attackers for data exfiltration if the service is available.

---

## Authentication Attacks
### MFA Fatigue Attack
* **Mechanism:** Push-based systems wait until a human approves the notification.
* **Method:** Repeated login attempts to flood the user's device.
* **Human Factor:** Exploits the human side of security (users becoming annoyed or confused and eventually clicking "Approve").
* **Prevention:** Requires user training and rate-limiting.

### Mask Attacks
* **Definition:** Optimized brute force attacks.
* **Method:** Uses defined patterns rather than random characters.
* **Efficiency:** Best used against systems with easily guessable password policies.
* **Tools:** Hashcat, John the Ripper.

### OIDC (OpenID Connect)
* **Definition:** A federated identity protocol.
* **Vulnerabilities:**
    * Token substitution/Replay attacks.
    * Open redirect vulnerabilities.
* **Testing:** OIDC flows must be rigorously tested for validation logic.

### SAML Attacks
* **Definition:** XML-based protocol for authentication and authorization.
* **Vulnerabilities:**
    * Signature wrapping.
    * Assertion spoofing.
* **Impact:** High-impact target during authentication-focused security assessments.

---

## Man-in-the-Middle (MitM) Exploits
* **Definition:** The attacker intercepts communication between a sender and a receiver.
* **Actions:** May modify, regenerate, or forward traffic.

### Common MitM Techniques
* **DNS Cache Poisoning:** Modifying a DNS server's records to redirect users.
* **ARP Spoofing:** Spoofing local MAC addresses to intercept LAN traffic.
* **Pass the Hash:** Grabbing NTLM user credentials (the hash) and reusing them in Windows environments.
* **Replay Attacks:** Grabbing a valid transmission and resending it later.
* **Relay Attacks:** Intercepting a request and sending it to an alternate destination.
* **SSL Stripping:** Intercepting HTTPS traffic and "stripping" the encryption to see data in plain text.
* **Downgrade Attack:** Proxying a connection and negotiating a lower encryption standard (or no encryption).
* **DoS and Stress Test:** Flooding resources to disrupt service.
* **NAC Bypass:** Intercepting and using a different control to bypass Network Access Control.
* **VLAN Hopping:** Moving from one VLAN to another to access restricted network segments.