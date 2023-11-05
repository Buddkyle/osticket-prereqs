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

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/1a2ab673-b1cd-464d-93c1-3de3ce5fb488)

</p>
<p>
Next Install Rewrite Module
</p>
<br />

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/d5fd8b67-68a5-405d-85a8-2522c50a574a)

</p>
<p>
Next Install PHP
</p>
<br />

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/dc87ab60-3963-41ad-956e-cb31a5f23039)

</p>
<p>
Next Install C++ Redistributable
</p>

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/d3839472-e07e-4174-b889-934800fadf58)

</p>
<p>
Next Install MySQL Server
</p>
<br />

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/54c0108c-77b2-4441-98f5-a5432be6d582)

</p>
<p>
Set up a root username and password in MySQL Server
</p>

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/da1a90eb-7601-48d8-b702-797bb9b10e82)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/522eb522-1e2c-49eb-be95-fb8c15736adf)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/5cbc4f92-225f-4cbe-a83b-21ab5e5f1524)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/a43dcbf9-4ac6-414d-8402-b7279f8d1536)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/8af9a6cc-5024-48c1-b7b9-6390fc9b84dd)


</p>
<p>
Search "IIS" and run as admin. 
  Select PHP manager. 
  Select Register new PHP version. 
  Choose "php.cgi" in the PHP folder. 
  After installation, restart the IIS server.
</p>

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/cbb272f0-72cc-4f8c-b8fb-f34768ef7348)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/53dd1578-d088-428d-997c-482dbd566b04)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/16c225cd-7afc-4c83-affb-a712da1776f0)

</p>
<p>
Download osTicket. Copy the "upload" folder and place it in C: > inetpub > wwwroot and rename it "osTicket". After this, restart the IIS server again.
</p>

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/5d8b5afd-34ea-45cf-b8f2-56bc920eb687)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/e8325821-351e-4e25-bdc3-fa3ba7990fab)

</p>
<p>
In IIS, expand "Sites" > "Default Web Site" > "osTicket" and then click "Browse *:80 (http)" on the right hand side to get to the osTicket site.
</p>

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/3af39db0-fe2e-45cd-81f5-c72188667c7d)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/a087a0cc-857a-4085-a0e6-412a3bd3156b)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/33f0b8cc-6a48-401c-801f-a9ca79c1fbcd)

</p>
<p>
Back in IIS, while under osTicket select "PHP Manager". At the bottom select "Enable or disable an extension". Enable the extensions "php.imap.dll", "php.intl.dll", "php.opcache.dll"
</p>

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/3fa3176e-5c1d-4ce4-9654-5ba37d596257)

</p>
<p>
Refresh the osTicket internet browser to ensure the extensions were enabled correctly
</p>

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/734ea414-500f-4fb6-a7b7-1593d67741ee)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/92d701e8-57d8-42ef-99e0-474b5a9eef1e)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/4036dbd2-7558-4012-8a8a-53fb171e9129)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/2bf1c24a-1513-4819-b547-077f0536157f)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/859400dd-e482-4861-b19f-1ab0c43a35a9)


</p>
<p>
In windows explorer, navigate to C: > inetpub > wwwroot > osTicket > include and rename "ost-sampleconfig.php" to "ost-config.php". Right click "ost-config.php" and select properties and then click advanced. Click on "Disable inheritance" at the bottom and then click "Remove all inherited permissions from the object". Click Add at the bottom. When the permission entry window opens click "Select a principal" and in the new window type "Everyone" in the box and click ok. In the basic permissions section, select "Full Control" and click ok.
</p>

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/b93dc6ae-301c-4daa-8d60-bdd151546ce3)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/290e4a28-c03b-443a-8e1d-7cecd6f23bed)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/23d4d26c-72bb-44f5-abab-4400e17ed5fd)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/d23bf600-97e8-4d2a-95fa-af66ce50890b)

</p>
<p>
Install HeidiSQL. Enter username and password that was created for MySQL. Create a new database in HeidiSQL called "osTicket"
</p>

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/0dd0b14e-084e-4389-8feb-f1528ec68fdb)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/33f84def-100b-4bbb-8f39-587d8195552b)

</p>
<p>
Fill out osTicket information and click install now at the bottom.
</p>

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/ca7f3183-06ab-4170-bfc2-b999477da341)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/c82a0a93-a576-4a09-b4f4-90ac0e9d7833)

![image](https://github.com/Buddkyle/osticket-prereqs/assets/149748803/7833f9d6-a85e-461d-a43f-f60849b4dc8c)

</p>
<p>
In windows explorer, navigate to C: > inetpub > wwwroot > osTicket and delete the folder called "setup". Go into the include folder and right click the file "ost-config.php" and click properties. Change the permissions on "everyone" back to "read & execute" and "read". Log into osTicket with username and password and osTicket installation is now complete.
</p>
<br />
