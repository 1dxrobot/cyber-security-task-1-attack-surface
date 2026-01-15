<h5>Cyber-security-task-1-attack-surface</h5>
<h4>1.Research cyber security fundamentals, emphasizing the CIA triad (confidentiality, integrity, availability) with examples from banking and social media. </h4> 
1.1 Introduction to the CIA Triad
The CIA triad—Confidentiality, Integrity, and Availability—is a foundational model in cybersecurity used to guide policies and strategies for protecting information. Despite its name, it has no connection to the Central Intelligence Agency; instead, it represents three core principles that ensure data remains secure, accurate, and accessible.
<h4> 1.2 Confidentiality in Cybersecurity </h4>
<li>Encryption</li> <li> Access Control </li>   <li>Multi Factor Authentication (MFA) </li>
<h4> 1.3 Integrity in Cybersecurity </h4>
<li>Hashing</li> <li>Digital signatures</li>
<li>Version control systems</li>
<h4> 1.4 Availability in Cybersecurity</h4>
<li>Redundant systems </li>
<li>Disaster recovery plans </li>
<li>DDoS protection </li>
<br>
<h3> 1.5 CIA Triad in Social Media </h3>
Confidentiality:<li>User passwords and private messages are encrypted. Platforms use OAuth and MFA to prevent account takeovers. </li> 
Integrity: <li>Measures like content hashing and audit logs help detect fake accounts or manipulated posts. However, misinformation remains a challenge.</li> 
Availability:<li>Platforms must remain online despite massive traffic. Content delivery networks (CDNs) and auto-scaling cloud infrastructure ensure continuous access.</li>
<br>
<h4> 2.Identify attacker types like script kiddies, insiders, hacktivists, and nation-state actors using credible security blogs.</h4> 
<h4> 2.1 Script Kiddies</h4>
<li>Attacker Who Use pre written Tools Or Script developed By Others without Understanding an Underlying the mechanism. </li>
<br>
<h4>2.2 Insiders</h4>
<li>Insider threats come from individuals within an organization—employees, contractors, or partners—who misuse their authorized access to compromise data or systems. </li>
<br> 
<h4> 2.3 Hacktivists</h4>
<li> Hacktivists use cyber attacks to promote political, social, or ideological causes. They often target organizations they perceive as unethical.</li> 
<br> 
<h4>2.4 Nation-State Actors</h4>
<li> Nation-state actors are highly skilled, well-funded groups backed by governments to conduct cyber espionage, sabotage critical infrastructure, or steal intellectual property.</li>
<br>
<h4> 3.Explore attack surfaces such as web apps, mobile apps, APIs, networks, and cloud infrastructure</h4>
<h3>3.1 Web Applications</h3>
<li> Web applications are a major component of the digital attack surface, exposed to threats like SQL injection, cross-site scripting (XSS), and insecure authentication.
  
<b> Example:</b> The 2023 MOVEit breach exploited a vulnerability in a web-based file transfer tool, compromising thousands of organizations.

<b> Mitigation:</b> Regular patching, input validation, and web application firewalls (WAFs).</li>
<br>
<h3>3.2 Mobile Apps</h3>
<li>Mobile apps expand the attack surface through insecure data storage, weak encryption, and third-party SDKs. Lost or stolen devices also pose physical risks.

<b>Risk:</b> Apps may leak sensitive data via insecure APIs or local storage.

<b>Protection:</b> Code obfuscation, runtime application self-protection (RASP), and secure API communication.</li>
<br>
<h3> 3.3 APIs</h3>
<li> APIs act as connective tissue between services but are frequently exposed, poorly authenticated, or lack rate limiting.

Threat: In 2023, Honda suffered a data breach due to an API vulnerability in its e-commerce platform.

Best Practices: Enforce authentication (OAuth), input validation, logging, and API gateways.</li>
<br>
<h3> 3.4 Networks</h3>
The network attack surface includes routers, switches, firewalls, and open ports that can be exploited for lateral movement.

Vulnerabilities: Unsecured protocols, outdated firmware, or misconfigured access controls.

Defense: Network segmentation, intrusion detection systems (IDS), and zero-trust architecture.
<br>
<h4>4. Top 10 OWASP </h4> Research on 2025
<li> 4.1 A01: Broken Access Control – Unauthorized access due to improper permissions (e.g., accessing another user’s account).</li>
<li>4.2 A02: Cryptographic Failures – Weak or missing encryption exposing sensitive data (e.g., plaintext passwords). </li> 
<li>4.3 A03: Injection – Malicious input (e.g., SQL, NoSQL) executed as commands.</li> 
<li>4.4 A04: Insecure Design – Flaws in application logic or architecture.</li> 
<li>4.5 A05: Security Misconfiguration – Improperly configured systems (e.g., open cloud storage).</li> 
<li>4.6 A06: Vulnerable and Outdated Components – Use of unpatched libraries or frameworks.</li> 
<li>4.7 A07: Identification and Authentication Failures – Weak login mechanisms (e.g., no MFA). </li> 
<li>4.8 A08: Software and Data Integrity Failures – Unverified code updates or deserialization flaws.</li> 
<li>4.9 A09: Security Logging and Monitoring Failures – Lack of detection for breaches.</li> 
<li>4.10 A10: Server-Side Request Forgery (SSRF) – Forcing a server to access internal resources.</li> 
<br>
<h4> 5.Map attack surfaces in everyday apps like email, WhatsApp, and banking. </h4> 
<h4> 5.1 Email </h4>
<li> Email is a primary attack surface due to its widespread use in personal and professional communication. Common threats include:<ol> Phishing & BEC </ol> <ol> Malware Delivery </ol> <ol> Spoofing </ol></li>
<h4> 5.2 WhatsApp </h4>
<li>WhatsApp’s popularity makes it a prime target, especially in regions like Brazil where it's used for business and banking:   <ol> Malware Propagation </ol> <ol> Auto-Messaging Worms </ol><ol> Social Engineering </ol></li>
<h4> 5.3 Banking Apps </h4>
<li> Banking applications face multi-layered threats across mobile and web platforms:    <ol> Overlay Attacks </ol> <ol> Man-in-the-Disk </ol> <ol> Device Tampering </ol></li> 
<h4> 6.Document data flow: user → application → server → database. </h4> 
<li> 6.1 User: Initiates a request through a web or mobile interface.
  
6.2 Application (Frontend): Captures user input and sends it via HTTP(S) to the backend server, often in JSON or form-data format.

6.3 Server (Backend): Receives the request, processes it and queries the database as needed using APIs or ORM tools.

6.4 Database: Stores, retrieves, or updates data in response to server queries. Results are sent back through the same chain to the user.</li>

<h4> 7.Pinpoint attack points along that data flow.</h4>

<li>7.1 User → Application (Frontend)
Attack Points: Phishing, keyloggers, malicious browser extensions
  
Threats: Credentials stolen before input; fake login overlays (e.g., in banking apps)</li>
<br> 
<li>7.2 Application (Client-Side) → Server
Attack Points: HTTP requests, APIs, forms

Threats: Injection attacks (e.g., SQLi via login fields)

Cross-Site Scripting (XSS): Malicious scripts injected into input fields

CSRF: Unauthorized actions triggered via authenticated sessions
Insecure data transmission if TLS is missing or weak</li> 
<br>
<li> 7.3 Server (Backend)
Attack Points: Authentication logic, session management, API endpoints

Threats:
Broken access control: Unauthorized access to resources

Server-Side Request Forgery (SSRF): Forcing server to access internal systems

Insecure deserialization: Remote code execution via manipulated data </li>
<br>
<li>7.4 Server → Database
Attack Points: Database queries, connection strings, stored procedures

Threats:
SQL Injection: Direct manipulation of queries to extract or alter data

Excessive database privileges: Compromised server gains full DB access

Unencrypted data at rest: Data exposure if storage is breached</li>
