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

<br />

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

<br />

<p align="center">
  <img src="https://github.com/user-attachments/assets/648cb690-9ef6-4bfe-b257-3a66e93f4cea" width="80%" alt="IIS Manager"/>
</p>

<p align="center">
<b>Figure 3.</b> IIS Manager displaying the Features View after the successful installation of Internet Information Services (IIS).
</p>

<p>
IIS Manager was opened to verify that the web server was installed correctly and to access the management console used for configuring websites, application pools, and server features throughout the osTicket installation.
</p>

<br />

<p align="center">
  <img src="https://github.com/user-attachments/assets/104819d5-5ae3-4fb9-8757-5fa22f6675a6" width="80%" alt="Default IIS Website"/>
</p>

<p align="center">
<b>Figure 4.</b> Default IIS welcome page displayed by browsing to <code>http://localhost</code>.
</p>

<p>
The default IIS landing page was successfully displayed, confirming that the web server was operational and able to serve web content before continuing with the remaining osTicket installation steps.
</p>

<br />

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

<br />

<p align="center">
  <img src="https://github.com/user-attachments/assets/9cc3c823-5e1e-4ae2-99bd-396bf591d476" width="80%" alt="IIS URL Rewrite Module"/>
</p>

<p align="center">
<b>Figure 6.</b> IIS URL Rewrite Module setup.
</p>

<p>
The IIS URL Rewrite Module was installed to enable URL rewriting functionality required by osTicket. This component allows IIS to process and rewrite incoming URL requests before they are handled by the web application.
</p>

<br />

<p align="center">
  <img src="https://github.com/user-attachments/assets/fb1fb21e-025c-4acb-9fbd-2ea804853023" width="80%" alt="PHP Manager and URL Rewrite in IIS"/>
</p>

<p align="center">
<b>Figure 7.</b> IIS Manager displaying the PHP Manager and URL Rewrite modules after installation.
</p>

<p>
After both components were installed, IIS Manager was opened to verify that the PHP Manager and URL Rewrite modules were successfully added and available for configuring the osTicket web application.
</p>

<br />

<h3>Step 4 - Install PHP</h3>

<p align="center">
  <img src="https://github.com/user-attachments/assets/835b758a-769a-4e2c-8144-dfdc20d60669" width="80%" alt="PHP Installation Folder"/>
</p>

<p align="center">
<b>Figure 8.</b> PHP extracted to the <code>C:\PHP</code> directory.
</p>

<p>
The PHP package was extracted to the <code>C:\PHP</code> directory, where the PHP executable files were stored for use by Internet Information Services (IIS).
</p>

<br />

<p align="center">
  <img src="https://github.com/user-attachments/assets/0954d452-81e3-46b3-bad7-cba06280eeb6" width="80%" alt="FastCGI Settings"/>
</p>

<p align="center">
<b>Figure 9.</b> FastCGI configured to use the PHP executable.
</p>

<p>
FastCGI Settings were configured to register <code>C:\PHP\php-cgi.exe</code>, enabling IIS to process PHP requests for the osTicket application.
</p>

<br />

<p align="center">
  <img src="https://github.com/user-attachments/assets/3fb500ab-b105-4b3d-9bd7-9e4d318bfde9" width="80%" alt="PHP Manager"/>
</p>

<p align="center">
<b>Figure 10.</b> PHP Manager confirming the successful PHP configuration.
</p>

<p>
PHP Manager was used to verify that PHP was successfully registered with IIS and that the required PHP configuration files and extensions were available before proceeding with the remaining osTicket installation.
</p>

<br />

<h3>Step 5 - Install Microsoft Visual C++ Redistributable</h3>

<p align="center">
  <img src="https://github.com/user-attachments/assets/32ec1522-343b-46b8-b8d2-18391358c7da" width="80%" alt="Microsoft Visual C++ Redistributable"/>
</p>

<p align="center">
<b>Figure 11.</b> Microsoft Visual C++ 2015–2022 Redistributable (x86) installed successfully.
</p>

<p>
The Microsoft Visual C++ 2015–2022 Redistributable (x86) was installed to provide the runtime libraries required by PHP. This dependency ensures that PHP and the osTicket application can run properly within the IIS web server environment.
</p>

<br />

<h3>Step 6 - Install MySQL Server</h3>

<p align="center">
  <img src="https://github.com/user-attachments/assets/da124d64-8906-4da7-be2c-c5fcb402b709" width="80%" alt="MySQL Server Installer"/>
</p>

<p align="center">
<b>Figure 12.</b> MySQL Server 5.5 installation package used during the osTicket installation.
</p>

<p>
The MySQL Server 5.5 installation package was launched from the osTicket installation files to install the database server required by osTicket. During the installation, a root administrator account was configured to manage the MySQL database used by the osTicket application.
</p>

<br />

<h3>Step 7 - Install HeidiSQL</h3>

<p align="center">
  <img src="https://github.com/user-attachments/assets/4327d7d6-52e6-4983-a6f9-fb5d511aee5e" width="80%" alt="HeidiSQL Installer"/>
</p>

<p align="center">
<b>Figure 13.</b> HeidiSQL installation package used during the osTicket installation.
</p>

<p>
The HeidiSQL installation package was launched from the osTicket installation files. HeidiSQL provides a graphical interface for connecting to and managing the MySQL database server used by the osTicket application.
</p>

<br />

<p align="center">
  <img src="https://github.com/user-attachments/assets/bb47d391-172f-4648-9487-9e9eb6acd3b5" width="80%" alt="HeidiSQL Connected to MySQL"/>
</p>

<p align="center">
<b>Figure 14.</b> HeidiSQL successfully connected to the local MySQL server and displaying the osTicket database.
</p>

<p>
After connecting successfully, HeidiSQL displayed the <code>osticket</code> database and its tables, confirming that the MySQL server was functioning correctly and ready for the osTicket application.
</p>

<br />

<h3>Step 8 - Install osTicket</h3>

<p align="center">
  <img src="https://github.com/user-attachments/assets/925d7547-9b7e-4542-be9f-00f732081f5a" width="80%" alt="osTicket Installation Files"/>
</p>

<p align="center">
<b>Figure 15.</b> osTicket installation package prepared for deployment.
</p>

<p>
The osTicket installation package was extracted from the installation files and prepared for deployment to the IIS web root directory so that the application could be hosted by Internet Information Services (IIS).
</p>

<br />

<p align="center">
  <img src="https://github.com/user-attachments/assets/03bd3b1d-3639-4e1c-b446-676efcdc58b5" width="80%" alt="osTicket Installer"/>
</p>

<p align="center">
<b>Figure 16.</b> osTicket installer confirming a successful installation.
</p>

<p>
Accessing the osTicket installer displayed a message indicating that the application was already installed, confirming that the deployment had completed successfully and that the configuration files were in place.
</p>

<br />

<p align="center">
  <img src="https://github.com/user-attachments/assets/8ba584da-42c7-476e-8b67-1198354bb5b7" width="80%" alt="osTicket Agent Login"/>
</p>

<p align="center">
<b>Figure 17.</b> osTicket Agent Login page.
</p>

<p>
The Agent Login page was successfully displayed, confirming that the web application was accessible through IIS and ready to authenticate users.
</p>

<br />

<p align="center">
  <img src="https://github.com/user-attachments/assets/cd6dfe68-8e07-4cec-9cfe-9c32048bf636" width="80%" alt="osTicket Administrator Panel"/>
</p>

<p align="center">
<b>Figure 18.</b> osTicket Administrator Panel after a successful login.
</p>

<p>
After signing in with the administrator account, the osTicket dashboard loaded successfully, confirming that IIS, PHP, MySQL, and osTicket were configured correctly and that the help desk environment was ready for post-installation configuration.
</p>

<br />

<h2>Installation Complete</h2>

<p>
The osTicket application was successfully deployed on a Windows 11 virtual machine hosted in Microsoft Azure using IIS, PHP, MySQL, and HeidiSQL. The environment is now fully configured and ready for post-installation tasks, including creating agents, departments, teams, SLA plans, help topics, and configuring the help desk workflow.
</p>
