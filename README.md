# 🔒 Cyber Security Lab Environment Setup

*Building an isolated virtual lab for penetration testing and ethical hacking practice*



![Skill](https://img.shields.io/badge/Skill-Cybersecurity-red)
![VirtualBox](https://img.shields.io/badge/Ver-VirtualBox%20v7.2-blue)
![Kali](https://img.shields.io/badge/Kali%20Linux-v2026.2-orange)
![Linux](https://img.shields.io/badge/Skill-Linux-red)
![Network](https://img.shields.io/badge/Network-10.0.0.0%2F24-teal)
![PenTest](https://img.shields.io/badge/Penetration-Testing-darkred)
![Virtualization](https://img.shields.io/badge/Skill-Virtualization-red)
![GitHub](https://img.shields.io/badge/GitHub-blue?logo=github)
![NetworkWalks](https://img.shields.io/badge/NetworkWalks-red)
![Ethical](https://img.shields.io/badge/Ethical-Hacking-orange)
![Author](https://img.shields.io/badge/Author-mumbelsec-red)
---

## 📌 Project Overview

This project focuses on setting up a virtual cybersecurity and penetration-testing laboratory using VirtualBox and Kali Linux.
This labs aims to provide a controlled environment where cyber security tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities can be performed safely and repeatedly.
further more, the lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.

## 🎯 Objectives

The main objectives of this project are to:

- Install and configure VirtualBox.
- Install/import Kali Linux as a virtual machine.
- Create a private **NAT Network** for the cybersecurity lab.
- Configure network connectivity for Kali Linux.
- Assign a consistent IP address to the Kali VM.
- Verify network connectivity and DNS resolution.
- Take a clean VM snapshot for recovery.
- Document the complete setup process.
- Prepare the environment for future cybersecurity projects.
  
## 🛡️ Purpose of the Lab

The lab provides an isolated and controlled environment for cybersecurity learning and authorized security testing.

It can be used for the following activities;

- Network reconnaissance
- Port scanning
- Vulnerability assessment
- Packet analysis
- Web security testing
- Exploitation practice
- Security-tool experimentation

> ⚠️ **Important:** This laboratory must only be used for systems that you own or have explicit permission to test. Do not use the lab or its tools to attack unauthorized systems. If caught using on unauthorized networks you will face legal action.

## 🏗️ Lab Architecture

![Lab Architecture](architechture.png)





The lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.

## ⚙️ Lab Configuration

| 🔧 Component | ⚙️ Configuration |
|---|---|
| 🖥️ Host OS | Windows 10 pro |
| 🧠 Host RAM | 4 GB |
| ⚡ Processor | Intel Core i7 |
| 📦 Hypervisor | VirtualBox 7.2.16 |
| 🐉 Security OS | Kali Linux 2026.2 |
| 🧠 Kali RAM | 1.9 GB |
| 🌐 Virtual Network | NAT Network |
| 📡 Network Address | 10.0.0.0/24 |
| ⬆️ Kali IP Address | 10.0.0.2/24 |
| 🖥️ Default Gateway | 10.0.0.1 |
| 🌍 DNS Server | 8.8.8.8 |
| 🧩 Future VM Range | 10.0.0.3–10.0.0.99 |

## 🛠️ Lab Setup Procedure

### Step 1. Install 7-Zip
7-Zip was installed to extract the Kali Linux virtual-machine package, which may be distributed as a `.7z` archive.

**Tool:** 7-Zip was used

### Step 2. Install VirtualBox
Installation of VirtualBox as the hypervisor.

### Step 3. Create the NAT Network
Creation of dedicated NAT Network in VirtualBox.

**Configuration:**
- Network Name: `NatNetwork`
- IPv4 Prefix: `10.0.0.0/24`
- DHCP: Enabled
- IPv6: Disabled
