# 🔐 Task 4: Setup and Use a Firewall on Windows 11

## 📁 Internship Task – Cybersecurity Basics

This task demonstrates how to use **Windows Defender Firewall** to manage network traffic. The objective is to block a vulnerable port (Telnet) and optionally allow a secure port (SSH), showcasing basic firewall skills and traffic filtering.

---

## 🎯 Objective

- ✅ Understand basic firewall rules
- ✅ Block **Port 23 (Telnet)** – known for being insecure
- ✅ (Optional) Allow **Port 22 (SSH)** – for secure remote access
- ✅ Practice adding, viewing, and removing rules
- ✅ Document and explain firewall behavior

---

## 🛠️ Tools Used

- 🔸 **Windows 11**
- 🔸 **Windows Defender Firewall with Advanced Security**
- 🔸 (Optional) Command Prompt or PowerShell

---

## 📶 Steps Followed

### 1️⃣ Open Windows Firewall
- Press `Windows + R`, type `wf.msc`, press Enter  
  *(or)*  
  Go to: `Start → Windows Defender Firewall with Advanced Security`

### 2️⃣ Block Port 23 (Telnet)
- Navigate to: **Inbound Rules → New Rule**
- Choose **Port**, then **TCP**, and specify **port 23**
- Action: **Block the connection**
- Profile: Domain, Private, Public
- Name the rule: `Block Port 23 (Telnet)`
- ✅ *Screenshot taken*

### 3️⃣ (Optional) Allow Port 22 (SSH)
- Same steps as above, but specify **port 22** and choose **Allow the connection**
- Name it: `Allow Port 22 (SSH)`
- ✅ *Screenshot taken*

### 4️⃣ Remove the Block Rule (Cleanup)
- Find `Block Port 23 (Telnet)` under **Inbound Rules**
- Right-click → Delete
- ✅ *Screenshot taken*

---

## 🔎 Understanding Ports

| Port | Protocol | Status | Reason |
|------|----------|--------|--------|
| 23   | Telnet   | Blocked ❌ | Insecure protocol – sends data in plain text |
| 22   | SSH      | Allowed ✅ | Secure protocol – encrypts data for safe remote login |

---

## 📘 Telnet vs SSH

| Feature          | Telnet                     | SSH                          |
|------------------|----------------------------|-------------------------------|
| Full Form        | Teletype Network           | Secure Shell                  |
| Encryption       | ❌ No                      | ✅ Yes                        |
| Security Level   | 🔓 Insecure                | 🔐 Secure                     |
| Data Sent        | Plain Text                 | Encrypted                     |
| Port             | 23                         | 22                            |
| Use Today        | Obsolete                   | Widely used                   |
| Risk             | High – easy to hack        | Low – secure & reliable       |

---

## 🧠 Key Learnings

- How to configure firewall rules manually using Windows GUI.
- Understanding the difference between insecure and secure protocols.
- Why blocking unused/insecure ports is essential for cybersecurity.
- Hands-on practice in testing, applying, and deleting rules.

---

## 📸 Screenshots

> ✅ Please find screenshots of:
- Created rule to block Port 23
- Allowed rule for Port 22 (optional)
- Deletion of rule (cleanup step)

---

## 🔗 Submission

All task files and screenshots are uploaded to this GitHub repo.  
**Task Submitted at:** [Google Form Link](https://forms.gle/8Gm83s53KbyXs3Ne9)

---

## 📌 Notes

- No third-party tools were used.
- All steps performed using built-in Windows tools.
- No real Telnet/SSH services were needed — the focus is on rule setup.

---

> ✨ *This task strengthened my foundational skills in network security and firewall management.*
