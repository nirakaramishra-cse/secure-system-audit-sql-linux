# Mini Project Report – SQL & Linux Security Audit

## 1. Introduction

This project demonstrates a basic security audit by combining SQL log analysis
with Linux file-permission hardening. The goal is to identify suspicious login
activity and secure sensitive files by applying least-privilege access controls.

---

## 2. SQL Log Analysis Summary

SQL queries were used to investigate authentication logs and identify:

- Failed login attempts occurring after business hours  
- Login activity on specific incident-related dates (May 8–9, 2022)  
- Logins originating from outside Mexico  
- Employees filtered by department or building for further review  

These queries help detect unusual or unauthorized authentication behavior.

---

## 3. Linux Permissions Audit Summary

A permissions audit was performed in the directory
`/home/researcher2/projects` to identify insecure file and directory settings.

Corrections included:

- Removing unnecessary write permissions  
- Securing the archived file `.project_x.txt`  
- Restricting access to the `drafts` directory  
- Verifying updated permissions using `ls -la`  

These steps ensure only authorized users can access or modify sensitive files.

---

## 4. Conclusion

This mini-project highlights essential cybersecurity skills, including:

- Authentication log investigation using SQL  
- Detecting suspicious login activity  
- Understanding Linux permission models (user/group/other)  
- Applying `chmod` to enforce least-privilege access  
- Documenting findings and remediation steps  


