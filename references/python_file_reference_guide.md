✅ CyberWolf_001 Python Reference Guide

# Python Reference Guide – File Operations & Parsing  
**CyberWolf_001 Lab Notes – Module 4**

---

## 🐺 File Operations

| Concept       | Syntax                                               | Description                                                                 |
|---------------|------------------------------------------------------|-----------------------------------------------------------------------------|
| `with`        | `with open("wolf_logs.txt", "r") as wolf_file:`      | Safely opens a file and auto-closes after the block                         |
| `open()`      | `open("wolfpack_report.txt", "r")`                   | Opens a file for reading, writing, or appending                             |
| `as`          | `as wolf_file:`                                      | Assigns a variable to the opened file object                                |
| `.read()`     | `wolf_data = wolf_file.read()`                       | Reads the entire file into a string                                         |
| `.write()`    | `wolf_file.write("Howl Detected @ Port 443\n")`      | Writes a string to the file (append or overwrite depending on mode)         |

### 🔄 File Modes:
- `"r"` – Read only  
- `"w"` – Write (overwrite)  
- `"a"` – Append (add to end)

---

### 🧪 File Examples:
```python
with open("wolf_login_log.txt", "r") as log:
    data = log.read()

with open("patched_dens.txt", "w") as patch_log:
    patch_log.write("den-01 secured on 2025-05-18\n")

with open("unauthorized_wolfpack.txt", "a") as alert:
    alert.write("ALERT: Lone wolf from 192.168.9.9\n")

🧠 Parsing Methods
| Method     | Syntax                                 | Description                                            |
| ---------- | -------------------------------------- | ------------------------------------------------------ |
| `.split()` | `"alpha,beta,gamma".split(",")`        | Turns a string into a list by splitting on a delimiter |
| `.join()`  | `"-".join(["alpha", "beta", "gamma"])` | Joins a list into a string with a custom separator     |

.join() – From list to string:
pack = ["luna", "ghost", "shadow"]
joined = "-".join(pack)
# ➜ "luna-ghost-shadow"

🛡️ CyberWolf Analyst Tips
Always use with open() to safely manage files and avoid lock issues.

.split() is useful when working with logs or CSV data.

.join() helps reformat lists for logging, output, or SIEM integration.

Double-check paths and modes ("r", "w", "a") based on use case.

Prepared By:
BOBBY [Abbiu] FⱯLERO
Cybersecurity Analyst | FALE Network Solutions
Project Codename: CyberWolf_001
GitHub: CyberSecFale


---

Let me know if you'd also like:
- 🔽 A downloadable ZIP with `.md` and `.pdf` versions  
- 🖨 A printable dark-mode styled CyberWolf PDF  
- ✅ A matching lab logging template to go with this reference guide


