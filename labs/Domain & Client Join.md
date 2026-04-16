# Lab: Active Directory Domain Setup & Client Join

## Objective
To deploy a Windows Server 2022 domain controller, configure Active Directory, and join a Windows 11 client machine to the domain.

## Environment
- VMware Workstation
- Windows Server 2022 (Domain Controller)
- Windows 11 (Client Machine)

---

## 1. Domain Controller Setup
- Installed Windows Server 2022 on VMware
- Promoted the server to a Domain Controller
- Configured Active Directory Domain Services (AD DS)
- Created a new domain (e.g., homelab.local)

---

## 2. Organizational Unit (OU) Structure
Created three Organizational Units:
- IT
- HR
- Finance

---

## 3. User Management
- Created multiple domain user accounts
- Assigned users to appropriate OUs

---

## 4. Windows 11 Client Setup
- Installed Windows 11 on VMware
- Configured network settings

---

## 5. Issue Encountered: Domain Join Failure
- Initial attempt to join the domain failed

### Root Cause:
- Client machine was not using the Domain Controller as its DNS server

---

## 6. Resolution
- Manually configured the Windows 11 DNS to point to the Domain Controller's IP address

---

## 7. Outcome
- Successfully joined Windows 11 to the domain
- Logged in using domain user credentials
- Verified connectivity and domain functionality

---

## Key Learning
- Active Directory relies on DNS for domain discovery and authentication
- Proper DNS configuration is critical for domain-joined environments
