# ☁️ Cloud-Based Active Directory Setup & User Management

A hands-on cybersecurity lab documenting the deployment of a small enterprise-style **Active Directory (AD) environment in Microsoft Azure** — covering domain controller setup, client domain join, user/OU management, and Windows Security event log monitoring.

📄 **[Read the full lab report (PDF) →](docs/CloudBased_AD_Setup_and_User_Management.pdf)**
🧭 **[Read the narrative walkthrough with troubleshooting →](docs/LAB-WALKTHROUGH.md)**

---

## 🎯 Goal

Build practical, hands-on experience with the identity and access management concepts a SOC analyst or Windows security practitioner works with daily — provisioning cloud infrastructure, standing up a real Active Directory domain from scratch, managing users, and reading the security telemetry that domain generates.

---

## 📝 Description

This project simulates a small enterprise identity environment end-to-end:

- Provisioning two Windows Server virtual machines in Azure on a shared virtual network
- Installing Active Directory Domain Services (AD DS) and promoting a server to a Domain Controller, creating a new forest (`corp.local`)
- Joining a client machine to the domain and validating authentication
- Creating Organizational Units and user accounts, and managing group membership
- Reviewing Windows Security event logs and mapping key Event IDs (logons, account management, group changes) to the actions that generated them — the same correlation work performed during SOC investigations

The full step-by-step walkthrough, actual deployment configuration, screenshots, and troubleshooting encountered along the way are documented in the [`docs/`](docs) folder.

---

## ✅ Requirements / Prerequisites

- A cloud provider free tier (this lab uses **Microsoft Azure**, which offers a 12-month free tier including Windows VMs)
- Two Windows Server VMs (e.g. Windows Server 2022 — Desktop Experience, not Server Core)
- Remote Desktop (RDP) access to the VMs
- Basic familiarity with Windows Server and networking concepts

---

## 🛠️ Tools & Technologies

- **Microsoft Azure** — VM provisioning, Virtual Networks, NSGs, Resource Groups
- **Windows Server 2022** — Active Directory Domain Services, DNS Server role
- **Active Directory Users and Computers (ADUC)** — OU/user/group management
- **Windows Event Viewer** — Security log analysis

---

## 📁 Repository Structure

```
├── README.md
└── docs/
    ├── CloudBased_AD_Setup_and_User_Management.docx   # Full lab report (source)
    ├── CloudBased_AD_Setup_and_User_Management.pdf    # Full lab report (viewable)
    ├── LAB-WALKTHROUGH.md                             # Narrative walkthrough w/ real troubleshooting + screenshots
    └── images/                                        # Screenshots referenced by LAB-WALKTHROUGH.md
```

---

## 📌 Notes

This lab was completed independently as part of ongoing hands-on preparation for SOC analyst / cybersecurity roles, building on foundational knowledge from CompTIA Security+.
