# osticket-prereq<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket in a virtual machine.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Clean VM Windows 10 work space for testing purposes
- Download and have available this folder of needed software: https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD
  
<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/QMWUBCl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Search the start menu and open Controll Pannel
</p>
<br />

<p>
<img src="https://i.imgur.com/ZmMDOXz.png" height="80%" width="80%" "/>
</p>
<p>
Open "Uninstall a program"
</p>
<br />

<p>
<img src="https://i.imgur.com/Qnl5uBk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open "Turn Windows Features On or Off"
</p>
<br />

<p>
<img src="https://i.imgur.com/AwNn5ya.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enable "Internet Information Services"
</p>
<br />
<p>
<img src="https://i.imgur.com/DySt2Qr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Expand World Wide Web Services
</p>
<br />

<p>
<img src="https://i.imgur.com/qc6Gkct.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Expand Application Development Features and Enable "CGI". Click okay and wait for Web services download to complete. 

  You can close the page once completed
</p>
<br />
<p>
<img src="https://i.imgur.com/7w9PIdN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Time to check everything is working correctly. Open a new web browser and navigate to "127.0.0.1" your webpage should look like above!
</p>
<br />

<p>
<img src="https://i.imgur.com/6ajAOdq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download PHP Manager from File link
</p>
<br />
<p>
<img src="https://i.imgur.com/Uu6NW3z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install "rewrite_amd64_en-US"
</p>
<br />

<p>
<img src="https://i.imgur.com/SXOdZdS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate to the C drive and create a folder labled "PHP"
</p>
<br />
<p>
<img src="https://i.imgur.com/sGW4dj9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open the Download folder and extract "php-7.3.8-nts-Win32-VC15-x86" into the PHP folder you just created on the C-drive
</p>
<br />
<p>
<img src="https://i.imgur.com/QnmGDSi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the Download folder install "VC_redist.x86"
</p>
<p>
<img src="https://i.imgur.com/54EFiq5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder, install MySQL 5.5.62 (mysql-5.5.62-win32.msi)

  Typical Setup ->
Launch Configuration Wizard (after install) ->
Standard Configuration ->
Username: root
Password: root
</p>
<br />
<p>
<img src="https://i.imgur.com/NceNH2S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the search bar, search for IIS, and run as an Admin.
</p>
<br />

<p>
<img src="https://i.imgur.com/NdTwSeO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From IIS open "PHP Manager"
<p>
<img src="https://i.imgur.com/E2QBxta.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open "Register new PHP Version", Click on the 3 dots, Navigate to the C drive and open the PHP Folder we made earlier, and select the "php-cgi" application
</p>
<br />

<p>
<img src="https://i.imgur.com/Y4WFk1d.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click back to the Home page on the left side on the window under connections, and restart IIS on the right side under actions
</p>
<br />
<p>
<img src="https://i.imgur.com/YYkyUqX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go back to the downloads folder and extract "osTicket-v1.15.8" (the same folder is fine)
</p>
<br />

<p>
<img src="https://i.imgur.com/7by6shE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open a new File explorer and Copy the "upload" File into - c:\inetpub\wwwroot 
</p>
<br />
<p>
<img src="https://i.imgur.com/MmimiuZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Rename the "upload" folder you just moved over to "osTicket"
</p>
<p>
<img src="https://i.imgur.com/Y4WFk1d.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go back to the IIS window and restart IIS on the right side under actions
</p>
<br />
<p>
<br /><p>
<img src="https://i.imgur.com/7by6shE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><p>
<img src="https://i.imgur.com/7by6shE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><p>
<img src="https://i.imgur.com/7by6shE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><p>
<img src="https://i.imgur.com/7by6shE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><p>
<img src="https://i.imgur.com/7by6shE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
