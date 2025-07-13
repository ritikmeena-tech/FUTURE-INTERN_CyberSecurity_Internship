
# 🛡 Incident Response Report – Task 2

**Intern:** Ritik Meena  
**Internship Track:** Cyber Security  
**Task:** Task 2 – Security Alert Monitoring & Incident Response  
**Tools Used:** ELK Stack, Splunk (Free Trial)  
**Sample Data:** Simulated web and authentication logs  

---

## 🔍 Objective
Monitor and analyze simulated security alerts using SIEM tools to identify, classify, and respond to security incidents.

---

## 🧪 Summary of Alerts

| Time | Alert Type | Description | Severity | Status |
|------|------------|-------------|----------|--------|
| 10:32 AM | Brute-force attempt | Multiple failed logins from single IP | High | Investigated |
| 11:07 AM | SQLi pattern | Suspicious input on login field | Medium | Flagged |
| 11:25 AM | File access | Sensitive file access by unprivileged user | High | Escalated |
| 11:43 AM | XSS payload detected | Reflected XSS in search parameter | Medium | Contained |

---

## 🧠 Incident Classification

1. **Brute-force Login Attack**
   - **Logs:** Repeated failed login attempts (401 status codes)
   - **Remediation:** Implement CAPTCHA, account lockout, IP blocking

2. **SQL Injection Probe**
   - **Logs:** Presence of `' OR '1'='1` and similar patterns
   - **Remediation:** Input validation, prepared statements

3. **Privilege Escalation Attempt**
   - **Logs:** Access to `/etc/passwd` by non-admin user
   - **Remediation:** Enforce least privilege, audit access logs

---

## 🛡 Remediation Summary

| Incident | Mitigation |
|----------|------------|
| Brute-force | CAPTCHA, lockout threshold |
| SQLi | Input sanitization |
| Privilege Abuse | RBAC enforcement |
| XSS | Output encoding, CSP headers |

---

## 📚 Learnings

- Worked with real-world-style log data
- Understood SIEM workflows and alert triage
- Applied incident response lifecycle principles

---

**Date: 12 July 2025  
**Submitted by:** Ritik Meena
