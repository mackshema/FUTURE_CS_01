#  Vulnerability Assessment Report — cyberbase-nine.vercel.app
### Future Interns Cybersecurity Task 1 (2026)

![Assessment Type](https://img.shields.io/badge/Assessment-Passive%20Read--Only-blue)
![Tools](https://img.shields.io/badge/Tools-Nmap%20%7C%20ZAP%20%7C%20SecurityHeaders-navy)
![Status](https://img.shields.io/badge/Status-Completed-green)
![Risk Level](https://img.shields.io/badge/Overall%20Risk-Medium-orange)

---

##  About This Report

This repository contains the full Vulnerability Assessment Report produced  
as part of **Future Interns Cybersecurity Task 1 (2026)**.

The assessment was conducted against a **live web application** using  
**passive, read-only techniques only** — no exploitation, no brute force,  
no denial-of-service was performed at any point.

---

##  Target

| Field | Detail |
|-------|--------|
| **URL** | https://cyberbase-nine.vercel.app/ |
| **IP Addresses** | 216.198.79.67 / 64.29.17.131 |
| **Hosting** | Vercel (CDN + Edge) |
| **Tech Stack** | React, React Router 7.13.1, Tailwind CSS, GSAP, Vercel |
| **Assessment Date** | 26 April – 1 May 2026 |
| **Scope** | Public-facing pages only — passive scan |

---

##  Tools Used

| Tool | Version | Purpose |
|------|---------|---------|
| SecurityHeaders.com | Web Tool | HTTP security header audit |
| OWASP ZAP | 2.17.0 | Automated passive scanning |
| Nmap | 7.99 | Port & service enumeration |
| Qualys SSL Labs | v2.4.1 | TLS/SSL certificate analysis |
| Wappalyzer | Chrome Extension | Technology stack fingerprinting |
| Browser DevTools | Chrome 124 | Manual header & cookie inspection |

---

##  Findings Summary

| ID | Finding | Severity | Status |
|----|---------|----------|--------|
| VUL-01 | Missing Content-Security-Policy | Medium | Open |
| VUL-02 | Cross-Domain Misconfiguration (CORS) | Medium | Open |
| VUL-03 | Missing X-Frame-Options (Clickjacking) | Low | Open |
| VUL-04 | Server Information Disclosure | Low | Open |
| VUL-05 | Session ID in URL Rewrite | Low | Open |
| VUL-06 | Missing X-Content-Type-Options | Low | Open |
| VUL-07 | Missing Referrer-Policy | Low | Open |
| VUL-08 | Missing Permissions-Policy | Low | Open |
| VUL-09 | HSTS Not Set (22 instances) | Info | Partial |
| VUL-10 | Timestamp Disclosure — Unix | Info | Open |
| VUL-11 | Modern Web Application Detected | Info | Informational |
| VUL-12 | Cache-Control Directives | Info | Open |
| VUL-13 | SSL Scan Limitation (CDN Edge) | Info | Accepted |

**Overall Grade:** SecurityHeaders.com → **D**  
**Overall Risk Level:** **Medium**

---

##  Ethical Disclaimer

> This assessment was performed on an application owned by the auditor.  
> All testing was **passive and read-only**.  
> No exploitation, login bypass, brute force, or DoS was performed.  
> This report is produced for **educational purposes** as part of Future Interns Task 1.

---

##  Auditor

**Mack (Siva Sanjay Muthu T)**  
Future Interns — Cybersecurity Intern (2026)  
 [LinkedIn](https://linkedin.com/in/siva-sanjay-muthu-t-823318304)  
 [GitHub](https://github.com/mackshema)

---

*Future Interns · Cybersecurity Task 1 · 2026*
