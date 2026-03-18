# Enterprise IT Lab

A hands-on Windows-based enterprise infrastructure lab built using VMware Workstation Pro.

This project simulates a small enterprise environment with centralized identity, domain-joined systems, and internal networking. Each lab focuses on deploying, validating, and troubleshooting core infrastructure components.

---

## Key Skills Demonstrated

- Active Directory domain deployment and management  
- Domain join and authentication workflows  
- DNS integration with Active Directory  
- Network configuration and isolation  
- System validation and troubleshooting  

---

## Environment Overview

The lab environment runs on a virtualized infrastructure using **VMware Workstation Pro**.

### Network

| Setting | Value |
|---|---|
| Network Type | Host-only |
| VMware Network | VMnet1 |
| Subnet | 192.168.10.0/24 |

The network is isolated from external networks to simulate an internal enterprise environment.

---

## Architecture


```
Host Machine
│
VMware Workstation Pro
│
VMnet1 (192.168.10.0/24)
│
├─ DC01
│  Windows Server 2022
│  Domain Controller
│  DNS Server
│  192.168.10.10
│
└─ CLIENT01
   Windows 11
   Domain Workstation
   192.168.10.20
```

The domain controller (**DC01**) provides Active Directory Domain Services and DNS.  
**CLIENT01** is joined to the domain and used for authentication and testing.

---

## Infrastructure

| Machine | Operating System | Role | IP Address |
|---|---|---|---|
| DC01 | Windows Server 2022 | Domain Controller / DNS Server | 192.168.10.10 |
| CLIENT01 | Windows 11 | Domain Workstation | 192.168.10.20 |

---

## Lab Progress

| Lab | Topic | Status |
|---|---|---|
| [00 - Lab Environment Setup](./00-Lab-Environment) | Virtual lab infrastructure setup | Completed |
| [01 - Active Directory](./01-Active-Directory) | Domain deployment and identity management | Completed |

Each lab contains structured documentation including implementation, validation, and troubleshooting.

---

## Technologies Used

- VMware Workstation Pro  
- Windows Server 2022  
- Windows 11  
- Active Directory Domain Services  
- DNS Server  
- Windows Command Line (CMD)  
- Bitwarden  

---

## Purpose

- Build practical system administration skills through hands-on implementation  
- Simulate a small enterprise infrastructure environment  
- Develop structured documentation and troubleshooting workflows  