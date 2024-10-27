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

- Configure Roles, Departments, & Teams 
- Allow ticket creation
- Configure Agents & Users
- Create SLA
- Create Help Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/qaTQtzi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/U9Pi2qq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Login to osTicket with your credentials you selected during the initial setup of osTicket. Notice you will automatically be directed to Agent Panel. In the top right corner of the page you can toggle between Agent and Admin Panel. This is where you will configure your Groups, Dept, ect.
</p>
<br />

<p>
<img src="https://i.imgur.com/BLd34dL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First, we will be configuring the Roles for grouping permissions. From the Admin Panel select Agents -> Roles -> Create roles. From here you will create Supreme Admin and grant it "all permissions".
</p>
<br />

<p>
<img src="https://i.imgur.com/dmM1hPf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After Roles has been configured, we need to configure the Departments, which allows for ticket visibility within Help Desk. Within the Admin Panel select the bolded Agents, then the sub-category Departments. Enter SysAdmin as the department name.
</p>
<br />

<p>
<img src="https://i.imgur.com/evSGGJ9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After Departments have been established we will configure Teams from within the same Agent tab under Admin Panel. Selct Teams and create an Online Banking Team. This allows us to pull Agents from different Depatments.

<p>
<img src="https://i.imgur.com/b0ipuap.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once we have configured our Roles, Teams, and Departments we have to allow access to create tickets by anyone. Again, under the Admin Panel go to Settings and then the sub-category User Settings. You must UNCHECK: unregistered users can create tickets. This ensures that registration is required by users to login and create tickets within the system.

<p>
<img src="https://i.imgur.com/E70xaIQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


<p>
<img src="https://i.imgur.com/NolOYkW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<p>
<img src="https://i.imgur.com/2CAOQz2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we must configure Agents/workers to handle the tickets that will be created within the ticketing system by the Users/customers. Under the Agent Panel -> Agents -> Add New. Once here you can add your Agents as desired. Be sure to register the Agent under a Team and allow access. Here you can also assign a generic password for the agent (Password1). If doing a mock lab be sure to unclick "Send agent a reset email for password" and "Require password change at next login" being that the email addresses and names provided are not real. 
  
<p>
<img src="https://i.imgur.com/y7BOTnS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/BuJ12fA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>  
After you have configured your Agents we can now configure our Users/Customers. Under Agent Panel -> Users -> Add New, once you have created users, notice how the user now is able to create tickets within the system. 

<p>
<img src="https://i.imgur.com/AblBZgC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 <p>
<img src="https://i.imgur.com/QCxb22y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
Next, we have to configure the SLA, which is a standard of the level of importance or each ticket and how long you have to complete the ticket after submission. Be aware that each business may have their own standard. Under Admin Panel -> Manage -> SLA we will create three basic SLA levels. Notice after creation you can see the active status, meaning that when an Agent is reviewing tickets they can assign the level of importance to each before directing the ticket to the appropriate department to be fixed.

<p>
<img src="https://i.imgur.com/WAqJtMu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/1JBsDbu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finally, we have to configure Help Topics for when a user creates a ticket. Under Admin Panel -> Manage -> Help Topics -> Add New, you can add as many topics as you like that relates to the business. I have added some common issues. Once this is done you can save it and now your ready to create tickets for your users. 






