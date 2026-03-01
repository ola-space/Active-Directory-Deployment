# Active Directory Simulation – BLU

## 📖 Project Overview

This project demonstrates the deployment of a Windows Server Domain Controller (Active Directory) 
for a simulated company called **BLU**.

The implementation includes:

- Domain setup
- Client configuration
- Organizational Unit (OU) design
- Group Policy configuration
- Access control enforcement

This lab aligns with:

- NIST CSF – Protect (PR)
- ISO 27001 Annex A – Access Control (A.5.15–A.5.23)

---

## 🏢 Company Structure

BLU is an IT services organization with the following structure:

- 1 Windows Server (Active Directory Domain Controller)
- 1 Windows 8 PC (IT Department)
- 1 Windows 8 PC (SALES Department)

---

## 🎯 Project Objectives

- Configure Active Directory Domain Services (AD DS)
- Promote Windows Server to Domain Controller
- Configure DNS & DHCP
- Join client PCs to the domain
- Create Organizational Units (IT & SALES)
- Implement Group Policies for access control
- Enforce least privilege principle

---

## 🌐 Network Design

Internet
↓
Router (Gateway: 10.0.2.1)
↓
Switch
├── Server (10.0.2.4)
├── PC1 - Windows 8 (10.0.2.15)
└── PC2 - Windows 8 (10.0.2.5)

---

## 🖥️ Device Configuration

| Device            | IP Address | Role                          |
|-------------------|------------|-------------------------------|
| Windows Server    | 10.0.2.4   | AD Domain Controller (DC)     |
| Windows 8 PC      | 10.0.2.15  | IT Client                     |
| Windows 8 PC      | 10.0.2.5   | SALES Client                  |

---

## 🏢 Domain Configuration

- **Domain Name:** blu.co
- **Server Name:** blu

---

## 🔐 Security Controls Implemented

- Password Policy Enforcement
- Account Lockout Policy
- Role-Based Access Control (RBAC)
- GPO Desktop Restrictions (IT)
- Administrative Privileges (IT)
- Least Privilege Enforcement

---

## 📸 Screenshots

- AD Domain Structure
- GPO Editor Screenshot
- PC joined to domain
- Result of denied shutdown/restart access

---

## 📚 Lessons Learned

- Importance of DNS in AD functionality
- Proper OU design simplifies policy management
- Group Policy centralizes security enforcement
- Documentation improves incident response readiness

---

## 🚀 Future Improvements

- Implement SIEM monitoring (e.g., Splunk)
- Simulate brute force detection
- Enable advanced auditing policies

---

## Author
Olanipekun Babatunde
