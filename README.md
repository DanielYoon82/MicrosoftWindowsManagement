<h1>Home Lab - Managing Computers and Groups in Active Directory</h1>

<h2>Description</h2>
In this virtual machine I demonstrate computer and group management in Active Directory.  
<br />


<h2>Languages and Utilities Used</h2>

- <b>Windows 10</b> 

<h2>Environments Used </h2>

- <b>Windows Server 2019</b>

<h2>Program walk-through:</h2>


- <b>Organizing Groups and Creating OU's for Group Policies</b> <br />
Two OU's, Workstations and Servers, have been created to place computers and servers in. In a professional work environment, it is optimal to segregate devices to set policies.
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

From the computer container, I will move them to the OU's created accordingly. <br />
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG1.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br />

- <b>Group Policy Management</b> <br />
OU's has been organized in which policies can now be deployed using Group Policy Management individually. Group Policy Objects will allow seperate baselines for devices and users. As shown, there are three existing GPO's in my VM.
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG2.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
</p>
<br /> 

The Default Domain Policy has been linked to tml.local domain. In the setting tab I can see that this Default Domain Policy only applies to Computer Configurations. <br />
<br />
<p align="center">
<img src="https://github.com/DanielYoon82/ActiveDirectoryComputersGroups/blob/main/image/ActiveDirectoryCG3.jpg" height="85%" width="85%" alt="Disk Sanitization Steps"/>
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
