

# Programmatic Vulnerability Remediation Project

This project is about remediating a Windows 10 VM with the following vulnerabilities using DISA STIG Compliance vulnerability scan:
- Old Version of FireFox: Insecure Software Windows
- Enable SMB v1
- Enable discouraged cryptographic protocols: SSL 2.0, SSL 3.0, TLS 1.0, TLS 1.1 

![Windows 10](https://github.com/user-attachments/assets/09eb2273-339e-418a-b74c-ec3672980485)

---
# Tools & Technology:
- Tenable (enterprise vulnerability management platform)
- Azure Virtual Machine
- PowerShell


---
# Table of contents

- [Step 1) Create a Windows virtual machine in the Azure portal](#step-1-create-a-windows-virtual-machine-in-the-azure-portal)
- [Step 2) Log into the VM and disable the Windows Firewall](#step-2-log-into-the-vm-and-disable-the-windows-firewall)
- [Step 3) Administrator Account & Assign Group](#step-3-administrator-account--assign-group)
- [Step 4) Guest Account & Assign Group](#step-4-guest-account--assign-group)
- [Step 5) Login to tenable](#step-5-login-to-tenable)
- [Step 6) Create a Scan Template](#step-6-create-a-scan-template)
- [Step 7) Create a Custom Scan](#step-7-create-a-custom-scan)

---


### Step 1) Provision virtual machine in the Azure portal

<img width="700" alt="vm7" src="https://github.com/user-attachments/assets/9e8c5e4a-3348-47c4-9565-a3958e21ee9b" />


---
### Step 2) Log into the VM and disable the Windows Firewall 

#### Bastion Connection:

<img width="700" alt="rdp" src="https://github.com/user-attachments/assets/cbed6adf-9061-4fe8-a49e-5e4061ac9ebb" />


#### Disable Windows Firewall 

<img width="700" alt="wf" src="https://github.com/user-attachments/assets/b2cc7376-5bc6-4cf1-82ad-e549a2c393ee" />

---

### Step 3) Login to tenable

<img width="700" alt="tenablelogin" src="https://github.com/user-attachments/assets/65aa3c73-113b-4b85-8b79-de3a142d4e4b" />

---

### Step 4) Create a Custom Scan

#### Select a DISA STIG Template

<img width="700" alt="scan" src="https://github.com/user-attachments/assets/4f4080e2-8a6f-478c-bbb8-d03fc46a32a9" />


#### Configure Scan Basic settings

<img width="700" alt="credentials" src="https://github.com/user-attachments/assets/18a0ca1f-7065-4e2a-9d10-8c28267efaf0" />

#### Scan Results Prior Remediation
<img width="700" alt="scan results" src="https://github.com/user-attachments/assets/4f0b71f1-f2a7-4141-a21c-3a6accac36fd" />


#### [Tenable Vulnerability Management Report](https://drive.google.com/file/d/1R3h84jjpO8A4EtUGahOlA8-Atyq1xzO9/view?usp=sharing)


##### Scan Results After Implementing Remediation
<img width="700" alt="scan results" src="https://github.com/user-attachments/assets/2cf0f6bb-51c9-4052-9649-7a3049937a0e" />

#### Tenable Vulnerability Management Report
[Tenable Vulnerability Management Report](https://drive.google.com/file/d/1wsiYlNjNFqvXqji4pbG02z2_a-n1-Hs_/view?usp=drive_link)


---
