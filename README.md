# Nmap Enumeration Project

This project demonstrates a complete Nmap scanning workflow performed as part of my cybersecurity learning on TryHackMe.

## 📌 Project Description

The goal of this project was to learn and practice network reconnaissance using Nmap. The scans were executed on a controlled lab environment (TryHackMe AttackBox and target machine). Each step focused on a specific enumeration objective.

## 🛠️ Tools Used
- Nmap
- TryHackMe AttackBox (Kali Linux)

## 🧭 Steps Performed

### 1️⃣ Host Discovery
**Command:**
```
nmap -sn <target-ip>
```
**Purpose:**
Identify whether the host is online and reachable.

---

### 2️⃣ Full TCP SYN Port Scan
**Command:**
```
nmap -sS -p- <target-ip>
```
**Purpose:**
Scan all 65,535 TCP ports to find open ports.

---

### 3️⃣ Service Version Detection
**Command:**
```
nmap -sV -p <ports> <target-ip>
```
**Purpose:**
Determine what services are running on the open ports and their versions.

---

### 4️⃣ Script Scan
**Command:**
```
nmap -sC -sV -p <ports> <target-ip>
```
**Purpose:**
Run Nmap default scripts to collect additional information and check for common misconfigurations.

---

### 5️⃣ OS Detection
**Command:**
```
nmap -O -p <ports> <target-ip>
```
**Purpose:**
Attempt to identify the target operating system.

---

## 🖼️ Screenshots

Screenshots of each scan result are included in this repository for reference and documentation.

---

## 📄 Learning Outcomes

- Gained hands-on experience performing network enumeration with Nmap.
- Learned how to interpret scan results, including:
  - Open ports and services
  - Service versions
  - OS fingerprinting
  - Basic script output

---

## 🔗 Author

Hanan Fathima K

---

*This project was conducted in a safe lab environment and did not target any unauthorized systems.*
