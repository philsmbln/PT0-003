# Web and Database Attacks

## Injection Attacks
*Inserting additional data beyond what the app is expecting.*

### Types
* **SQL Injection:** Adding crafted SQL input to extract/modify data or execute commands.
* **HTML Injection:** Submitting data to change how a page works or how data is handled within the HTML interpreted environment.
* **Command Injection:** Adding command-line options that change the way commands operate.
* **Code Injection:** Adding code of any language to change a program's behavior.

---

## Application Exploits
* **Credential Brute-Forcing:** Systematic attempts to guess passwords (e.g., using tools like **Hydra**).
* **Session Hijacking:** Intercepting and using a session token to take over a valid user session.
* **Redirect:** Sending the user to a different site from what they expected (commonly used in phishing).
* **Default Credentials:** Exploiting "out of the box" settings/passwords left unchanged.
* **Weak Credentials:** Exploiting easily guessable or common passwords.
* **Kerberos Exploits:** Forging tickets to allow unauthorized access to network resources.

---

## Authorization Exploits
* **Parameter Exploits:** Providing custom input parameters to a service or API operation to manipulate logic.
* **Invocation Intercept:** Similar to an injection attack but targeted toward distributed systems.
* **Insecure Direct Object Reference (IDOR):** A programming mistake that allows an attacker to bypass access controls and access resources or data by manipulating identifiers.

---

## Cross-Site Scripting (XSS)
*Forcing a client to run malicious code when sent to them.*

* **Stored/Persistent:** Attack data (script) is stored permanently on the target server (e.g., in a database or comment section).
* **Reflected:** A non-persistent attack where the malicious script is "reflected" off a web application to the victim's browser (usually via a link).
* **Document Object Model (DOM):** An XSS attack that uses XML/client-side scripts, rather than HTML, to transport and execute attack code.

---

## CSRF/XSRF & UI Redressing
* **CSRF/XSRF (Cross-Site Request Forgery):** Occurs within an authenticated session. The attacker causes an authorized user to take an unwanted action by clicking a link.
* **Clickjacking:** Tricking a user into clicking a different link than they intended. 
    * Uses transparent or opaque layers (overlaying).

---

## Security Misconfiguration
* **Directory Traversal:** Allows users to navigate outside a web server's root directory to access restricted files.
* **Cookie Manipulation:** Gaining access to cookies to change how a web application operates for a specific user or session.
* **File Inclusion:** Related to directory traversal; allowing an attacker to build a path to an executable or sensitive file.
    * **Local File Inclusion (LFI)**
    * **Remote File Inclusion (RFI)**