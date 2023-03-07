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

<h2>Operating Systems Used</h2>

- Windows 10 (21H2)

<h2>List of Prerequisites</h2>

- Install/Enable IIS in Windows w/CGI
- Install PHP Manager for IIS
- Install the Rewrite Module
- Create the directory C:\PHP
- Download PHP 7.3.8 and unzip the contents into C:\PHP
- Download and Install Microsoft Visual C++ Redistributable
- Download and Install MySQL 5.5.62
- IIS Configuration
- Install osTicket v1.15.8

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/iIxElH6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This process was done on a Virtual Machine I created through Microsoft Azure. In the first step, I had to enable IIS in windows. I did that by going to the control panel and opening programs; once opened, I clicked on the "turn windows features on or off" tab. Once inside, I expanded the Internet Information Service tab(IIS), then I expanded the World Wide Web Services tab and clicked on Application Development Features. Once inside the ADF tab, I checked off CGI and clicked "ok" to allow the computer to apply the changes I had made.
</p>
<br />

<p>
<img src="https://i.imgur.com/VHak5ha.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this next step I downloaded and installed PHP Manager for IIS.
</p>
<br />

<p>
<img src="https://i.imgur.com/eCPOvzj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, I had to download and install the Rewrite Module. The Rewrite Module has a unique configuration inside of it that allows specific URLs to work on osTicket. This Module is needed to allow osTicket to run and function properly.
</p>
<br />

<p>
<img src="https://i.imgur.com/df1AVy9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this next step, I had to create the directory c:\PHP. I went to the file manager, clicked the "This PC" tab, and opened the Windows(c:) drive. Once I was in the c:\ drive folder, I right-clicked on my mouse, hit the "New" tab, then hit the "Folder" tab and created the new directory for c:\PHP.
</p>
<br />

<p>
<img src="https://i.imgur.com/DbDA7LV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here I downloaded PHP 7.3.8 and then had to unzip all of the contents into the c:\PHP folder I had created in the previous step.
</p>
<br />

<p>
<img src="https://i.imgur.com/WWlNK60.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After that, I downloaded and installed Microsoft Visual C++ Redistributable. This program is needed and required by PHP. 
</p>
<br />

<p>
<img src="https://i.imgur.com/wBYCFeR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this step, I had to download and install the MySQL server. After it was installed, I had to set up credentials in order for me to use MySQL Server. Once I configured MySQL, it created a database for osTicket to store its information.
</p>
<br />

<p>
<img src="https://i.imgur.com/VEVzncQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This is the last step before finally downloading and installing osTicket. I had to do some configuration in IIS as an Admin. I did that by searching for IIS, and before clicking the tab, I had to right-click and tap "Run as Administrator." Next, I clicked on the PHP Manager folder and selected "Register new PHP version." Lastly, I browsed my PHP folder on the c: drive and selected Php-cgi.
</p>
<br />

<p>
<img src="https://i.imgur.com/VpUi1ys.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/yVlzgao.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/4ViSUYz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/IgK8Ofn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/k2ser8I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/o5SrVt6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/1HoB6xQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This was the longest and final step in the process. First, I downloaded and installed osTicket; once installed, I needed to extract and copy the "Upload" folder into the c:\inetpub\wwwroot folder. After extracting all of the data from the upload folder, I renamed the upload folder to "osTicket." Next, I had to go back inside IIS and go to the "sites" folder, then "Default Web Site," then "osTicket," and lastly clicked on the browse *:80 tab, which allowed me to bring up osTicket Installer. Then I had to go back into IIS to enable certain features to allow osTicket to work correctly. After I enabled the features, I went into the ost.config.php file and had to assign permissions to allow everyone Full Control. After completing that part, I went back into osTicket Installer to finish the setup which included creating a help desk name, Admin User and setting up the database settings. Lastly, I had to download one more program, called "HeidiSQL." This program allows me to connect to the SQL database I downloaded earlier, and once downloaded, I created a new database called "osTicket." The last thing left was to install osTicket onto the Virtual Machine I had been using throughout the entire process. 
</p>
<br />
