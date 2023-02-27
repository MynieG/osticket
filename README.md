# osticket-prereqs
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

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/CAu12fb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a Windows 10 Virtual Machine (VM) with 2-4 Virtual CPUs.

</p>
<br />

<p>
<img src="https://i.imgur.com/dB4EnNp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 Use Remote Desktop to remotely connnect to the Virtual Machine. Use the Public IP address from the Virtual Machine.
</p>
<br />

<p>
<img src="https://i.imgur.com/l4JQgVm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi) and Download and install Rewrite Module (rewrite_amd64_en-US.msi)
</p>
<br />


<p>
<img src="https://i.imgur.com/Px9qr1n.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>



<p>
<img src="https://i.imgur.com/hnww6PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create the directory C:\PHP.
</p>
<br />



<p>
<img src="https://i.imgur.com/0rKoHCq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) and unzip the contents into C:\PHP
</p>
<br />


<p>
<img src="https://i.imgur.com/55vLgYA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install VC_redist.x86.exe.
</p>
<br />



<p>
<img src="https://i.imgur.com/mcTqzKV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
Typical Setup ->
Launch Configuration Wizard (after install) ->
Standard Configuration ->
Create Password

.
</p>
<br />

<p>
<img src="https://i.imgur.com/EnBP2nc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS as an Admin

Register PHP from within IIS

Reload IIS (Open IIS, Stop and Start the server)

</p>
<br />

<p>
<img src="https://i.imgur.com/Wb8TXVB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<p>
<img src="https://i.imgur.com/3WQKBCM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
Download osTicket from the Installation Files Folder
Extract and copy “upload” folder to c:\inetpub\wwwroot
Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”

</p>
<br />



<p>
<img src="https://i.imgur.com/0YS9jAw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to sites -> Default -> osTicket
On the right, click “Browse *:80”
</p>
<br />




<p>
<img src="https://i.imgur.com/e3CHvdR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go back to IIS, sites -> Default -> osTicket
Double-click PHP Manager
Click “Enable or disable an extension”
Enable: php_imap.dll
Enable: php_intl.dll
Enable: php_opcache.dll
Refresh the osTicket site in your browse, observe the changes
</p>
<br />

<p>
<img src="http://i.imgur.com/rzsjq5B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>




<p>
<img src=https://i.imgur.com/h0PUl8q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Continue Setting up osTicket in the browser (click Continue)
Name Helpdesk
Default email (receives email from customers)

</p>
<br />



<p>
<img src="https://i.imgur.com/bzIhmtx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install HeidiSQL.
Create a new session, root/
Connect to the session
Create a database called “osTicket
</p>
<br />


<p>
<img src="https://i.imgur.com/fmQFim1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open Heidi SQL
Create a new session, root/Password1.Connect to the session.Create a database called “osTicket”
</p>
<br /> 



<p>
<img src="https://i.imgur.com/rZspk3u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
MySQL Database: osTicket
Enter-Username: root
Enter+ Password
Click “Install Now!”


</p>
<br />



<p>
<img src="https://i.imgur.com/x7hl3m3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Congratulations, 
Browse to your help desk login page: http://localhost/osTicket/scp/login.php

Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
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
