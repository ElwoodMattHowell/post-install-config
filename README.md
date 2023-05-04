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
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-agents-users.png" height="40%" width="40%" alt="configure roles"/>
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-roles-name.png" height="40%" width="30%" alt="configure roles">
   <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-roles-permissions.png" height="40%" width="25%" alt="configure rolese">
</p>


Our first task in the admin panel will be to configure Roles.  Roles are the permissions granted to Agents per Department that they have access to.  For more information on Roles, please visit https://docs.osticket.com/en/latest/Admin/Agents/Roles.html.  From the Admin Panel we can click through to _Agents_ -> _Roles_.  From here, click on _Add New Role_.  For the name you can type in 'Supreme Admin.'  For this Role we will give the user full access to all.  Once you have entered the name of the Role, click _Permissions_.  Check all of the boxes under _Tickets_, _Tasks_, and _Knowledgebase_.  Once they are all checked, click _Add Role_.  
<br />


<p float="left">
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-agents-departments.png" height="40%" width="45%" alt="configure departments"/>
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-add-department.png" height="40%" width="25%" alt="configure departments">
</p>


Our next task will be to configure Departments.  For more information on Departments, please visit https://docs.osticket.com/en/latest/Admin/Agents/Departments.html.  From the Admin Panel, click through _Agents_ -> _Departments_, and click _Add New Department_.  In the _Name_ box, type 'System Administrators' or whatever you would like your department to be called.  For the purposes of this exercise, we will leave the rest of the default settings in place.  At the bottom of the page, click _Create Dept_.     
<br />


<p float="left">
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-agents-teams.png" height="40%" width="35%" alt="configure teams"/>
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-teams-team.png" height="40%" width="25%" alt="configure teams">
    <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-teams-members.png" height="40%" width="35%" alt="configure teams">
</p>


Continuing our configurations, we will now configure Teams.  Teams allow you to pull Agents from different Departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter.  For more information on Teams, please visit https://docs.osticket.com/en/latest/Admin/Agents/Teams.html.  From the Admin Panel, click through _Agents_ -> _Teams_, and click _Add New Team_.  In the _Name_ box, type 'Level II Support' or whatever you would like your Team to be called.  Under the _Members_ tab, click the drop down arrow next to _Select Agent_.  You should see your name there, click your name and then _Add_.  Back under the _Teams_ tab, you should now be able to assign yourself as _Team Lead_.  Click _Create Team_.     
<br />


<p float="left">
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-agents.png" height="40%" width="40%" alt="configure agents"/>
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-new-agent.png" height="40%" width="20%" alt="IIS homepage">
    <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-agents-access.png" height="40%" width="35%" alt="configure agents">
</p>


Next, we will configure Agents.  Agents are given access to the help desk with the intent to respond and resolve the tickets.  For more information on Agents, please visit https://docs.osticket.com/en/latest/Admin/Agents/Agents.html.  From the Admin Panel, click through _Agents_ -> _Agents_, and click _Add New Agent_.  Fill in _First Name_ and _Last Name_, and _Email Address_. We can leave phone number blank for now.  Create a _Username_.  Click the _Access_ tab, under _Primary Department_, select a _Department_ and a _Role_.  Leave _Permissions_ as they are, and under the _Teams_ tab you can select a team.  Now click _Create_.     
<br />


<p float="left">
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-agent-users.png" height="40%" width="45%" alt="configure users"/>
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-add-user.png" height="40%" width="35%" alt="configure users">
</p>


Now we move on to Users.  Users are the ticket owners of the tickets in the help desk.  For more information on Users, please visit https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html.  From the Admin Panel, in the upper right corner, click _Agent Panel_.  Under the _Users_ tab, click _Add User_.  Fill out _Email Address_ and _Full Name_ and then click _Add User_.     
<br />


<p float="left">
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-manage-sla.png" height="40%" width="45%" alt="configure SLA"/>
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-add-sla.png" height="40%" width="35%" alt="configure SLA">
</p>


Next up, we will configure our SLA Plans.  The purpose of the SLA Plan is to provide a length of time in which the help desk Administrator expects tickets to be closed.  For more information on SLA plans in osTicket, please visit https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html.  First, navigate back to the _Admin Panel_.  From the _Admin Panel_ click through _Manage_ -> _SLA_, and click _Add New SLA Plan_.  You can add as many SLA Plans as are needed.  Typical names might be SEV-A, SEV-B, SEV-C, or something similar.  _Grace Period_ indicates the number of hours in which tickets must be resolved.  _Schedule_ has 3 choices, 24-7 (all day everyday), 24-5(all day workweek), or Monday-Friday, 8am-5pm(workdays during the work week).  Make choices for all of these and click _Add Plan_.
<br />


<p float="left">
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-add-helptopic.png" height="40%" width="45%" alt="configure Help Topics"/>
  <img src="https://github.com/ElwoodMattHowell/images/blob/main/osticket-helptopic-options.png" height="40%" width="35%" alt="configure Help Topics">
</p>


Our final configuration will be of Help Topics.  Help Topics will help streamline your end-user’s help desk experience to ensure proper assignment and prompt response to the ticket.  For more information on SLA plans in osTicket, please visit https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html?highlight=help%20topics.  From the _Admin Panel_ click through _Manage_ -> _Help Topics_, and click _Add New Help Topic_.  Under the _Help Topic Information_ tab, you can enter a name for the Help Topic.  Under the _New ticket options_ tab you can set priorities and assign an SLA Plan among other options.  When you have configured your Help Topic, you can click _Add Topic_.  You are now ready to use osTicket!
<br />
