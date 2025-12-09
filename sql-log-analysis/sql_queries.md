
# SQL Log Analysis – Investigation Queries

This file contains SQL queries used to analyze authentication activity and
identify suspicious login patterns in the system.

---

## 1. After-Hours Failed Login Attempts

```sql
SELECT *
FROM log_in_attempts
WHERE success = FALSE
  AND login_time > '18:00';
```


Identifies failed logins occurring after business hours.

---

## 2. Login Attempts on Specific Incident Dates (May 8–9, 2022)

```sql
SELECT *
FROM log_in_attempts
WHERE login_date = '2022-05-09'
   OR login_date = '2022-05-08';
```

Used to investigate login activity around a specific incident window.

---

## 3. Login Attempts from Outside Mexico

```sql
SELECT *
FROM log_in_attempts
WHERE country NOT LIKE 'MEX%';
```

Flags logins originating from unexpected geographic regions.

---

## 4. Marketing Employees in the East Building

```sql
SELECT *
FROM employees
WHERE department = 'Marketing'
  AND office LIKE 'East%';
```

Retrieves employees in Marketing located in the East building.

---

## 5. Employees in Finance or Sales Departments

```sql
SELECT *
FROM employees
WHERE department = 'Finance'
   OR department = 'Sales';
```

Lists employees belonging to either Finance or Sales.

---

## 6. Employees Not in the IT Department

```sql
SELECT *
FROM employees
WHERE department <> 'Information Technology';
```

