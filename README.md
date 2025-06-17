<h1>Active-Directory-Home-Lab
</h1>


<h2>Description</h2>
🏢 Active Directory Home Lab (Portfolio Project)
As part of my technical portfolio, this project showcases my ability to design and deploy a fully functional Active Directory (AD) environment using VirtualBox on a local machine.

The lab simulates a real-world Windows enterprise network and includes:

🔐 Windows Server 2019 as a Domain Controller with DNS & DHCP roles

👥 Windows 10 client machines joined to the domain

⚙️ Group Policy Objects (GPOs) for centralized configuration

🌐 Isolated virtual network simulating a secure enterprise environment

🧠 What This Demonstrates
Proficiency in Windows Server administration

Strong understanding of Active Directory architecture

Practical experience with domain joins, user/group creation, GPOs, and networking

The ability to build, troubleshoot, and automate a multi-VM environment

This hands-on lab reinforces my foundational knowledge of enterprise identity management and IT infrastructure, and reflects my capability to work in environments where system administration, security, and network configuration intersect.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 


<h2>Environments Used </h2>

- <b>Windows 10</b> 

<h2>## 📋 Step-by-Step Overview

### 1. Install VirtualBox and Create VMs
- Create two VMs: one for the **Domain Controller**, one for the **Windows 10 Client**
- Configure **dual NICs** on the DC: `NAT` for internet, `Internal Network` for lab

### 2. Set Static IP & Install Server Roles
- Assign a static internal IP (e.g., `172.16.0.1`)
- Install **AD DS, DNS, DHCP**, and **Remote Access (Routing)** via Server Manager

### 3. Promote Server to Domain Controller
- Set up a new AD forest (e.g., `labdomain.local`)
- Configure DNS during promotion
- Restart and verify domain services

### 4. Configure DHCP & NAT
- Set DHCP scope for internal network (e.g., `172.16.0.100–200`)
- Use NAT to enable internet access for internal clients

### 5. Automate User Creation with PowerShell
- Modify `names.txt` with sample user names
- Use a custom PowerShell script to generate hundreds of users in the domain

### 6. Join Windows 10 Client to Domain
- Assign to internal network
- Set DNS to point to Domain Controller
- Join domain and test login with created users

---

## ✅ Skills Demonstrated

- 🧩 Active Directory design and deployment  
- 🛜 Windows networking, DNS/DHCP configuration  
- 🧪 Troubleshooting domain join and NAT issues  
- 💬 PowerShell scripting for bulk account provisioning  
- 💡 Real-world enterprise environment simulation

---

## 🚀 Why This Lab Matters

This project reflects my ability to create and manage secure, scalable, and realistic Windows infrastructure environments. It's an essential foundation for roles in:

- IT Support / Help Desk
- System Administration
- Cybersecurity Engineering
- Identity & Access Management (IAM)

---

## 📎 Resources

- [Windows Server Eval ISO](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)
- [Windows 10 ISO](https://www.microsoft.com/software-download/windows10)
- [Oracle VirtualBox](https://www.virtualbox.org/)
- [FLARE VM (for malware labs)](https://github.com/mandiant/flare-vm) *(optional)*

---

### 🧠 “Build it. Break it. Rebuild it.”

