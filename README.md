# 🛡️ Case Study: Vulnerability Assessment of testaspnet.vulnweb.com
**Internship Track:** Cyber Security (CS)  
**Assigned to:** Muhammad Shadab Shaik  
**CIN ID:** FIT/MAR26/CS7147

---

## 📖 The Mission
As part of the **Future Interns** Cyber Security program, I was tasked with performing a professional-grade, read-only security audit of a live web application. The goal was not just to "find bugs," but to act as a security consultant—identifying risks and translating them into clear business language for a client.

### 🛠️ The Toolkit
* **Kali Linux:** My primary operations environment.
* **Nmap:** Used for network-level reconnaissance and service fingerprinting.
* **OWASP ZAP:** Deployed for passive web application vulnerability scanning.
* **Browser DevTools:** Utilized for manual inspection of security headers and session cookies.

---

## 🕵️ Phase 1: Reconnaissance (Network Layer)
My first step was to "knock on the doors" of the server to see what was running. 

> **Finding:** The scan revealed an open **Port 80 (HTTP)** running **Microsoft IIS 8.5** on a Windows environment.
> **Risk:** Running a specific, identifiable version of IIS allows attackers to look up known CVEs (Common Vulnerabilities and Exposures) for that exact software.

---

## 🔍 Phase 2: Web Analysis (Application Layer)
Moving deeper, I utilized **OWASP ZAP** and **Browser DevTools** to analyze the application's behavior without disrupting its services.

* **Passive Scanning:** I monitored the traffic to identify missing security headers (like CSP or HSTS) that protect users from XSS and Clickjacking.
* **Risk Classification:** Every finding was categorized as **Low, Medium, or High** based on its potential impact on business continuity.

---

## 📊 Phase 3: The Deliverable
The technical data was then synthesized into a **Vulnerability Assessment Report** designed for a non-technical stakeholder.

* **Strategic Insights:** Focused on remediation steps rather than just technical flaws.
* **Client Value:** Provided a clear roadmap to harden the web application's security posture.

---

## 📁 Investigation Evidence
* [📄 Full PDF Report](./Report/Vulnerability_Assessment_Report.pdf)
* [📸 Scan Screenshots](./Evidence/)
* [📜 Raw Tool Logs](./Evidence/nmap_output.txt)

---

> **Disclaimer:** This assessment was conducted under a "Read-Only" scope. No intrusive exploitation or unauthorized access was attempted, adhering to the strict ethical guidelines of the Future Interns program.
