<h1>Home Lab - Windows 10 Security & System Administration</h1>

<h3>Project Overview</h3>
This home lab demonstrates common Windows 10 administrative and security configuration tasks performed by IT Support and Desktop Support professionals. The project focuses on securing Windows workstations through User Account Control (UAC), Local Group Policy, password and account lockout policies, Windows Defender Firewall configuration, and hardware management while following Windows security best practices. 
<br />

<h3>Objectives </h3>

- Configure User Account Control (UAC)
- Manage Local Group Policy settings
- Implement password security policies
- Configure account lockout policies
- Review Windows Defender Firewall settings
- Disable unused network adapters to improve security
- Demonstrate Windows security hardening techniques

<h3>Environment </h3>

- Windows 10 Pro
- Local Group Policy Editor (gpedit.msc)
- Local Security Policy
- Windows Defender Firewall
- Device Manager

<h3>Skills Demonstrated </h3>

- Windows 10 Administration
- Security Hardening
- User Account Control (UAC)
- Local Group Policy
- Password Policy Configuration
- Account Lockout Policy
- Windows Defender Firewall
- Endpoint Security
- Device Management
- Principle of Least Privilege
</p>  
<br />

<br />
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMTWorkflow.jpg" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

<h2>Step 1 – Configure User Account Control (UAC)</h2>

<h3>Actions Performed </h3>

- Opened Control Panel → User Accounts
- Accessed Change User Account Control Settings

<h3>Purpose </h3>

User Account Control helps enforce the Principle of Least Privilege by requiring administrator approval before system-level changes are made.
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT1.jpg" height="95%" width="95%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

- Reviewed the available notification levels
- Configured UAC to Always Notify
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT2.jpg" height="95%" width="95%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h2>Step 2 – Configure Local Group Policy (UAC)</h2>

<h3>Actions Performed </h3>

- Opened Local Group Policy Editor (gpedit.msc)
- Reviewed available administrative templates
- Examined local computer and user configuration policies
- Identified security-related policy settings used to manage workstation behavior

<h3>Purpose </h3>

Local Group Policy allows administrators to centrally manage security and operating system behavior on standalone Windows systems.
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT3.jpg" height="95%" width="95%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

<h2>Step 3 – Configure Password Policy (UAC)</h2>

<h3>Actions Performed </h3>

- Opened Local Security Policy
- Navigated to: Security Settings → Account Policies → Password Policy
- Enabled password complexity requirements
- Configured a minimum password length of 10 characters
- Verified the updated password policy

<h3>Purpose </h3>

Strong password policies help protect user accounts against brute-force and dictionary attacks.
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT4.jpg" height="95%" width="95%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h2>Step 3 – Configure Password Policy (UAC)</h2>

<h3>Actions Performed </h3>

- Navigated to: Security Settings → Account Policies → Account Lockout Policy
- Configured an account lockout threshold of 3 failed logon attempts
- Reviewed lockout duration settings
- Verified the policy configuration

<h3>Purpose </h3>

Account lockout policies reduce the effectiveness of password-guessing attacks by temporarily locking compromised accounts.
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT5.jpg" height="95%" width="95%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

<h2>Step 3 – Configure Password Policy (UAC)</h2>

<h3>Actions Performed </h3>

- Opened Windows Defender Firewall with Advanced Security
- Reviewed Domain, Private, and Public firewall profiles
- Verified inbound and outbound firewall settings
- Confirmed Windows Defender Firewall was enabled for all network profiles

<h3>Purpose </h3>

Windows Defender Firewall helps prevent unauthorized network access while allowing approved applications and services to communicate securely.
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT6.jpg" height="95%" width="95%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

<h2>Step 6 – Disable Unused Network Adapters (UAC)</h2>

<h3>Actions Performed </h3>

- Opened Device Manager
- Reviewed installed network adapters
- Identified unused networking devices
- Disabled unnecessary adapters to reduce the system's attack surface

<h3>Purpose </h3>

Disabling unused hardware reduces potential security risks and simplifies workstation management.
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT7.jpg" height="95%" width="95%" alt="Disk Sanitization Steps"/>
</p>
<br /> 


<h3>Administrative Tasks Demonstrated </h3>

- Windows workstation administration
- User Account Control configuration
- Local Group Policy management
- Password policy administration
- Account lockout configuration
- Windows Defender Firewall management
- Device Manager administration
- Endpoint security hardening

<h3>Key Takeaways </h3>

This lab demonstrates practical Windows 10 administration and security hardening techniques commonly performed by Help Desk, Desktop Support, and Junior Systems Administrators. By configuring User Account Control, password policies, account lockout settings, Windows Defender Firewall, and Local Group Policy, administrators can improve workstation security, enforce organizational standards, and reduce the risk of unauthorized access.
<br />
<br />
