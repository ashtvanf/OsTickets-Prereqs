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

<h2>Installation Steps</h2>

<img src="https://github.com/ashtvanf/OsTickets-Prereqs/assets/138221709/cbc74c53-5d08-4f88-aae2-2c906f9d3e5e"/>

- Download and install all programs from installation list. <https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6>
- Install/Enable IIS in Windows with CGI, Common HTTP Features, and IIS Management Console
- Create the directory C:\PHP
  
Open IIS as an Administrator and register PHP. Afterwards reload IIS and restart the server.
Once that is completed, Install osTicket v1.15.8

After installation, extract and copy “upload” folder to c:\inetpub\wwwroot.
Once finished, go within c:\inetpub\wwwroot, and rename “upload” to “osTicket.”
If not named specifically "osTicket" the installation may not complete.
</p>
<br />

<p>
<img src="https://github.com/ashtvanf/OsTickets-Prereqs/assets/138221709/a1defd86-0ca1-4b2a-a357-8a58919ccaa0"
  
</p>
<p>
Go to sites -> Default -> osTicket.
On the right, click “Browse *:80”
  
You'll notice that some extensions are not enabled.

Go back to IIS, sites -> Default -> osTicket
-Double-click PHP Manager

-Click “Enable or disable an extension”

-Enable: php_imap.dll

-Enable: php_intl.dll

-Enable: php_opcache.dll

Refresh the osTicket site in your browser, and ensure changes have been made.

Rename: ost-config.php, origin will be: "ost-sampleconfig.php"

</p>
<br />

<p>
<img src="https://github.com/ashtvanf/OsTickets-Prereqs/assets/138221709/31196919-1548-4670-a75a-5d74257d680b"

</p>
<br />
