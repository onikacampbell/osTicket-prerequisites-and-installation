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

<p align="center">
  <img src="https://github.com/user-attachments/assets/c42984dc-892f-4bd0-85be-0b42ecee28c8" width="80%" alt="Windows 11 Virtual Machine in Microsoft Azure"/>
</p>

<p align="center">
<b>Figure 1.</b> Windows 11 virtual machine created in Microsoft Azure for the osTicket installation lab.
</p>

<p>
A Windows 11 virtual machine was created in Microsoft Azure to host the osTicket help desk application. This virtual machine serves as the environment where all installation and configuration tasks are completed.
</p>

<h3>Step 2 - Install Internet Information Services (IIS)</h3>

<p align="center">
  <img src="https://github.com/user-attachments/assets/39b2e647-95ca-4a1c-b99d-811491905b1c" width="80%" alt="Windows Features - IIS"/>
  </p>

<p align="center">
<b>Figure 2.</b> Internet Information Services (IIS) enabled through the Windows Features menu.
</p>

<p>
Internet Information Services (IIS) was enabled by selecting the required web server features from the Windows Features dialog. IIS provides the web server environment required to host the osTicket application.
</p>

<br>

<p align="center">
  <img src="https://github.com/user-attachments/assets/648cb690-9ef6-4bfe-b257-3a66e93f4cea" width="80%" alt="IIS Manager"/>
</p>

<p align="center">
<b>Figure 3.</b> IIS Manager displaying the Features View after the successful installation of Internet Information Services (IIS).
</p>

<p>
IIS Manager was opened to verify that the web server was installed correctly and to access the management console used for configuring websites, application pools, and server features throughout the osTicket installation.
</p>

<br>

<p align="center">
  <img src="https://github.com/user-attachments/assets/104819d5-5ae3-4fb9-8757-5fa22f6675a6" width="80%" alt="Default IIS Website"/>
</p>

<p align="center">
<b>Figure 4.</b> Default IIS welcome page displayed by browsing to <code>http://localhost</code>.
</p>

<p>
The default IIS landing page was successfully displayed, confirming that the web server was operational and able to serve web content before continuing with the remaining osTicket installation steps.
</p>

<h3>Step 3 - Install PHP Manager and IIS URL Rewrite Module</h3>

<p align="center">
  <img src="https://github.com/user-attachments/assets/02559a65-c713-44b2-9b5e-2775a520918b" width="80%" alt="PHP Manager Installation"/>
</p>

<p align="center">
<b>Figure 5.</b> PHP Manager for IIS successfully installed.
</p>

<p>
PHP Manager for IIS was installed to simplify the configuration and management of PHP within Internet Information Services (IIS). This tool provides an interface for registering PHP and managing PHP settings required by the osTicket application.
</p>

<br>

<p align="center">
  <img src="https://github.com/user-attachments/assets/9cc3c823-5e1e-4ae2-99bd-396bf591d476" width="80%" alt="IIS URL Rewrite Module"/>
</p>

<p align="center">
<b>Figure 6.</b> IIS URL Rewrite Module setup.
</p>

<p>
The IIS URL Rewrite Module was installed to enable URL rewriting functionality required by osTicket. This component allows IIS to process and rewrite incoming URL requests before they are handled by the web application.
</p>

<br>

<p align="center">
  <img src="https://github.com/user-attachments/assets/fb1fb21e-025c-4acb-9fbd-2ea804853023" width="80%" alt="PHP Manager and URL Rewrite in IIS"/>
</p>

<p align="center">
<b>Figure 7.</b> IIS Manager displaying the PHP Manager and URL Rewrite modules after installation.
</p>

<p>
After both components were installed, IIS Manager was opened to verify that the PHP Manager and URL Rewrite modules were successfully added and available for configuring the osTicket web application.
</p>

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
