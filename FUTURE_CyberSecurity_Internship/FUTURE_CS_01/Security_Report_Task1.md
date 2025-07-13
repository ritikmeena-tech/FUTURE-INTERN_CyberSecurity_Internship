
# 🛡 Web Application Security Testing Report

**Intern:** Ritik Meena  
**Internship Track:** Cyber Security  
**Task:** Task 1 – Web Application Security Testing  
**Tools Used:** OWASP ZAP, SQLMap, Burp Suite, DVWA  

---

## 🔍 Objective:
Conduct vulnerability assessment on a sample web application (DVWA) to identify common security issues.

---

## 🧪 Vulnerabilities Identified

### 1. SQL Injection (SQLi)
- **Tested URL:** `/vulnerabilities/sqli/`
- **Tool Used:** SQLMap
- **Impact:** Data leakage from backend database
- **Mitigation:** Use prepared statements, parameterized queries.

### 2. Cross-Site Scripting (XSS)
- **Tested URL:** `/vulnerabilities/xss_r/`
- **Tool Used:** OWASP ZAP passive scan
- **Impact:** Script execution in victim browser
- **Mitigation:** Encode output, use CSP headers.

### 3. Weak Authentication
- **Tool Used:** Burp Suite Intruder
- **Impact:** Account compromise through weak credentials
- **Mitigation:** Implement strong password policies and rate-limiting.

---

## 🛡 Mitigation Summary

| Vulnerability | Mitigation |
|---------------|------------|
| SQLi | Use parameterized queries |
| XSS | Encode output, use CSP |
| Auth Flaws | Enforce MFA, rate-limit login |

---

## 📚 Learnings
- Basics of penetration testing workflow
- Practical use of tools like OWASP ZAP and SQLMap
- Understanding web security best practices

---

**Date:12 July 2025  
**Submitted by:** Ritik Meena  
