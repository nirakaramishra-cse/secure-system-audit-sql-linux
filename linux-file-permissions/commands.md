
# Linux File Permission Hardening – Commands & Explanations

This file contains Linux commands used to review and correct file and directory
permissions during the security audit.

---

## 1. View Current Permissions

```bash
ls -la /home/researcher2/projects
````

Displays file types, ownership, and permissions for all items, including hidden files.

---

## 2. Fix Overly Permissive File (project_k.txt)

```bash
chmod o-w project_k.txt
ls -la project_k.txt
```

Removes write permission from “other” users.

---

## 3. Secure Archived Hidden File (.project_x.txt)

```bash
chmod u-w .project_x.txt
chmod g-w .project_x.txt
chmod g+r .project_x.txt
ls -la .project_x.txt
```

Removes modification access and ensures only read access where needed.

---

## 4. Restrict Access to drafts Directory

```bash
chmod g-x drafts
chmod o-rx drafts
ls -la drafts
```

Only the owner can access or enter the directory.

---

## 5. Verify Final Permissions

```bash
ls -la /home/researcher2/projects
```

Confirms all permission corrections have been applied.

