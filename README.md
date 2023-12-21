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
Prerequisites:

- Server Setup-Ensure a web server.
- Database Preparation-Verify PHP and Composer are installed.

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/chyaFyl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 1: Azure VM Setup
Create a Resource Group.
Establish a Windows 10 VM in the Resource Group with 2-4 vCPUs.
Allow the creation of a new Virtual Network (Vnet).
<br />

<p>
<img src="https://i.imgur.com/chyaFyl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 2:
  Enable CGI and Common HTTP Features in IIS on the Windows VM.
Install IIS Management Console.
Download and install PHP Manager for IIS.
Download and install the Rewrite Module.
Set up C:\PHP and install PHP 7.3.8.
Install VC_redist.x86.exe.
Install MySQL 5.5.62 with a typical setup, choosing "Password1" as the password.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 3:
Open IIS as an Admin and register PHP.
Reload IIS (Stop and Start the server to check).
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 4:
Download osTicket and place the "upload" folder in c:\inetpub\wwwroot, renaming it to "osTicket."
Reload IIS.
Enable necessary PHP extensions in PHP Manager.
Rename ost-sampleconfig.php to ost-config.php.
Set permissions on ost-config.php.
Continue osTicket setup in the browser, specifying Helpdesk as the name and the default email for customer communication.
Download and install HeidiSQL.
In HeidiSQL, create a new session (root/Password1), connect to it, and create a database named "osTicket."
Complete osTicket setup in the browser, specifying MySQL Database as "osTicket," MySQL Username as "root," and MySQL Password as "Password1." Click "Install Now"
</p>
<br />
