<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable Internet Infornation Service (IIS).
- Install Web Platform Installer.
- Install PHP.
- Install IIS URL Rewrite module 2.
- Install MySQL.
- Install C++ redistribution.
- Configure permissions and install OS Ticket.
- Install HeidiSQL to store the tickets in the database.

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/zNwGCWM.png" height="80%" width="80%" alt="Enabling and Installing IIS"/>
</p>
<p>
Enable ISS and install Web Platformer Installer.
</p>
<br />

<p>
<img src="https://i.imgur.com/uV1bc83.png" height="40%" width="40%" alt="Pick typical"/>
<img src="https://i.imgur.com/q1B7Wdt.png" height="40%" width="40%" alt="Pick standard"/>
</p>
<p>
When installing MySQL, pick typical and standard configuration.
</p>
<br />

<p>
<img src="https://i.imgur.com/QJcuh2H.png" height="80%" width="80%" alt="Pick the file"/>
</p>
<p>
Pick the “php-cgi” file. Copy the "upload" file and paste it to c:\inetpub\wwwroot. Then rename "upload" to "osTicket." 
Restart the IIS.
</p>
<br />

<p>
<img src="https://i.imgur.com/b1K2huF.png" height="80%" width="80%" alt="Pick the file"/>
</p>
<p>
On the right, click “Browse *:80”
</p>
<br />

<p>
<img src="https://i.imgur.com/tliVLmG.png" height="80%" width="80%" alt="Pick the file"/>
</p>
<p>
Go back to IIS and go to:sites, then Default, and then osTicket. Double-click PHP Manager. Click “Enable or disable an extension.”
Select and enable: php_imap.dll, php_intl.dll, php_opcache.dll. Refresh the osTicket site in your browse, observe the changes
</p>
<br />

<p>
<img src="https://i.imgur.com/wEPm87q.png" height="30%" width="30%" alt="Pick typical"/>
<img src="https://i.imgur.com/wCdXoF5.png" height="30%" width="30%" alt="Pick standard"/>
<img src="https://i.imgur.com/WHFKXzc.png" height="30%" width="30%" alt="Pick standard"/>
</p>
<p>
Rename "C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php" to "C:\inetpub\wwwroot\osTicket\include\ost-config.php" Change its
permissions by disabling ihheritance for all. then add everyone to all.
</p>
<br />

<p>
<img src="https://i.imgur.com/aQeBuIK.png" height="80%" width="80%" alt="Pick the file"/>
</p>
<p>
Go back to IIS and go to:sites, then Default, and then osTicket. Double-click PHP Manager. Click “Enable or disable an extension.”
Select and enable: php_imap.dll, php_intl.dll, php_opcache.dll. Refresh the osTicket site in your browse, observe the changes
</p>
<br />
