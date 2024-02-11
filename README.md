<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Part 1: Create Virtual Machine in Azure 
- Part 2: Install and enable ISS (Internet Information Services) and CGI in Windows 
- Part 3: Download and install MySQL; Set up Username and Password.
- Part 4: Register PHP
- Part 5: Install osTicket and Configure Permissions
  

<h2>Installation Steps</h2>

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/dcd8f29b-c2fc-4090-b9ab-2d696883888a)

First, create a Resource Group to organize our Azure resources. Then, we deploy a Windows 10 Virtual Machine with 2-4 Virtual CPUs, allowing it to establish a new Virtual Network for seamless communication.

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/e9ef78a6-7675-42f9-8040-7daf5b4f2ace)

Next install IIS with CGI and Common HTTP Features onto your windowms 10 VM. We want to ensure seamless management with the inclusion of the IIS Management Console, facilitating control over CGI and essential HTTP functionalities for efficient application development.

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/eb50a144-5548-4210-b686-69b75661025d)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/f02fdbb6-48fb-428a-91f5-5cbd08b30224)

After installing IIS and CGI, download and install MySQL 5.5.62 on your Windows system. Follow up by launching the Configuration Wizard, opting for a Standard Configuration, and setting the password to any password of your choice for straightforward and secure database setup.

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/a4270b73-6a24-430c-a48e-f3942b8b3022)

After you set the passwored on MYSQL, open ISS as an admninistrator to register PHP. 

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/552bb8ce-15c7-48a6-a169-33a0d8354d0d)

Download osTicket, then streamline the installation process by extracting and copying the "upload" folder to c:\inetpub\wwwroot. Simplify the directory structure by renaming the "upload" folder to "osTicket" within c:\inetpub\wwwroot for a clean and accessible web deployment.`

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/7fd718bb-0deb-4015-baa3-1f9fa5bc63d4)

<h2>Post-Install Configuration Objectives</h2>

This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket. Configure roles like "Supreme Admin," departments such as "System Administrators," and teams like "Level I Support" and "Level II Support" in the admin panel. Enable ticket creation by adjusting user settings and add agents like Jane and John. Set up users like Karen and Ken, define SLAs, and categorize issues with help topics, ensuring efficient management in your system.

<h2>Post-Install Configuration Objectives</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />


