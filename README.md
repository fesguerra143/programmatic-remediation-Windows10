

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


- [Step 1) Log into the VM and disable the Windows Firewall](#step-2-log-into-the-vm-and-disable-the-windows-firewall)
- [Step 2) Login to tenable](#step-3-login-to-tenable)
- [Step 3) Create a Custom Scan](#step-4-create-a-custom-scan)
- [Step 4) Remediation Implementation](#step-5-remediation-implementation)
- [Step 5) Scan Results After Remediation](#step-6-scan-results-after-remediation)
---





---
### Step 1) Log into the VM and disable the Windows Firewall 

#### Bastion Connection:

<img width="700" alt="rdp" src="https://github.com/user-attachments/assets/cbed6adf-9061-4fe8-a49e-5e4061ac9ebb" />


#### Disable Windows Firewall 

<img width="700" alt="wf" src="https://github.com/user-attachments/assets/b2cc7376-5bc6-4cf1-82ad-e549a2c393ee" />

---

### Step 2) Login to tenable

<img width="400" alt="tenablelogin" src="https://github.com/user-attachments/assets/65aa3c73-113b-4b85-8b79-de3a142d4e4b" />

---

### Step 3) Create a Custom Scan

#### Select a DISA STIG Template

<img width="700" alt="scan" src="https://github.com/user-attachments/assets/4f4080e2-8a6f-478c-bbb8-d03fc46a32a9" />


#### Configure Scan Basic settings

<img width="700" alt="credentials" src="https://github.com/user-attachments/assets/18a0ca1f-7065-4e2a-9d10-8c28267efaf0" />

#### Configure Scan Credential settings

<img width="700" alt="credentials" src="https://github.com/user-attachments/assets/606215a5-f8da-466c-bcd1-edbdbbd42ddb" />

#### Scan Results Prior Remediation
<img width="700" alt="scan results" src="https://github.com/user-attachments/assets/4f0b71f1-f2a7-4141-a21c-3a6accac36fd" />


#### [Tenable Vulnerability Management Report](https://drive.google.com/file/d/1nMRHKEVorILV_Hu9w-JCPfZ9BqZymT0g/view?usp=sharing)
---
### Step 4) Remediation Implementation

##### Remediate FireFox

<img width="400" alt="scan results" src="https://github.com/user-attachments/assets/8bb0add0-ae35-411e-bdcd-f267df0f28fe" />


[Remediation PowerShell Script](remediation/remediation-FireFox-uninstall.ps1)

##### Remediate SMB v1
<img width="400" alt="scan results" src="https://github.com/user-attachments/assets/2c974f26-b78f-47d3-92cc-1c8a1f647c02" />

[Remediation Powershell Script](remediation/remediation-SMBv1.ps1)


##### Remediate discouraged cryptographic protocols
<img width="400" alt="scan results" src="https://github.com/user-attachments/assets/72b61abf-5959-4ab0-8ed5-b992bdf36cbf" />


[Remediation Powershell Script](https://github.com/fesguerra143/automation/blob/cc635a606dfa9d55829f1b4ffbe6a9d34a4debad/toggle-protocols.ps1)



---
### Step 5) Scan Results After Remediation

<img width="700" alt="scan results" src="https://github.com/user-attachments/assets/57c73500-cfc4-4cdb-9b9a-a4cc93103aa8" />


#### [Tenable Vulnerability Management Report](https://drive.google.com/file/d/1_M0wvOA_Ny5vVql6tYUPwE0a6QHjss8H/view?usp=drive_link)


---
