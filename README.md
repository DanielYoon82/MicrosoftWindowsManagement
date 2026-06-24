<h1>Home Lab - Managing With Microsoft Windows 10 Pro</h1>

<h2>Description</h2>
Here, I will employ various practices for general management of policies and configurations. This will demonstrate the core understanding of the Windows platform capability.
<br />



<h2>Environments Used </h2>

- <b>Windows 10 Pro</b>

<h2>Program walk-through:</h2>


- <b>User Account Control (UAC)</b> <br />
This feature enhances access control ensuring applications execute in non-admistrator accounts. This follows the Principle of Least Privelege which helps mitigate potential malware impact. To access:  Control Panel -> User Accounts -> Change User Account Control Setting.
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT1.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

Four different settings can be chosen. Here, the option chosen will allow the Administrator to always be notified when changes are made and new software is installed. <br />
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT2.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br />

- <b>Local Policy and Group Policies Editor</b> <br />
This editor can implement local and group policies. It can be used for a network or workstations to limit executions of vulnerable extensions, set password policies, and other administrative settings. This can be accessed through the search bar by typing in "local group."
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT3.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

- <b>Password Policies</b> <br />
This ensures complex and strong passwords for user accounts. Placing certain rules maximizes security. Password complexity requirements was enabled with a minimum of 10 characters. This was accessed with the path: Security settings > Account Policies > Password policy
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT4.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br />

- <b>Setting a Lockout Policy</b> <br />
To protect the password from being guessed by an attacker, a lockout threshold is set for three attempts. This can be accessed by path:  Local Security Policy > Windows Settings > Account Policies > Account Lockout Policy  
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT5.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

- <b>Windows Defender Firewall</b> <br />
Built-in application that protects computers from malicious attacks and blocks unauthorized traffic through inbound and outbound rules. This is accessible through the search bar by typing "Windows Defender" for auto-prompt selection. Path accessed: Advanced Settings > Windows Defender Firewall Properties. I can see that Domain, Private, and Public are all set to default including blocking inbound connections.
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT6.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

- <b>Disable Unused Networking Devices</b> <br />
Network devices such as routers, ehternet cards, WiFi adapters etc., enable data sharing between computers. If not being used by the owner, it should be disabled for security reasons. It accessed by path: Control panel > System and Security Setting > System > Device Manager
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/MicrosoftWindowsManagement/blob/main/images/Windows10MGMT7.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br /> 


- <b>Summary</b> <br />
I demonstrated managing and configuring users, groups, password policies, firewall, and disabling network devices with Windows 10 Pro. Delegating controls on an administrative level was used in a real world simulation with VM.
<br />
<br />
