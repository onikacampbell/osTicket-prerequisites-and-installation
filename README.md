<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket Logo"/>
</p>

<h1>osTicket - Prerequisites & Installation</h1>

This project walks through the installation and initial setup of the open-source help desk ticketing system <b>osTicket</b> in a Windows virtual machine hosted in Microsoft Azure.

<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
- Windows 11
- Remote Desktop (RDP)
- Internet Information Services (IIS)
- PHP Manager
- MySQL
- HeidiSQL
- osTicket

<h2>Operating System Used</h2>

- Windows 11 Pro

<h2>Prerequisites</h2>

- Microsoft Azure account
- Windows 11 Virtual Machine
- Remote Desktop Connection
- osTicket installation files
- Web browser
- Internet connection

<h2>Installation Steps</h2>

<h3>Step 1 - Create a Windows 11 Virtual Machine</h3>

<p>
<img src="<img width="1801" height="286" alt="image" src="https://github.com/user-attachments/assets/c42984dc-892f-4bd0-85be-0b42ecee28c8" />
" width="80%" alt="Azure Virtual Machine"/>
</p>

<p>
Create a Windows 11 virtual machine in Microsoft Azure and connect to it using Remote Desktop.
</p>

<br />

<h3>Step 2 - Install Internet Information Services (IIS)</h3>

<p>
<img src="YOUR-SCREENSHOT-HERE" width="80%" alt="Install IIS"/>
</p>

<p>
Enable Internet Information Services (IIS) and the required web server features.
</p>

<br />

<h3>Step 3 - Install PHP Manager and IIS Rewrite Module</h3>

<p>
<img src="YOUR-SCREENSHOT-HERE" width="80%" alt="PHP Manager"/>
</p>

<p>
Install PHP Manager and the IIS Rewrite Module required by osTicket.
</p>

<br />

<h3>Step 4 - Install PHP</h3>

<p>
<img src="YOUR-SCREENSHOT-HERE" width="80%" alt="Install PHP"/>
</p>

<p>
Extract PHP to the correct directory and register it with IIS.
</p>

<br />

<h3>Step 5 - Install Microsoft Visual C++ Redistributable</h3>

<p>
<img src="YOUR-SCREENSHOT-HERE" width="80%" alt="Visual C++ Redistributable"/>
</p>

<p>
Install the Microsoft Visual C++ Redistributable required by PHP.
</p>

<br />

<h3>Step 6 - Install MySQL</h3>

<p>
<img src="YOUR-SCREENSHOT-HERE" width="80%" alt="MySQL Installation"/>
</p>

<p>
Install MySQL Server and configure the root account.
</p>

<br />

<h3>Step 7 - Install HeidiSQL</h3>

<p>
<img src="YOUR-SCREENSHOT-HERE" width="80%" alt="HeidiSQL"/>
</p>

<p>
Install HeidiSQL and verify the MySQL connection.
</p>

<br />

<h3>Step 8 - Install osTicket</h3>

<p>
<img src="YOUR-SCREENSHOT-HERE" width="80%" alt="osTicket Installation"/>
</p>

<p>
Copy the osTicket files into the IIS web directory and complete the installation wizard.
</p>

<br />

<h2>Final Result</h2>

<p>
<img src="YOUR-SCREENSHOT-HERE" width="80%" alt="osTicket Installed"/>
</p>

<p>
osTicket has been successfully installed and is ready for post-installation configuration.
</p>
