# Edward E. Spence

![Active Directory](https://img.shields.io/badge/Active_Directory-0078D4?style=flat&logo=microsoft&logoColor=white)
![Microsoft Entra ID](https://img.shields.io/badge/Microsoft_Entra_ID-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![HashiCorp Vault](https://img.shields.io/badge/HashiCorp_Vault-1.16-black?style=flat&logo=vault&logoColor=white)
![Delinea](https://img.shields.io/badge/Delinea-Secret_Server-5A2CA0?style=flat)
![Splunk](https://img.shields.io/badge/Splunk-SIEM-000000?style=flat&logo=splunk&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-SAML_Federation-FF9900?style=flat&logo=amazonaws&logoColor=white)
![RHEL](https://img.shields.io/badge/RHEL-Linux_Hardening-EE0000?style=flat&logo=redhat&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-Automation-5391FE?style=flat&logo=powershell&logoColor=white)
![CMMC](https://img.shields.io/badge/CMMC-Level_2-blue?style=flat)
![Zero Trust](https://img.shields.io/badge/Zero_Trust-Architecture-darkgreen?style=flat)

---

## Identity & Access Management Engineer

I build and operate enterprise-grade IAM and PAM environments on real infrastructure. My work covers the full identity lifecycle — from provisioning and access governance to privileged account control, threat detection, and incident response.

Every repository in this profile reflects hands-on engineering executed in a fully operational lab environment — not guided browser exercises. Real Active Directory. Real Entra ID tenant. Real Vault and Delinea deployments. Real Splunk SIEM. Real Linux enforcement.

---

## 🏗️ Lab Environment — IAMPAM.LAB

My home lab simulates a production enterprise identity platform for a fictional aerospace manufacturer operating under **CMMC Level 2** compliance requirements.

```text
Domain          IAMPAM.LAB
Network         172.31.100.0/24
Entra Tenant    FairmountManufacturing.onmicrosoft.com
Compliance      CMMC Level 2
```

| System | Role |
|---|---|
| DC01 | Active Directory Domain Controller |
| MGMT01 | Privileged Access Workstation (PAW) |
| ID-SYNC01 | Microsoft Entra Connect Sync |
| SIEM01 | Splunk Enterprise |
| PAMVAULT01 | HashiCorp Vault |
| DELINEA01 | Delinea Secret Server |
| RHEL01 | Privileged Linux Server |

---

## 🔐 Core Competencies

**Identity Lifecycle Management**
Full JOINER → MOVER → LEAVER lifecycle engineering across Active Directory and Microsoft Entra ID. Bulk provisioning with PowerShell error handling, AAD-Sync-Users scope control, group-based RBAC enforcement, and Entra delta sync validation.

**Privileged Access Management**
HashiCorp Vault LDAP integration, policy-based secret access control, and Delinea Secret Server folder-based RBAC governance. Privileged tier accounts intentionally excluded from Entra ID synchronization per Microsoft Enterprise Access Model — hard boundary between cloud and privileged identity planes enforced by design.

**Hybrid Identity Architecture**
On-premises Active Directory synchronized to Microsoft Entra ID via Entra Connect. AAD-Sync-Users scoping group controls which identities are eligible for cloud synchronization. AWS SAML federation configured for privileged identity groups through the Entra ID identity plane.

**Linux Privileged Access Enforcement**
RHEL hardening with Active Directory integration via SSSD and Kerberos. SSH access control enforced through AllowGroups. Audit logging configured and forwarded to Splunk for visibility. Access validation confirms least privilege enforcement across the Linux tier.

**SIEM-Driven Identity Operations**
Splunk used for identity lifecycle audit validation and threat detection. Windows Security Event log ingestion from DC01. SPL queries built for user creation (4720), group membership (4728), logon activity (4624, 4625), and privilege escalation (4672). Rex field extraction used to normalize raw event data into investigation-ready output.

**Incident Response**
Full IR lifecycle execution — detection, investigation, containment, and validation using Splunk and PowerShell IAM controls. MITRE ATT&CK aligned. Break-glass GPO scenarios documented with architectural rationale.

**Compliance Alignment**
CMMC Level 2 controls mapped across AC, AU, IR, IA, and CM practice families. Evidence documented in lab outputs including Splunk queries, PowerShell results, and validated access control behavior.

---

## 🎓 Certifications

![SEC+](https://img.shields.io/badge/CompTIA-Security%2B-FF0000?style=flat&logo=comptia&logoColor=white)
![SC-900](https://img.shields.io/badge/Microsoft-SC--900-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![Splunk Power User](https://img.shields.io/badge/Splunk-Core_Certified_Power_User-000000?style=flat&logo=splunk&logoColor=white)
![Splunk Admin](https://img.shields.io/badge/Splunk-Enterprise_Certified_Admin-000000?style=flat&logo=splunk&logoColor=white)

- CompTIA Security+
- Microsoft SC-900 — Security, Compliance and Identity Fundamentals
- Splunk Core Certified Power User
- Splunk Enterprise Certified Admin

---

## 📁 Featured Repositories

### 🔵 [HYBRID-IDENTITY-ACCESS-MGMT](https://github.com/eespence/HYBRID-IDENTITY-ACCESS-MGMT)
Enterprise hybrid identity architecture — Active Directory to Microsoft Entra ID synchronization, AWS SAML federation, RBAC governance, and PAM architecture design.

### 🔵 [IAM-PRIVILEGED-ACCESS-ENGINEERING](https://github.com/eespence/IAM-PRIVILEGED-ACCESS-ENGINEERING)
Privileged Access Management deep dive — HashiCorp Vault, Delinea Secret Server, Splunk SIEM integration, RBAC enforcement, and Zero Trust architecture principles.

### 🔵 [RHEL-PRIVILEGED-ACCESS-ENFORCEMENT](https://github.com/eespence/RHEL-PRIVILEGED-ACCESS-ENFORCEMENT)
Linux privileged access enforcement — RHEL hardening, Active Directory integration via SSSD and Kerberos, SSH access control, audit logging, and Splunk visibility.

### 🔵 [FAIRMOUNT-MANUFACTURING-IAM-OPERATIONS](https://github.com/eespence/fairmount-manufacturing-iam-operations)
Full IAM/PAM operations lab for Fairmount Manufacturing LLC. Covers employee onboarding (JOINER lifecycle), incident response, Vault and Delinea PAM governance, Splunk audit validation, AWS SAML federation, and reusable PowerShell automation. CMMC Level 2 aligned.

---

## 🛡️ CMMC Level 2 Coverage

| Practice | Control |
|---|---|
| AC.1.001 | Limit system access to authorized users |
| AC.2.006 | Use non-privileged accounts |
| AC.2.007 | Limit privileged account use |
| AU.2.041 | Audit user management actions |
| AU.2.042 | Review and analyze audit logs |
| IR.2.092 | Establish incident handling capability |
| IR.2.093 | Track and document incidents |
| IA.3.083 | Use multifactor authentication |
| CM.2.061 | Establish baseline configurations |

---

## 🌐 Portfolio & Contact

🌐 [edwards-it-portfolio.com](https://edwards-it-portfolio.com)
💼 [LinkedIn — Edward E. Spence](https://www.linkedin.com/in/edward-e-spence-6598bb312/)
🐙 [GitHub — eespence](https://github.com/eespence)

---

**E.E. Spence — Identity Engineering | IAMPAM.LAB | Washington DC / Northern Virginia**
