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

- Azure Virtual Machine (VM)
- Remote Access
- Required Software & Dependencies
  - Internet Information Services (IIS) with CGI
  - PHP 7.3.8 (with required extensions)
  - MySQL 5.5.62
- File Downloads
  - osTicket Installation Package
  - IIS Rewrite Module
  - PHP Manager for IIS

<h2>Installation Steps</h2>
<h3>Deploy a Windows 10 Virtual Machine</h3>

<p>
Create a Windows 10 VM in Azure with 4 vCPUs and enable RDP access. This VM will host the osTicket system.
</p>
<p>
<img src="https://i.imgur.com/lcXtcZK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h3>Install IIS, PHP, MySQL</h3>

<p>
- Enable IIS (Internet Information Services) with CGI
- Install PHP 7.3.8 and enable required extensions (php_imap.dll, php_intl.dll, php_opcache.dll)
- Install MySQL 5.5.62, creating a database for osTicket
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h3>Download and Configure osTicket</h3>

<p>
- Extract osTicket installation files and move them 
- Rename the upload folder to osTicket.
- Register PHP in IIS and restart the web server.
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h3>Set Up osTicket in the Browser and Final Configuration</h3>

<p>
- Open osTicket setup page in a web browser.
- Configure database settings (MySQL root credentials).
- Complete initial helpdesk configuration (name, default email, admin login).
- Rename ost-sampleconfig.php to ost-config.php and adjust file permissions.
- Delete the setup directory for security.
- Set ost-config.php to read-only to prevent unauthorized changes.
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
