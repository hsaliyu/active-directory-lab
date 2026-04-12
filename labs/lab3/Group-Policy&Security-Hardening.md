📌 Overview

This lab focuses on implementing Group Policy Objects (GPOs) to enforce security controls within an Active Directory environment.

The goal was to simulate enterprise-level security by applying password policies, account lockout rules, and user restrictions.

🧰 Environment
OS: Windows Server 2022
Platform: VMware Workstation
Domain: lab.local
🎯 Objectives
Apply Group Policy Objects (GPOs)
Enforce password and account security policies
Implement user-level restrictions
Strengthen endpoint security posture
⚙️ GPO Configurations Implemented
1. 🔑 Password Policy (Domain Level)

Configured via Default Domain Policy:

Minimum password length: 8 characters
Password complexity: Enabled
Maximum password age: 30 days
Minimum password age: 1 day
Password history: 5 passwords

📍 Path:
Computer Configuration → Policies → Windows Settings → Security Settings → Account Policies → Password Policy

2. 🚫 Account Lockout Policy

Configured to prevent brute-force attacks:

Account lockout threshold: 5 failed attempts
Lockout duration: 15 minutes

📍 Path:
Computer Configuration → Policies → Windows Settings → Security Settings → Account Policies → Account Lockout Policy

3. ⏱️ Screen Timeout Enforcement

Configured to improve session security:

Screen saver timeout: 600 seconds (10 minutes)
Password protection on resume: Enabled

📍 Path:
User Configuration → Policies → Administrative Templates → Control Panel → Personalization

4. 🔒 Restrict Control Panel Access

Prevented users from accessing system settings:

Prohibit access to Control Panel: Enabled

📍 Path:
User Configuration → Policies → Administrative Templates → Control Panel

🔗 GPO Deployment
Created a custom GPO: GPO-IT-Security-Baseline
Linked GPO to the IT Organisational Unit (OU)
Applied policies to users within the OU
✅ Outcome
Successfully enforced password and account security policies
Reduced risk of unauthorised access and brute-force attacks
Implemented user restrictions to limit system changes
Demonstrated practical use of Group Policy in an enterprise environment
🧠 Key Learnings
Password policies must be applied at the domain level
GPOs can be scoped using Organisational Units (OUs)
Security policies can enforce both user and computer configurations
Group Policy is critical for centralised security management
🚀 Next Steps
Join a Windows client machine to the domain
Test GPO enforcement using gpupdate /force and gpresult /r
Implement Group Policy for software restrictions
Configure auditing and logging policies
