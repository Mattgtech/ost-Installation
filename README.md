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
](https://drive.google.com/file/d/1_OWh9p7VQLcrB0q_V7qT8yHl0xo5gv7z/view?usp=share_link)
<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<b>Step 1:<b/> Once the VM(Virtual machine) Is created then the user must make a copy of the IP address and connected it through Mircosfot remote desktop or any app the allows to do so whcih for me was "RD client". Then once you connect to virtual machine, it is yo go to control panel and open Programs. Within the program you need enable IIS, World Wide Web Services and CGI. This step is important because these programs that we enabled allows us to install PHP Files. Therefore, PHP is needed for the osTicketing system to run properly.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<b>Step 2:<b/> Install the Installations files which are "PHP Manger for IIS"(https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=share_link) and Rewrite Module <a href="https://drive.google.com/file/d/1tIK9GZBKj1JyUP87eewxgdNqn9pZmVmY/view?usp=share_link" </a>. After Installing these files, the next step is to create a folder called "PHP" in "windowsc:" so that we can install PHP 7.3.8
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The last part of the this Project requires admin setup, as well as the MSQL account setup. This is done within the php manger which is where all the installtions files were stored to and the reason being is because that's the only way to setup our ticketing system.
</p>
<br />
