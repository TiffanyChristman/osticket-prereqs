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

-  IIS in Windows WITH CGI and Common HTTP Features

- PHPManagerForIIS_V1.5.0.msi)
- (rewrite_amd64_en-US.msi
- php-7.3.8-nts-Win32-VC15-x86.zip
- VC redist // MySQL

<h2>Installation Steps</h2>

<p>
  
<![Screenshot 2024-03-01 092615](https://github.com/TiffanyChristman/osticket-prereqs/assets/161388738/f9f83821-a27d-411c-bc4a-9fad18f25e5f)

</p>
<p>
Install / Enable IIS in Windows WITH
CGI and Common HTTP Features
World Wide Web Services -> Application Development Features ->
[X] CGI
[X] Common HTTP Features
AND IIS Management Console
Internet Information Services -> Web Management Tools -> IIS Management Console
	[X] IIS Management Console

</p>
<br />

<p>
  
![Screenshot 2024-03-01 092907](https://github.com/TiffanyChristman/osticket-prereqs/assets/161388738/7ae774c1-2629-418a-a757-87719754f588)

</p>
<p>
A way to check IIS is intalled correctly, is to type the IP address into the browser for confirmation!

</p>
<br />

<p>
  
![Screenshot 2024-03-01 095050](https://github.com/TiffanyChristman/osticket-prereqs/assets/161388738/78185fc5-e368-4b3e-a3de-b614082765db)
</p>
<p>
Download and install the Rewrite Module (rewrite_amd64_en-US.msi)
</p>
<br />

<p
  
![Screenshot 2024-03-01 095625](https://github.com/TiffanyChristman/osticket-prereqs/assets/161388738/14d1b85b-d277-4bb6-a8c8-358d6e72542c)
</p>
<p>
Go back to IIS, sites -> Default -> osTicket
Double-click PHP Manager
Click “Enable or disable an extension”
Enable: php_imap.dll
Enable: php_intl.dll
Enable: php_opcache.dll
</p>
<br />

<p>
  
![Screenshot 2024-03-01 095720](https://github.com/TiffanyChristman/osticket-prereqs/assets/161388738/11444eee-4052-46bc-9392-6b082ae9a845)

</p>
<p>

Refresh the osTicket site in your browse, observe the changes

</p>
<br />

<p>
  
![Screenshot 2024-03-01 095406](https://github.com/TiffanyChristman/osticket-prereqs/assets/161388738/d6575edc-26af-4f1c-a8d7-68b32ee16676)


</p>
Open Heidi SQL
Create a new session, root/Password1
Connect to the session
Create a database called “osTicket”

Continue Setting up osticket in the browser
MySQL Database: osTicket
MySQL Username: root
MySQL Password: Password1
Click “Install Now!”

<p>


</p>
<br />

<p
  
![Screenshot 2024-03-03 111838](https://github.com/TiffanyChristman/osticket-prereqs/assets/161388738/84695a28-4d0f-4afb-9b8b-09fa9288a6d6)

</p>
<p>
Install osTicket v1.15.8
Download osTicket from the Installation Files Folder
Extract and copy “upload” folder to c:\inetpub\wwwroot
Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”

 Go back to IIS, sites -> Default -> osTicket
Double-click PHP Manager
Click “Enable or disable an extension”
Enable: php_imap.dll
Enable: php_intl.dll
Enable: php_opcache.dll
Refresh the osTicket site in your browse, observe the changes

</p>
<br />







