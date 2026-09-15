# 🔐 Cybersecurity Lab Environment Setup

## 📌 Project Overview

This project documents the setup of an isolated cybersecurity laboratory using VirtualBox and Kali Linux.

The purpose of the lab is to create a controlled environment for cybersecurity learning, network reconnaissance, vulnerability assessment, and authorized security testing.

---

## 🎯 Objectives

The objectives of this project are:

* Install VirtualBox
* Install Kali Linux
* Configure a private virtual network
* Configure Kali Linux networking
* Verify network connectivity
* Create a clean VM snapshot
* Document the laboratory setup
* Prepare the environment for future cybersecurity projects

---

## 🛡️ Lab Purpose

The laboratory is designed for cybersecurity education and authorized security testing.

The environment can be used for:

* Network reconnaissance
* Port scanning
* Vulnerability assessment
* Packet analysis
* Web security testing
* Security tool experimentation

> ⚠️ **Important:** This laboratory must only be used against systems that you own or have explicit permission to test.

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
```

---

## ⚙️ Lab Configuration

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

## 🪜 Lab Setup Procedure

### Step 1 — Install VirtualBox

VirtualBox was installed as the virtualization platform for the cybersecurity laboratory.

### Step 2 — Create the NAT Network

A dedicated NAT Network was created for the cybersecurity laboratory.

**Network:**

```text
10.0.0.0/24
```

### Step 3 — Install Kali Linux

Kali Linux was installed/imported as a virtual machine.

### Step 4 — Configure the Network

The Kali Linux network adapter was connected to the VirtualBox NAT Network.

### Step 5 — Configure the IP Address

The Kali Linux network was configured with the following example settings:

```text
IP Address:     10.0.0.2
Subnet Mask:    255.255.255.0
Gateway:        10.0.0.1
DNS:            8.8.8.8
```

### Step 6 — Create a Clean VM Snapshot

A clean VirtualBox snapshot was created after completing the initial laboratory configuration.

**Snapshot name:**

```text
Clean Kali - Network Setup
```

The snapshot provides a recovery point before performing future cybersecurity experiments.

---

## 🔎 Lab Verification

The following commands can be used to verify the laboratory environment.

### Check IP Address

```bash
ip a
```

### Test Gateway Connectivity

```bash
ping 10.0.0.1
```

### Test Internet Connectivity

```bash
ping 8.8.8.8
```

### Test DNS Resolution

```bash
nslookup google.com
```

### Verify Nmap Installation

```bash
nmap --version
```

### Expected Results

| Test       | Command               | Expected Result        |
| ---------- | --------------------- | ---------------------- |
| IP Address | `ip a`                | Kali IP displayed      |
| Gateway    | `ping 10.0.0.1`       | Successful replies     |
| Internet   | `ping 8.8.8.8`        | Successful replies     |
| DNS        | `nslookup google.com` | Domain resolves        |
| Nmap       | `nmap --version`      | Nmap version displayed |

---

## 🐞 Problems Encountered & Solutions

### Problem 1 — Network Connectivity

The Kali VM experienced network connectivity issues after configuring the network.

**Solution:**

The network configuration was reviewed and the network connection was restarted.

---

### Problem 2 — Virtualization Error

VirtualBox could not start the VM because hardware virtualization was disabled.

**Solution:**

Hardware virtualization was enabled through the computer's BIOS/UEFI settings.

The following steps were performed:

1. Restart the computer.
2. Enter the BIOS/UEFI settings.
3. Enable Intel VT-x / hardware virtualization.
4. Save the configuration.
5. Restart the computer.
6. Start the Kali Linux virtual machine.

---

## 💡 What I Learned

Through this project, I learned:

* How virtualization works
* How to install Kali Linux
* How VirtualBox networking works
* How NAT Networks work
* How to configure IPv4 addressing
* How to test network connectivity
* How to use VM snapshots
* How to document cybersecurity projects
* How to use GitHub to document technical projects

---

## 🔐 Security & Ethical Use

This laboratory is intended strictly for educational purposes.

All security testing must be performed only against systems that are owned by me or where I have explicit authorization.

> 🛡️ **Ethical Notice:** Never use cybersecurity tools against systems, networks, websites, or devices without proper authorization.

---

## 🛠️ Tools Used

* VirtualBox
* Kali Linux
* Nmap
* 7-Zip
* GitHub

---

## 👤 Author

**Omotara Oluwadamilare**

IT / Cybersecurity Professional

GitHub: [Omotaradare](https://github.com/Omotaradare)

---

## 📌 Project Information

**Project:** Cybersecurity Lab Environment Setup
**Batch:** Week 1 — Cybersecurity Batch 83B
**Focus:** Virtualization, Networking & Cybersecurity Laboratory Setup

---

### ⭐ Project Status

**Completed — Initial Cybersecurity Lab Setup**
