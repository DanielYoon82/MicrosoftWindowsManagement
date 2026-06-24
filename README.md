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

Basic configurations are discovered that apply to most domains including password and account lockout policies. <br />
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG4.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br />

As a demonstration, a new policy has been set to use a minimum of 10 characters for passwords. The GPO Default Domain Policy was chosen to edit for all computers.   <br />
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG5.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br />

From there navigating to: Computer Configurations -> Policies -> Windows Setting -> Security Settings -> Account Policies -> Password Policy and changing the required policy value to 10.    <br />
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG6.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br />

- <b>Restricting Access to Control Panel</b> <br/>
Here, I would like to restrict access to the Control Panel in exception to the IT Department. I created a new GPO named "Restrict Control Panel Access."  <br />
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG7.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br />

User Configuration -> Administrative Templates -> Control Panel -> was then accessed in the editor to enable the feature to restrict access.  <br />
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG8.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br />

In Group Policy Management, by dragging the GPO Restrict Control Panel Accesss to the departments other than IT, I successfully restricted access to the Control Panel.  <br />
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG9.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br />

- <b>Auto Lock Screen in GPO</b> <br />
A new GPO was created named Auto Lock Screen. This will allow me to change policies from the root domain.
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG10.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

In the editor I accessed Computer Configurations -> Policies -> Windows Setting -> Security Settings -> Local Policies -> Security Options. I see that Machine Inactivity Limit is Not Defined. Edit was performed and set to inactivity limit to 5 minutes (300 seconds)  <br />
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG11.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br />

The new GPO was dragged into the root tml.local for enabling completing the task.  <br />
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG12.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br />


- <b>Summary</b> <br />
Using Windows Active Directory with modeling a VM in creating OU's, creating group policies, changing password policy, managing restricted access, and configuring auto lock screen was displayed. Managing computers and group policies was broken down using a VM as a simulation.
<br />
<br />
