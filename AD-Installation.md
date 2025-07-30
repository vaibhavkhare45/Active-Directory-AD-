Windows Server Download Links
⚠️ These are official Microsoft evaluation ISO downloads (180-day trial).
Sign in with a free Microsoft account.
Windows Server 2025 (Preview)
👉[ Download ISO](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2025)
Windows Server 2022
👉 [ Download ISO ](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022)

Windows Server 2019
👉 [ Download ISO ](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)

Windows 10 Client (for domain join)
👉 [Download Windows 10 ISO](https://www.microsoft.com/en-in/software-download/windows10)

📌Prerequisites
  VMware Workstation or VirtualBox
  2 Virtual Machines:
    Windows Server (Domain Controller)
    Windows 10 (Client)
  At least 4 GB RAM, 2 CPUs, 50 GB storage for the server

🔹 Step 1: Install Windows Server
1. Create a new VM and attach the Windows Server ISO.
2. Install Windows Server normally.
3. Create a strong password for the Administrator account.

 🔹 Step 3: Install Active Directory Domain Services
1. Open Server Manager.
2. Click Manage → Add Roles and Features.
3. Choose Role-based installation.
4. Select the local server.
5. In Server Roles, check:
    ✅ Active Directory Domain Services
    ✅ DNS Server (auto selected)
6. Click Install.
