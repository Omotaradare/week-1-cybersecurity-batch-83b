# 🔐 Cybersecurity Lab Environment Setup

## 📌 Project Overview

This project documents the setup of an isolated cybersecurity laboratory using VirtualBox and Kali Linux.

The purpose of the lab is to create a controlled environment for cybersecurity learning, network reconnaissance, vulnerability assessment and authorized security testing.

---

## 🎯 Objectives

The objectives of this project are:

- Install VirtualBox
- Install Kali Linux
- Configure a private virtual network
- Configure Kali Linux networking
- Verify network connectivity
- Create a clean VM snapshot
- Document the laboratory setup
- Prepare the environment for future cybersecurity projects

---

## 🛡️ Lab Purpose

The laboratory is designed for cybersecurity education and authorized security testing.

The environment can be used for:

- Network reconnaissance
- Port scanning
- Vulnerability assessment
- Packet analysis
- Web security testing
- Security tool experimentation

> ⚠️ This laboratory must only be used against systems that you own or have explicit permission to test.

---

## 🏗️ Lab Architecture

The laboratory consists of:

```text
              INTERNET
                  |
                  |
          ┌───────────────┐
          │   VirtualBox  │
          └───────┬───────┘
                  |
          ┌───────▼───────┐
          │  NAT Network  │
          │  10.0.0.0/24  │
          └───────┬───────┘
                  |
          ┌───────▼───────┐
          │  Kali Linux   │
          │  10.0.0.2     │
          └───────────────┘


---

## 🏗️ Lab configuration 


| Component       | Configuration |
| --------------- | ------------- |
| Host OS         | Windows 11    |
| Hypervisor      | VirtualBox    |
| Security OS     | Kali Linux    |
| Virtual Network | NAT Network   |
| Network         | 10.0.0.0/24   |
| Kali IP         | 10.0.0.2      |
| Gateway         | 10.0.0.1      |
| DNS             | 8.8.8.8       |

---
##🪜 Lab Setup Procedure
Step 1 — Install VirtualBox

VirtualBox was installed as the virtualization platform.

Step 2 — Create the NAT Network

A dedicated NAT Network was created for the cybersecurity laboratory.

Network:

10.0.0.0/24
Step 3 — Install Kali Linux

Kali Linux was installed/imported as a virtual machine.

Step 4 — Configure the Network

The Kali Linux network adapter was connected to the NAT Network.

Step 5 — Configure the IP Address

Example:

IP Address: 10.0.0.2
Subnet Mask: 255.255.255.0
Gateway: 10.0.0.1
DNS: 8.8.8.8
---

##🐞 Problems Encountered
Problem 1 — Network Connectivity

The Kali VM experienced network connectivity issues after configuring the network.

Solution

The network configuration was reviewed and the connection was restarted.

Problem 2 — Virtualization Error

VirtualBox could not start the VM because hardware virtualization was disabled.

Solution

Hardware virtualization was enabled in the computer's BIOS/UEFI settings.
---
##💡 What I Learned

Through this project I learned:

How virtualization works
How to install Kali Linux
How VirtualBox networking works
How NAT Networks work
How to configure IPv4
How to test network connectivity
How to use VM snapshots
How to document cybersecurity projects

##🔐 Security & Ethical Use

This laboratory is intended strictly for educational purposes.

All security testing must be performed only against systems that are owned by me or where I have explicit authorization.

##🛠️ Tools Used
VirtualBox
Kali Linux
Nmap
7-Zip
GitHub
👤 Author

Your Name

Cybersecurity / IT Professional

GitHub: Your GitHub Profile


