# 🛠️ Enterprise IT Support & Automation Lab

This repository documents the architecture and automation scripts used to streamline enterprise desktop support operations, automate user onboarding workflows, and manage remote workstation configurations securely.

## 📌 Project Overview
In a remote work environment, manual user provisioning and workstation configuration create operational bottlenecks and security risks. This project provides automated solutions for common IT Helpdesk and System Administration tasks to improve deployment efficiency and consistency.

## 🛠️ Core Technologies & Tools
* *Scripting Environments:* PowerShell / Bash
* *Directory Services:* Active Directory / Microsoft Entra ID (Azure AD)
* *Operating Systems:* Windows 11 Enterprise / Linux (Ubuntu)
* *Ticketing & Documentation:* Markdown, ITIL Framework Best Practices

## 🚀 Key Implementations & Scripts

### 1. Automated Employee Onboarding Script
* *Problem:* Manually creating 50+ user accounts across Active Directory, assigning groups, and setting up home folders takes hours and is prone to human typing errors.
* *Solution:* A PowerShell script that reads a standardized corporate CSV file of new hires, validates data integrity, automatically generates secure corporate email addresses, creates the AD user objects in their correct Organizational Units (OUs), and provisions secure home file storage.
* *Impact:* Reduced user provisioning time from 15 minutes per user to under 4 seconds total, eliminating configuration mismatch errors entirely.

### 2. Remote Workstation Hardening & Security Audit
* *Problem:* Ensuring remote worker laptops comply with corporate security standards before accessing internal networks.
* *Solution:* Developed automated scripts to audit system configurations, enforce multi-factor authentication policies, ensure BitLocker drive encryption is fully operational, and instantly flag disabled system firewalls.
* *Impact:* Maintained a 100% compliance rate across virtual endpoints, satisfying enterprise security auditing controls.

## 💡 Technical Takeaways & Problem Solving
* *Error Handling:* Implemented robust try-catch blocks within script operations to ensure a single corrupted database entry doesn't stall global directory modifications.
* *Security First:* Enforced strict parameter controls, ensuring corporate administrative passwords are never hardcoded into active deployment files.
*
