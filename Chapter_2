# Chapter 2: Information Gathering and Vulnerability Scanning

This chapter covers the methodologies for discovering targets and identifying weaknesses within an environment.

---

## 1. Scanning and Enumeration
The initial phase of identifying the attack surface.

### Scan Targets
*   **Infrastructure**: Network devices, computers, and application services.
*   **Physical & Virtual**: Identifying both physical hardware and virtualized application environments.

### Enumeration
The process of counting and identifying specific instances of target classes, including:
*   **Hosts/Nodes**
*   **Networks and Shares**
*   **Users and Groups**

### Core Toolsets
*   **Nmap**: The industry standard for network discovery and "Scanning Demo".
*   **Packet Investigation**: `nc` (Netcat), `hping` for packet crafting, and **Wireshark/tcpdump** for traffic inspection and sniffing.
*   **Fingerprinting**: Determining OS types, versions, and identifying insecure cryptography.

---

## 2. OSINT (Open-Source Intelligence)
Gathering information from public and semi-public resources to prioritize and prepare for attacks.

*   **Vulnerability Repositories**: 
    *   **NVD/NIST**: Up-to-date vulnerability announcements and databases.
    *   **CVE**: A global list of all common vulnerabilities.
    *   **CWE**: A repository for software weaknesses, providing an alternative perspective to CVE.
*   **Search Engines**: 
    *   **Shodan/Censys**: Identifying Internet-connected devices.
    *   **Wayback Machine**: Accessing historical data via the internet archive.
    *   **Google Dorking**: Using strategic search queries to find exposed sensitive data.
*   **Source Code Repos**: Monitoring Git, SourceForge, and Bitbucket for accidental credential leaks or software flaws.

---

## 3. Vulnerability Analysis and Prioritization
Quantifying risk to determine which issues provide the highest payoff for exploitation.

### Scoring Frameworks
*   **CVSS (Common Vulnerability Scoring System)**: Quantifies severity (0–10) based on factors like attack complexity, required privileges, and impact on Confidentiality, Integrity, and Availability.
*   **EPSS (Exploit Prediction Scoring System)**: A predictive layer (0–1) estimating the probability of a vulnerability being exploited, used alongside CVSS for prioritization.

### High-Value Targets
*   **EOL (End of Life)**: Software no longer receiving security updates, making it a prime target.
*   **Default Configurations**: Systems running with factory settings or weak encryption.
*   **Vulnerable Services**: Outdated, unnecessary, or misconfigured services.

---

## 4. Active Reconnaissance and Detection Avoidance
Probing targets directly while attempting to remain stealthy.

### Defense Detection
*   **WAF Detection**: Using tools like `wafw00f` or the `http-waf-detect` Nmap script.
*   **Load Balancer Detection**: Using the `lbd` command.
*   **Detection Avoidance**: Determining the necessary level of stealth and using Nmap timing options (`-T0` to `-T5`).

### Web & Cloud Recon
*   **Robots.txt**: Checking for hidden directories, admin panels, or staging environments.
*   **Sitemap.xml**: Discovering all URL structures on a site.
*   **Cloud Assets**: Tools like `Cloudbrute` or `OWASP Amass` to find hosted services and their restrictions.

---

## 5. Vulnerability Scanning Types
*   **Credentialed (Authenticated)**: Provides detailed, accurate internal information.
*   **Non-Credentialed (Non-Authenticated)**: Simulates the perspective of an external attacker.
*   **Application Scanning**: 
    *   **Dynamic (DAST)**: Testing while the application is up and running.
    *   **Static (SAST)**: Analyzing artifacts post-execution.
*   **Scan Categories**: Discovery (Ping sweep), Full Scan (Noisy, e.g., `nikto`), Stealth (`-sS`), and Compliance scans.

---

## 6. Analyzing and Leveraging Results
*   **Adjudication**: Filtering out false positives and verifying which vulnerabilities are valid.
*   **Prioritization**: Ranking assets and mapping vulnerabilities to potential exploits using scripts like `vulners` or Metasploit.
*   **Exploit Prep**: 
    *   **Modifying Exploits**: Tweaking code for specific environment success.
    *   **Cross-Compiling**: Compiling exploit code for a different target OS (e.g., using `Mingw-w64`).
    *   **Chaining**: Compromising one system to gain access to another.

---

## 7. Credential Attacks and Automation
*   **Credential Attacks**: 
    *   **THC Hydra**: Fast network logon cracker for brute-forcing.
    *   **Enlightened Attacks**: Using dictionaries or Rainbow Tables (pre-hashed lists) for offline cracking.
*   **Automation Goals**: Achieving repeatability with minimal interaction and handling multi-environment (Cloud, on-prem, third-party) scenarios.