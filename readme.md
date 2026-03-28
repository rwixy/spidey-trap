# 🕷️ Spidey CTF Machine ![Type](https://img.shields.io/badge/Type-CTF-blue)

Spidey is a beginner-to-intermediate vulnerable machine designed to simulate a real-world penetration testing scenario. It focuses on web exploitation, credential discovery, and privilege escalation.

---

## 🎯 Difficulty

![Difficulty](https://img.shields.io/badge/Difficulty-Beginner--Intermediate-yellow)

---

## 🧠 Skills Practiced

* Network Enumeration (Nmap)
* Local File Inclusion (LFI)
* Sensitive File Discovery
* SSH Key Exploitation
* Privilege Escalation (Custom Script Abuse)

---

## 🔥 Vulnerabilities Included

* Local File Inclusion (LFI)
* Misconfigured file permissions
* Exposed SSH private key
* Misconfigured sudo privileges

---

## 🗺️ Attack Path Overview

1. Enumerate open ports (22, 80)
2. Discover web application
3. Identify LFI vulnerability
4. Extract username via `/etc/passwd`
5. Retrieve SSH private key
6. Gain access via SSH
7. Exploit misconfigured backup script
8. Achieve root access

---

## 📥 Download

👉 [Download OVA](https://drive.google.com/file/d/1pUkKq9ovCfP7GYE7fMn-_tx8Gv7a9nge/view?usp=sharing)

---

## ⚙️ Setup Instructions

1. Import the OVA into VirtualBox
2. Set network to Host-Only Adapter
3. Start the machine
4. Find IP using `nmap`

---

## ⚠️ Disclaimer

This machine is created for educational purposes only. Do not use it in unauthorized environments.

---

## 👨‍💻 Author

Created by Ihsan
