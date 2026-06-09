# ApexPlanet Cyber Security Internship - Task 1

## Kali Linux & Metasploitable2 Lab Setup

### Author

**Vadla Laxmi**

---

## Overview

This project was completed as part of the ApexPlanet Cyber Security Internship.

The objective of this task was to set up a cybersecurity lab environment using VirtualBox, Kali Linux, and Metasploitable2, and perform basic network reconnaissance and service enumeration.

---

## Objectives

* Install Kali Linux in VirtualBox
* Set up Metasploitable2 vulnerable machine
* Configure virtual networking
* Verify network connectivity
* Perform host discovery
* Perform service enumeration
* Explore cybersecurity tools
* Understand penetration testing lab environments

---

## Tools Used

| Tool            | Purpose                              |
| --------------- | ------------------------------------ |
| VirtualBox      | Virtualization Platform              |
| Kali Linux      | Penetration Testing Operating System |
| Metasploitable2 | Vulnerable Target Machine            |
| Nmap            | Network Scanning                     |
| Wireshark       | Packet Analysis                      |
| Burp Suite      | Web Security Testing                 |

---

## Lab Environment

### Virtual Machines

#### Kali Linux

Purpose:

* Attacker Machine
* Security Testing
* Network Reconnaissance

#### Metasploitable2

Purpose:

* Vulnerable Target Machine
* Ethical Hacking Practice Environment

---

## Network Configuration

### Kali Linux

* Adapter 1: NAT
* Adapter 2: Host-Only Adapter

### Metasploitable2

* Adapter 1: NAT
* Adapter 2: Host-Only Adapter

This configuration allows secure communication between Kali Linux and Metasploitable2 inside an isolated virtual network.

---

## IP Address Verification

### Kali Linux

Command:

```bash
ip addr
```

IP Address:

```text
192.168.56.102
```

### Metasploitable2

Command:

```bash
ip addr
```

IP Address:

```text
192.168.56.101
```

---

## Host Discovery

Command Used:

```bash
sudo nmap -sn 192.168.56.0/24
```

Purpose:

* Discover active hosts on the network
* Verify communication between virtual machines

Result:

```text
192.168.56.101
192.168.56.102
```

---

## Service Enumeration

Command Used:

```bash
sudo nmap -sV 192.168.56.101
```

Purpose:

* Identify open ports
* Detect running services
* Determine service versions

---

## Open Ports and Services

| Port | Service    |
| ---- | ---------- |
| 21   | FTP        |
| 22   | SSH        |
| 23   | Telnet     |
| 25   | SMTP       |
| 53   | DNS        |
| 80   | HTTP       |
| 111  | RPC        |
| 139  | NetBIOS    |
| 445  | SMB        |
| 512  | rexec      |
| 513  | rlogin     |
| 514  | rsh        |
| 1099 | Java RMI   |
| 1524 | Bindshell  |
| 2049 | NFS        |
| 2121 | ProFTPD    |
| 3306 | MySQL      |
| 5432 | PostgreSQL |
| 5900 | VNC        |
| 6000 | X11        |
| 6667 | IRC        |

---

## Wireshark

### Purpose

Wireshark is a network protocol analyzer used to:

* Capture network packets
* Monitor traffic
* Analyze communication protocols
* Troubleshoot network issues

### Activity Performed

* Opened Wireshark
* Explored available interfaces
* Learned packet capture workflow

---

## Burp Suite

### Purpose

Burp Suite is a web application security testing tool used for:

* Intercepting HTTP Requests
* Web Vulnerability Assessment
* Security Testing

### Activity Performed

* Launched Burp Suite Community Edition
* Explored Dashboard
* Explored Proxy Features

---

## Screenshots

The **Screenshots** folder contains:

* VirtualBox Setup
* Kali Linux Desktop
* Kali Linux IP Address
* Metasploitable Login
* Metasploitable IP Address
* Nmap Host Discovery
* Nmap Service Enumeration
* Wireshark
* Burp Suite

---

## Learning Outcomes

Through this task, I learned:

* Virtual Machine Setup
* Kali Linux Installation
* Metasploitable2 Deployment
* Virtual Networking
* IP Address Configuration
* Host Discovery Techniques
* Service Enumeration Techniques
* Basic Network Reconnaissance
* Usage of Nmap
* Introduction to Wireshark
* Introduction to Burp Suite

---

## Conclusion

Successfully created a cybersecurity lab environment using Kali Linux and Metasploitable2. Performed host discovery and service enumeration using Nmap and explored industry-standard cybersecurity tools such as Wireshark and Burp Suite.

This task provided practical exposure to network reconnaissance and penetration testing fundamentals.

---

## Repository Structure

```text
ApexPlanet-CyberSecurity-Task1
│
├── README.md
├── Task1_Report.pdf
├── Commands_Used.txt
├── Findings.md
│
└── Screenshots
    ├── 01_VirtualBox_Setup.png
    ├── 02_Kali_Desktop.png
    ├── 03_Kali_IP_Address.png
    ├── 04_Metasploitable_Login.png
    ├── 05_Metasploitable_IP.png
    ├── 06_Nmap_Host_Discovery.png
    ├── 07_Nmap_Service_Scan.png
    ├── 08_Wireshark.png
    └── 09_BurpSuite.png

**ApexPlanet Software Pvt Ltd**
**Cyber Security Internship – Task 1**
