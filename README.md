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
- Part 4: Install C++ Redistributable
- Part 5: Install osTicket and Configure Permissions
  

<h2>Installation Steps</h2>

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/dcd8f29b-c2fc-4090-b9ab-2d696883888a)

First, we create a Resource Group to organize our Azure resources. Then, we deploy a Windows 10 Virtual Machine with 2-4 Virtual CPUs, allowing it to establish a new Virtual Network for seamless communication.

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/e9ef78a6-7675-42f9-8040-7daf5b4f2ace)

Next we will enable a robust web server on our Windows 10 VM by installing IIS with CGI and Common HTTP Features. We want to ensure seamless management with the inclusion of the IIS Management Console, facilitating control over CGI and essential HTTP functionalities for efficient application development.

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/eb50a144-5548-4210-b686-69b75661025d)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/13f5d63a-ce52-4d01-bee8-7d088dcc3ffe)
  
After installing ISS and CGI, download and install MySQL 5.5.62 on your Windows system. Follow up by launching the Configuration Wizard, opting for a Standard Configuration, and setting the password to any password of your choice for straightforward and secure database setup.
