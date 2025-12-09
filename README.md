
# 🔐 Secure System Audit – SQL Log Analysis & Linux Permission Hardening

<p align="center">

  <!-- Project Type -->
  <img src="https://img.shields.io/badge/Project-Security_Audit-2ea44f?style=for-the-badge">

  <!-- SQL Badge -->
  <img src="https://img.shields.io/badge/SQL-Log_Analysis-blue?style=for-the-badge&logo=postgresql&logoColor=white">

  <!-- Linux Badge -->
  <img src="https://img.shields.io/badge/Linux-Permission_Hardening-yellow?style=for-the-badge&logo=linux&logoColor=black">

  <!-- Tools Badge -->
  <img src="https://img.shields.io/badge/Tools-SQL%20%7C%20chmod%20%7C%20ls-lightgrey?style=for-the-badge">

  <!-- Status Badge -->
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge">

</p>

This project simulates a real-world security audit by analyzing authentication
logs using SQL and hardening Linux file permissions to enforce least-privilege
access. It demonstrates fundamental cybersecurity skills required for SOC,
system administration, and security engineering roles.

<p align="center">
  <img src="assets/banner.png" alt="Secure System Audit Banner" width="100%" height="auto">
</p>

---

## 📘 Overview

The project is divided into two main components:

### 1️⃣ SQL Log Analysis
Investigates suspicious login activity using filters such as:
- After-hours access attempts  
- Unusual geographic locations  
- Date-based filtering for incident windows  
- Department-based retrieval for remediation  

### 2️⃣ Linux Permissions Audit
Assesses and corrects file and directory permissions by:
- Reviewing access levels using `ls -la`  
- Securing files with `chmod`  
- Restricting sensitive directories  
- Applying least-privilege principles  

---

## 📁 Project Structure

```
secure-system-audit-sql-linux/
│── README.md
│
├── sql-log-analysis/
│ └── sql_queries.md
│
├── linux-file-permissions/
│ └── commands.md
│
└── report/
└── mini_project_report.md

```

---

## 🧩 Part 1: SQL Log Analysis

The SQL portion focuses on extracting meaningful insights from the
`log_in_attempts` and `employees` tables to identify:
- Failed logins after business hours  
- Activity on specific suspicious dates  
- Login attempts originating outside approved regions  
- Employee lists filtered by building or department  

Full SQL queries are documented in:  
➡️ `sql-log-analysis/sql_queries.md`

---

## 🛡️ Part 2: Linux Permission Hardening

The Linux portion reviews permissions within a project directory and applies
corrective actions:
- Identifying overly permissive files  
- Securing archived files  
- Restricting directory access  
- Verifying updated permissions  

Complete Linux commands are documented in:  
➡️ `linux-file-permissions/commands.md`

---

## 🎯 Skills Demonstrated

- SQL log filtering & investigation  
- Identifying authentication anomalies  
- Linux file system security (rwx model)  
- Access control with `chmod`  
- Documentation & incident analysis  
- Understanding and applying least-privilege  

---

## 🛠️ Technologies Used
- SQL (Filtering & Analysis)
- Linux Shell  
- File Permission Utilities (`ls`, `chmod`)  

---

## 👨‍💻 Author
**Nirakar Mishra**  
Cybersecurity Analyst 

If you find this project useful, please ⭐ star the repository.

#### **Connect with me:**

- 🌐 [Portfolio](https://nirakaramishra-cse.github.io/Portfolio)  


