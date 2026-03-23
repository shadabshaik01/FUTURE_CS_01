# 🛡️ Case Study: Vulnerability Assessment of testaspnet.vulnweb.com
[cite_start]**Internship Track:** Cyber Security (CS) [cite: 26]
**Assigned to:** Muhammad Shadab Shaik
[cite_start]**CIN ID:** FIT/MAR26/CS7147 [cite: 35]

---

## 📖 The Mission
As part of the **Future Interns** Cyber Security program, I was tasked with performing a professional-grade, read-only security audit of a live web application. [cite_start]The goal was not just to "find bugs," but to act as a security consultant—identifying risks and translating them into clear business language for a client[cite: 108, 115].

### 🛠️ The Toolkit
* [cite_start]**Kali Linux:** My primary operations environment[cite: 39].
* [cite_start]**Nmap:** Used for network-level reconnaissance and service fingerprinting[cite: 41].
* [cite_start]**OWASP ZAP:** Deployed for passive web application vulnerability scanning[cite: 69].
* [cite_start]**Browser DevTools:** Utilized for manual inspection of security headers and session cookies[cite: 69].

---

## 🕵️ Phase 1: Reconnaissance (Network Layer)
My first step was to "knock on the doors" of the server to see what was running. 

> **Finding:** The scan revealed an open **Port 80 (HTTP)** running **Microsoft IIS 8.5** on a Windows environment.
> **Risk:** Running a specific, identifiable version of IIS allows attackers to look up known CVEs (Common Vulnerabilities and Exposures) for that exact software.

---

## 🔍 Phase 2: Web Analysis (Application Layer)
[cite_start]Moving deeper, I utilized **OWASP ZAP** and **Browser DevTools** to analyze the application's behavior without disrupting its services[cite: 69].

* **Passive Scanning:** I monitored the traffic to identify missing security headers (like CSP or HSTS) that protect users from XSS and Clickjacking.
* **Risk Classification:** Every finding was categorized as **Low, Medium, or High** based on its potential impact on business continuity.

---

## 📊 Phase 3: The Deliverable
[cite_start]The technical data was then synthesized into a **Vulnerability Assessment Report** designed for a non-technical stakeholder[cite: 70, 77].

* [cite_start]**Strategic Insights:** Focused on remediation steps rather than just technical flaws[cite: 75, 116].
* **Client Value:** Provided a clear roadmap to harden the web application's security posture.

---

## 📁 Investigation Evidence
* [cite_start][📄 Full PDF Report](./Report/Vulnerability_Assessment_Report.pdf) [cite: 77]
* [📸 Scan Screenshots](./Evidence/)
* [📜 Raw Tool Logs](./Evidence/nmap_output.txt)

---

> **Disclaimer:** This assessment was conducted under a "Read-Only" scope. No intrusive exploitation or unauthorized access was attempted, adhering to the strict ethical guidelines of the Future Interns program.
