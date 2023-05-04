<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure SLA
-Configure Help Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://github.com/ElwoodMattHowell/images/blob/main/osTicket-admin.png" height="80%" width="80%" alt="osTicket admin panel"/>
</p>

If you have not set up osTicket, please checkout https://github.com/elwoodmatthowell/osticket-prereqs for instructions on how to do so.  If you have osTicket set up and ready to go, navigate to http://localhost/osTicket/scp/login.php.  There you will be prompted for a username and password.  Enter the administrator username and password you used in the osTicket set up. Once you have logged in you will be brought directly to the _Agent Panel_.  From there, you can click through to the _Admin Panel_ in the upper right corner of the panel.
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

Our first task in the admin panel will be to configure Roles.  Roles are the permissions granted to Agents per Department that they have access to.  For more information on Roles, please visit https://docs.osticket.com/en/latest/Admin/Agents/Roles.html.  From the Admin Panel we can click through to _Agents_ -> _Roles_.  From here, click on _Add New Role_.  For the name you can type in 'Supreme Admin.'  For this Role we will give the user full access to all.  Once you have entered the name of the Role, click _Permissions_.  Check all of the boxes under _Tickets_, _Tasks_, and _Knowledgebase_.  Once they are all checked, click _Add Role_.  

<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
