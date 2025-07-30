# Active Directory Security Lab
This project is a **hands-on guide to setting up and understanding Active Directory (AD)**, its core components, and how attackers often exploit it.  
It also provides practical defense strategies to secure AD environments.

## 🔹 Objectives
- Install and configure Active Directory in a lab environment  
- Understand the working of AD and its key components  
- Explore **famous Active Directory attacks**  
- Implement countermeasures to secure the environment

## 🔹 Lab Setup
- **Windows Server 2022** (Domain Controller)
- **Windows 10 Client** (Domain-joined machine)
- **Kali Linux** (Attacker machine)
- Virtualization Platform: **VMware Workstation / VirtualBox**
See [AD-installation.md](AD-installation.md) for detailed instructions

## 🔹 Famous Active Directory Attacks
Detailed in [Attacks-On-AD.md](Attacks-On-AD.md):
- **Pass-the-Hash (PtH)**  
- **Pass-the-Ticket (PtT)**  
- **Kerberoasting**  
- **DCSync Attack**  
- **Golden Ticket Attack**  
- **Silver Ticket Attack**  
- **Mimikatz Credential Dumping**  
- **AS-REP Roasting**  

## 🔹 Defense and Countermeasures
See [Countermeasures.md](Countermeasures.md):

- Enforce **strong Kerberos policies**
- Implement **Privileged Access Management (PAM)**
- Regularly **rotate service account passwords**
- Use **Event Logging & Monitoring**
- Apply **Least Privilege** principle
- Deploy **Endpoint Detection & Response (EDR)**

## 🔹 Learning Outcomes
By the end of this project, you’ll:
- Have a working **Active Directory lab**  
- Understand **how attackers target AD**  
- Be able to demonstrate **defensive strategies**  
- Showcase a practical security project on your **resume & GitHub**
