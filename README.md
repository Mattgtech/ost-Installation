<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>osTicket Prerequisites</h2>

- Enable IIS w/CGI
- PHP Manager for IIS 
- Rewrite Module
- PHP 7.3.8 
- VC_redist.x86.exe
- Install osTicket
</h2>

<p>
<img src="https://i.imgur.com/X1GnsIE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <b>Step 1:</b> Once the VM(Virtual machine) Is created then the user must make a copy of the IP address and connected it through Mircosfot remote desktop or any app the allows to do so whcih for me was "RD client". Then once you connect to virtual machine, it is yo go to control panel & open "Programs and Features". Within the "Programs and Features" you need enable IIS, World Wide Web Services and CGI. This step is important because these programs that we enabled allows us to install PHP Files. Therefore, PHP is needed for the osTicketing system to run properly.
</p>
<br />

<p>
<img src="https://i.imgur.com/D50OZAk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <b>Step 2:</b> Install the Installations files which are <a href = "https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=share_link">PHP Manager for IIS</a> and <a href = "https://drive.google.com/file/d/1tIK9GZBKj1JyUP87eewxgdNqn9pZmVmY/view?usp=share_link">Rewrite Module</a>. After Installing these files, the next step is to create a folder called "PHP" in the directory C:\" so that we can install <a href = "https://drive.google.com/file/d/1snNMtLdCOpMtkCyD4mvl9yOOmvVIp9fP/view?usp=share_link">PHP 7.3.8</a> which contains the content that is needed to download osticket. Moreover, the last file that we are installing is <a href ="https://drive.google.com/file/d/1s1OsGF3-ioO0_9LYizPRiVuIkb3lFJgH/view?usp=share_link">VC_redist.x86.exe</a> which is also known as Mircosoft Visual c++.
</p>
<br />
  
<p>
<img src="https://i.imgur.com/EwUev1a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <b>Step 3:</b> Download and install <a href = "https://drive.google.com/file/d/1_OWh9p7VQLcrB0q_V7qT8yHl0xo5gv7z/view?usp=share_link">MySQL 5.5.62</a>. Once that's done installing open the file and click on "Typicla Setup", "Launuch Configuration Wizard"(After Install), "Standard Configuration" and the password for the Username is Password1. After completing this then you need open IIS as a admin and register PHP from within IIS. Next, Reload IIS (Open IIS, Stop and Start the server) in order to go to next step which is opening osTicket by going to sites-> Default -> osTicket"Browse *:80"  

</p>
<br />

<p>
<img src="https://i.imgur.com/c6NuQBo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <b>Step 4:</b> Go back to IIS, sites -> Default -> osTicket. Then double-click PHP ManagerClick and “Enable or disable an extension”. We need to enable php_imap.dll, php_intl.dll and php_opcache.dll. Once you do that then refresh the osTicket site in your browse and notice the changes.

</p>
<br />

<p>
<img src="https://i.imgur.com/aWtz0QA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <b>Step 5:</b> Rename ost-config.php by going to C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php. The new name for ost-sampleconfig.php should now be ost-config.php. Then assign Permissions through ost-config.php properties and disable inheritance -> remove All new Permissions -> everyone -> all. Next we will continue to setup osticket by entering our information like our helpdesk name, email, username and most importantly MySQL Database.

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The last part of the this Project requires admin setup, as well as the MSQL account setup. This is done within the php manger which is where all the installtions files were stored to and the reason being is because that's the only way to setup our ticketing system.
</p>
<br />
