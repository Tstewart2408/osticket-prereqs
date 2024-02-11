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

First, create a Resource Group to organize our Azure resources. Then, we deploy a Windows 10 Virtual Machine with 2-4 Virtual CPUs, allowing it to establish a new Virtual Network for seamless communication.

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/dcd8f29b-c2fc-4090-b9ab-2d696883888a)

Next install IIS with CGI and Common HTTP Features onto your windowms 10 VM. We want to ensure seamless management with the inclusion of the IIS Management Console, facilitating control over CGI and essential HTTP functionalities for efficient application development.

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/e9ef78a6-7675-42f9-8040-7daf5b4f2ace)

After installing IIS and CGI, download and install MySQL 5.5.62 on your Windows system. Follow up by launching the Configuration Wizard, opting for a Standard Configuration, and setting the password to any password of your choice for straightforward and secure database setup.

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/eb50a144-5548-4210-b686-69b75661025d)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/f02fdbb6-48fb-428a-91f5-5cbd08b30224)

After you set the passwored on MYSQL, open ISS as an admninistrator to register PHP. 

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/a4270b73-6a24-430c-a48e-f3942b8b3022)

Download osTicket, then streamline the installation process by extracting and copying the "upload" folder to c:\inetpub\wwwroot. Simplify the directory structure by renaming the "upload" folder to "osTicket" within c:\inetpub\wwwroot for a clean and accessible web deployment.

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/552bb8ce-15c7-48a6-a169-33a0d8354d0d)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/7fd718bb-0deb-4015-baa3-1f9fa5bc63d4)

<h2>Post-Install Configuration Objectives</h2>

This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket. We will Configure roles like "Supreme Admin," departments such as "System Administrators," and teams like "Level I Support" and "Level II Support" in the admin panel. We will also enable ticket creation by adjusting user settings and add agents like Howard and Dno. Last, we will set up users like Justin and Chris, define SLAs, and categorize issues with help topics, ensuring efficient management in your system.

<h2>Configuration Steps</h2>

First, we will create a role called "Supreme Admin" which will give people who have this role access to create tickets and delete tickets, pretty much everything. We will start by making sure we are on the Admin Panel, click the Agents tab and then roles. Here we can add our new "Supreme Admin" role and also edit the permissions we can enable or disable .

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/900efdc6-3f39-4c76-b696-2e8bb5f2a76a)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/bc3c1748-3287-41c9-a391-e1f16352a0c0)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/8d1da753-cf91-4a4d-a731-e5acd8106be9)

Next, we will configure some departments. We start by making sure we are in the Admins Panel, click the Agents tab, select Departments, click the add new department tab, and name the deparetment "System Administrator".  

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/0e6a2b6c-a945-40b6-a006-9749e2679010)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/633e354c-c382-496e-8a3d-f7fc678476d6)

We will now create our Teams by adding a Level II Support Team to go along our default Level I Support Team. Teams allow you to pull Agents from different Departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter. 

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/52de39a1-4b67-4bff-aa23-828da558ff4c)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/b269e8f2-e57e-41a7-8459-44bc795f2cd0)

Now we will begin configuring our Agents (Workers). First, make sure you are still on the Admin Panel, click the "Agents" tab, and then add a couple of new Agents. 

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/e74de13e-1e07-4fb4-9a0a-b052563734c0)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/b8b70468-bf57-4c88-bb0d-045e7ab9b2a5)

Next, we will configure the users (Customers) by switching to the Agent Panel, click the Users tab and then click the add user tab. 

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/35053b20-f786-463a-a5f0-b861d0f6aa76)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/30bbd0f2-7ad3-4db0-93a9-db2021f4f115)

After you created 2 new Users, we will congigure our SLAs. We will first head back over to our Admin Panel, Click the Manage Tab, and then select SLA and then select "Add New SLA Plan" to edit. We will create 3 SLAs for the purpose of this lab, SEV-A, SEV-B, and SEV-C. We will also give each SLA a different grace period and scheudle.  

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/76dedf6c-b682-4335-9f87-0e5f3b616c56)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/5412ba26-f7b7-4c94-85aa-9b2569fbb73c)

The last thing we will do in this section of the lab is configure our help topics which will help streamline the end-user's help desk experience to ensure proper assignment and prompt response to the ticket. After making sure we are in the Admin Panel, click Manage and select Help Topics. We will add 4 new Help Topics: Business Critical Outage, Personal Computer Issues, Equipment Request, and Password Reset. 

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/1f7942e9-8871-44a6-83fc-d188dfa9c681)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/f2e76c48-c0dc-4f48-b962-179d99080e46)


<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

In this last section of the osTicketing Lab, we will begin by opening up a web brower using the End User osTicket URL http://localhost/osTicket/ we will be acting like we are end users creating a few tickets so we can solve them ourselves as the help desk professional. 

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/85e1d40c-89be-4f93-bd77-5ac6269fa348)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/5e86db10-e1c9-46e7-b6d6-7d55810a81ea)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/5d83c600-39f0-4b1f-8861-463c418f5a51)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/0e24c8fa-34cb-49d3-8d6e-8879854ee18d)

Next we will login into osTicket as help desk professional (Agent) Howard.Williams. Once we log onto the Agent profile Howard, we shouold be able to see the tickets we created. We will then start with the most urgent ticket which is the entire mobile online banking being down. 

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/874acabd-b4ef-462a-9962-bebc57384c38)

We will now change the priority level of the tickets to the proper priority level, department, SLA Plan and agent we will assign the tickets to. 

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/8099159c-562d-4d17-8583-3258dc12046c)

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/31c7db8f-be84-47b4-bab6-c2e3568954df)

The final step of this lab is to resolve issues and close out the tickets which can be seen here.

![image](https://github.com/Tstewart2408/osticket-prereqs/assets/158493074/5055cd73-7605-4a9d-adc2-f9202467a52c)













