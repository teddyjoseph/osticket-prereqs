<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />
Outlining the necessary software, download steps, and initial installation to get osTicket up and running.

<h2>🖥️Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- Windows 10</b> (21H2)
<h2>⚙️Getting Started </h2>

<h2>List of Prerequisites</h2>

- Web Server: Apache, Nginx or Iss
- PHP: Version 8.1 - 8.2 (8.2 recommended)
- MySQL: Version 5.0 or higher
- MySQL Database: A database with a valid user, password, and hostname
- MySQL User Privileges: The MySQL user must have full privileges on the database
- osTicket Download: [osTicket Official Site](https://osticket.com/download)


<h2>Installation Steps</h2>

![Screenshot 2024-10-20 105725](https://github.com/user-attachments/assets/c4f9a76d-52e1-4d04-b50e-5ebc8f504813)




Create a Virtual Machine: Go to the Azure portal and create a new VM.
Choose a Windows Server image and configure the VM with the necessary resources (CPU, RAM, etc.).
</p>
<br />

![Screenshot 2024-10-22 195622](https://github.com/user-attachments/assets/f6cf0118-e955-440b-9259-a41a0e1452d5)

Connect to the VM: Use Remote Desktop to connect to your newly created VM.
Install Internet Information Services (IIS): Open the Server Manager and install the Web Server (IIS) role.
Enable CGI and Common HTTP Features, and IIS Management Console.
</p>
<br />

![Capture](https://github.com/user-attachments/assets/ff8aa4f4-423c-4439-8362-b762505e712a)

Install PHP: Download and install PHP Manager for IIS. Download and install PHP (e.g., PHP 7.3.8) and place it in C:\PHP.
Install VC Redist (Visual C++ Redistributable) if required.
Install MySQL: Download and install MySQL Server.
Set a root password for MySQL during installation.
</p>
<br />

![Capture2](https://github.com/user-attachments/assets/01318426-8966-4b89-93bf-a972829bd5d4)

Download osTicket: Download the osTicket files and extract them to your web server's root directory.
Configure database credentials in the include/ost-config.php file.
</p>
<br />

![Capture3](https://github.com/user-attachments/assets/c220d934-584b-46d6-b631-74bbff33211b)

Run the osTicket installer by navigating to http://your-server/osticket/.Follow the on-screen instructions to complete the installation, 
configuring settings such as email, help topics, and user permissions
<br />
