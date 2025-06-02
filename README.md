# 🛡️ Penetration Testing with Nmap & Metasploit

## 📌 Project Title
**Penetration Testing of Basic Pentesting: 1 Machine using Nmap and Metasploit**

---

## 🎯 Objective

This project aims to simulate a real-world penetration test using open-source tools. The goal is to:

- Discover target machine IP in a local network.
- Scan for open ports and services using **Nmap**.
- Perform enumeration and vulnerability assessment.
- Exploit discovered vulnerabilities using **Metasploit**.
- Gain shell access and extract useful information (flags).
- Document the entire process as a structured penetration test report.

---

## 🧱 Prerequisites

- Basic knowledge of Linux commands.
- **Kali Linux** (bare metal or in VirtualBox).
- Installed tools: `nmap`, `msfconsole`, `netdiscover`, `enum4linux`, `nikto`, `hydra`.
- Oracle VirtualBox.
- VulnHub Machine: [Basic Pentesting: 1](https://www.vulnhub.com/entry/basic-pentesting-1,216/)

---

## 🛠️ Setup Instructions

1. **Download VM** from VulnHub.
2. **Import `.vmdk` into VirtualBox** as a new Ubuntu (64-bit) machine.
3. Set **Network Adapter** to `Host-Only Adapter`.
4. Ensure both Kali and target VM are on the same subnet.
5. Start both machines.

---

## 🔍 Methodology

### 1. Discover Target IP
```bash
netdiscover -r 192.168.56.0/24
# Penetration-Testing-with-Nmap-Metasploit
