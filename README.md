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

- Enable IIS
- Install web platform installer
- Install MySQL/setup username and PW
- Install c++ redistributable
- Configure permissions and install osTicket

<h2>Installation Steps</h2>

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/c11b01a0-3766-46b5-b639-1c98d8f79c40)

</p>
<p>
Open control panel > Programs > Turn Windows features on or off. Turn "Internet Information Services" On. Expand "Internet Information Services" and make sure "Web Management Tools" and World Wide Web Services" and checked. Expand "World Wide Web Services" > "Application Developmrnt Features" and check "CGI".
  From "World Wide Web Services" > "Common HTTP Features", make sure everything is checked on.
</p>
<br />

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/2f34c31c-197f-40e3-b7f9-1329f568d3ab)

</p>
<p>
Open a web browser and go to "127.0.0.1" to ensure the change was made correctly
</p>
<br />

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/49e7df93-836d-4fb7-a268-efa5a2ddf5b6)

</p>
<p>
Next Install PHP Manager
</p>
<br />
