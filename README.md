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
