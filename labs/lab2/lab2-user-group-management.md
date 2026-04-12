# Lab 2: Active Directory User & Group Management

## Objective
To design and implement a structured Active Directory environment by creating Organizational Units (OUs), users, and security groups, and applying group-based access control.

## Environment
- Windows Server 2022
- Active Directory Users and Computers (ADUC)

## 1. Organizational Unit (OU) Creation

Created departmental OUs to logically separate users based on business function:

- IT
- HR
- Sales

This structure reflects a typical enterprise environment and supports efficient management and policy application.

## 2. User Creation

Users were created within their respective OUs with relevant attributes such as job title and department to simulate a real-world directory.

### IT Department:
- daniel.carter (IT Administrator)
- aisha.bello (Support Engineer)
- michael.chen (Network Engineer)

### HR Department:
- sarah.johnson (HR Manager)
- david.okafor (HR Officer)
- emily.turner (Recruiter)

### Sales Department:
- james.smith (Sales Executive)
- fatima.ahmed (Account Manager)
- lucas.brown (Sales Representative)

## 3. Security Group Creation

Created security groups to implement role-based access control (RBAC):

- IT_Admins
- HR_Staff
- Sales_Team

Group Type: Security  
Group Scope: Global  


## 4. Group Membership Assignment

Users were assigned to groups based on their department:

### IT_Admins:
- daniel.carter  
- aisha.bello  
- michael.chen  

### HR_Staff:
- sarah.johnson  
- david.okafor  
- emily.turner  

### Sales_Team:
- james.smith  
- fatima.ahmed  
- lucas.brown  

This demonstrates the use of RBAC to manage access efficiently.


## Outcome
Successfully implemented a structured Active Directory environment with departmental OUs, realistic user accounts, and group-based access control.

## Skills Demonstrated
- Organizational Unit (OU) Design
- User Account Creation and Management
- Security Group Configuration
- Role-Based Access Control (RBAC)
- Directory Structuring Based on Business Functions
