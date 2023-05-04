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


<p float="left">
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-agents-users.png" height="40%" width="40%" alt="install/enable iis"/>
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-roles-name.png" height="40%" width="30%" alt="IIS homepage">
   <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-roles-permissions.png" height="40%" width="25%" alt="IIS homepage">
</p>


Our first task in the admin panel will be to configure Roles.  Roles are the permissions granted to Agents per Department that they have access to.  For more information on Roles, please visit https://docs.osticket.com/en/latest/Admin/Agents/Roles.html.  From the Admin Panel we can click through to _Agents_ -> _Roles_.  From here, click on _Add New Role_.  For the name you can type in 'Supreme Admin.'  For this Role we will give the user full access to all.  Once you have entered the name of the Role, click _Permissions_.  Check all of the boxes under _Tickets_, _Tasks_, and _Knowledgebase_.  Once they are all checked, click _Add Role_.  
<br />


<p float="left">
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-agents-departments.png" height="40%" width="40%" alt="install/enable iis"/>
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-add-department.png" height="40%" width="30%" alt="IIS homepage">
</p>


Our next task will be to configure Departments.  For more information on Departments, please visit https://docs.osticket.com/en/latest/Admin/Agents/Departments.html.  From the Admin Panel, click through _Agents_ -> _Departments_, and click _Add New Department_.  In the _Name_ box, type 'System Administrators' or whatever you would like your department to be called.  For the purposes of this exercise, we will leave the rest of the default settings in place.  At the bottom of the page, click _Create Dept_.     
<br />
