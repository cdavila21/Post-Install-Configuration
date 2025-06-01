<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>
<h1 style="text-align: center; font-weight: bold; font-size: 16pt;">osTicket - Post Configuration Setup</h1> </p>
</p>
This tutorial outlines the post-configuration setup of the osTicket system.

<p>

</p>
</p>
<p>
We have successfully configured osTicket from scratch. Now, we will focus on system administration and perform some post-installation setup.

<hr>
<h1 style="text-align: center; font-weight: bold; font-size: 16pt;">Creating Roles </h1> </p>

First, we will configure new roles within the help desk: To do this, navigate to Admin Panel > Agents > Roles. Click "Add New Role" and enter the name of the new role. You can also modify specific role permissions. In this case, as we are creating a "Supreme Admin," we will assign all permissions to this role. It is important to note that roles define an agent's permissions, so not all agents will have unrestricted access. 

If you followed the steps correctly, your screen should resemble the example shown, where the "Supreme Admin" role has been successfully created.
</p>

<img width="713" alt="image" src="https://github.com/user-attachments/assets/f2125f54-20ee-4a02-8f02-500240d68b0e">


</p>
<br />
<p>
</p>

<hr>

<p>
  <h1 style="text-align: center; font-weight: bold; font-size: 16pt;">Creating Departments and Teams </h1> </p> <br>
  
Navigate to the Agents tab and select the "Departments" button. In this section, you can create new departments, with each agent being assigned to a specific department based on their role within the helpdesk.  <br>
  
For this tutorial, we will create the  four departments <br>
- System Administrators
- Payroll
- Support
- Leave of Absence
- Human Resources 
  
Company ticketing systems are generally organized into departments such as System Administration, Payroll, Support, Leave of Absence, and Human Resources. This structure ensures that tickets are efficiently routed to the appropriate teams, promoting faster resolutions, streamlined SLA management, and accountability by allowing each department to handle requests relevant to their specialized roles and protocols.

</p>
<p>
<img width="710" alt="image" src="https://github.com/user-attachments/assets/020fa493-7d26-4c14-a528-ac20bd1cf125">

</p>
<br />

<p>
Once a new department is configured, the next step is to establish a specialized team. Teams enable cross-departmental collaboration by assembling agents from various departments, allowing for the creation of high-performing groups with top technicians from specific areas.

For instance, a representative from Human Resources could be granted access to Payroll and Leave of Absence functions, empowering them to work on and resolve relevant tickets. This structure enhances operational flexibility and ensures that high-priority tickets are managed by the most qualified personnel. 

  
</p>
<br />
<p>
<img width="720" alt="image" src="https://github.com/user-attachments/assets/1af8d5e3-703c-4255-8d14-f495335a4c61">
</p>
<p>

<hr>
  <h1 style="text-align: center; font-weight: bold; font-size: 16pt;">Configuring Ticket Submission Access for All Users </h1> </p> 
  
With the new team established, the next step is to configure a setting that enables all users to create tickets. Navigate to Admin Panel > Settings > User Settings to apply this configuration.

</p>
<br />
<img width="701" alt="image" src="https://github.com/user-attachments/assets/cd7f2a6c-f54e-4bb8-ae65-afdbd174e465">

</p>

<br />

<hr>

<p>
  <h1 style="text-align: center; font-weight: bold; font-size: 16pt;">Creating Agents</h1> </p>

Below is a list of agents already created, followed by images detailing the steps to assign agents to specific departments and set their levels of access. <br>


<img width="720" alt="image" src="https://github.com/user-attachments/assets/00699565-e695-4fec-b0b3-2e4be852c047">

</p>
<b> STEP 1 </b> Admin Panel -> Agents -> Agents - Add New Agent <br>
<br>
<img width="704" alt="image" src="https://github.com/user-attachments/assets/da18c6e8-39ac-4e88-94c1-48f85b7402b8"> <br>

<b> STEP 2 </b> Fill out user information<br>

<img width="511" alt="image" src="https://github.com/user-attachments/assets/0a254ac5-3fae-40d4-9844-a0ccf3d5580e"><br>


<b> STEP 3 </b> Assign the agent’s designated department and access level; additional access privileges can be configured as necessary.<br>

<img width="604" alt="image" src="https://github.com/user-attachments/assets/7852e90d-d36d-4d19-9977-a07a971c9881"><br>


<b> STEP 4 </b> Assigning Permissions<br>

<img width="338" alt="image" src="https://github.com/user-attachments/assets/9a4d21a3-b0b9-4f51-9ca8-d0acc8c03a53"><br>

<b> STEP 5 </b> Team assignments can be configured here and updated from the Teams tab when adding multiple agents simultaneously.<br>

<img width="490" alt="image" src="https://github.com/user-attachments/assets/98b0955f-4d1f-433f-b1bd-a93381306f63"><br>

- Additional settings, including SLAs, managers, and email configurations, can be customized within the Departments tab. System administrators can also monitor ticket activity and assume responsibility when a Level 3 team member is unresponsive or when there is a direct request from a VP for personal handling of a ticket.


</P>

<hr>

<p>
    <h1 style="text-align: center; font-weight: bold; font-size: 16pt;">Creating SLA's</h1>
SLA Plans define the time frame within which the help desk is expected to resolve a specific ticket. These plans are created by navigating to Admin Panel > Manage > SLA Plans. Each SLA is associated with a schedule that includes a designated grace period. For instance, the SEV-1 SLA is set to operate 24/7 with a one-hour grace period.

</p>
<br />
<p>
For this tutorial, we will create the  three levels: <br>
- Sev 1 - Tier 1 Support <br>
- Sev 2 - Tier 2 Support <br>
- Sev 3 - Tier 3 Support <br>
</p>

<p> 

  <img width="727" alt="image" src="https://github.com/user-attachments/assets/adb796fe-93d7-4d57-a0d1-1cd4320aa98d">

</p>
Creating a Sev-1 plan with the appropriate grace time and the schedule type. This will be adjusted according to the sev type<br>
<img width="683" alt="image" src="https://github.com/user-attachments/assets/5803f76a-0619-47b9-9b7a-15e3479b89ab">

</p>

<hr>

<p>
    <h1 style="text-align: center; font-weight: bold; font-size: 16pt;">Help Topics</h1>

<p>
Help topics help users categorize their tickets. In the example below we have made a help topic for "Business Critical Outage" this can be if customers cannot access payroll or possibly tier 1 support. 
</p>
<br />
<img width="729" alt="image" src="https://github.com/user-attachments/assets/d29086f0-217f-4f8e-90b2-ef3c490be284">

</p>
<p>
