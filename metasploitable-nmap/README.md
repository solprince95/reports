# 🔍 Vulnerability Scan – Metasploitable 2 using Nmap

## 📘 Overview

This project demonstrates how to perform a *basic vulnerability scan* using nmap against a vulnerable virtual machine: *Metasploitable2*.

It was scanned from *Kali Linux* inside VirtualBox using Host-Only networking to simulate a real attacker/victim setup.

---

## 🧰 Tools Used

- 🐧 Kali Linux (Attacker VM)
- 🧱 Metasploitable 2 (Victim VM)
- 🛰️ Nmap (Network Scanner)
- 📸 Screenshot tool (Kali default)

---

## 🧪 Nmap Scan Command

```bash
nmap -sV -sC -oN metasploitable-scan.txt 192.168.176.4

-sV: Detect service versions

-sC: Run default scripts

-oN: Save output to a file



---

📎 Scan Screenshot



> (Screenshot shows discovered ports and services on Metasploitable2)




---

🔍 Key Findings

Port	Service	Notes

21	vsftpd 2.3.4	Known backdoor vulnerability 🔥
23	Telnet	Insecure, plaintext login
3306	MySQL	May accept default creds
139/445	Samba/SMB	Often misconfigured
8180	Tomcat	Could be brute-forced


🧨 Several services are intentionally vulnerable, designed for ethical hacking practice.


---

🎯 What I Learned

How to identify running services and versions using nmap

How to analyze open ports and their potential risks

The importance of segmentation and patching in real-world systems

How to simulate attacker behavior in a controlled lab



---

📁 Files Included

metasploitable-scan.txt – Full scan result

metasploitable-nmap.png – Screenshot of output

README.md – This writeup/report



---

✅ Created as part of my Cybersecurity Lab Portfolio

Certificate: Google Cybersecurity Professional Certificate
Tools: Kali Linux, Nmap, Metasploitable2
Goal: Build real-world scanning and reporting skills

---
