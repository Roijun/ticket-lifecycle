<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Tickets and Ticket Lifecycle</h1>
<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Have the osTicket software successsfully installed onto a virtual machine and configured with all of the items that we created in the last walkthrough.
 
<h2>Overview</h2>

In this walkthrough we're going to be creating tickets as end users and observing all the ticket properties and responding to them as help desk professionals. Solving mock tickets gives us a feel for how we would use the osTicket software to solve issues in real world scenarios, and deepens our understanding with the osTicket software.


<h2>Tickets and Ticket Lifecycle</h2>

- Maintenance Department

Before we start creating mock tickets we're going to go over and delete the maintenance department to prevent tickets from getting auto assigned to it, as it sometimes has a tendacy to do so. To do that we're going to need to be logged into osTicket as an admin, before clicking on the 'Admin Panel' at the top right of the screen. Once there click on the 'Agents' tab, and navigate to the departments section. 

![maintenance department](https://github.com/user-attachments/assets/cc8f3a44-ef78-42d0-8638-f5b547238983)

From here deleting the maintenance department is pretty simple, we just need to check the box on the left hand side, then hit the 'More' button near the top right. 'Delete' should be an option that appears underneath the 'More' dropdown menu. It will ask you to confirm once more before allowing you to actually delete the department.

- Creating a Ticket

Admin Login Page - http://localhost/osTicket/scp/login.php

End User Portal - http://localhost/osTicket

We're going to be creating a ticket as an end user. We'll want to navigate to the end user portal for osTicket so we can sign in as a user. I provided the link here just in case you lost or forgot it when osTicket diplsayed it for us earlier after we successfully completed the installation process. Once at the end user portal we just have to hit 'Open a New Ticket' from the right hand side. The only information we need to create a help ticket is the users name, and their email address. For this ticket we'll create we'll just say that the entire mobile/online banking system is down. In the box below I'll fill out the issue with a bit more depth. 

![opennewticket](https://github.com/user-attachments/assets/e991e26f-8797-47c8-a6c0-ebb7e7655d28)

With everything we need in order we can go ahead and select 'Create Ticket' in all red in the bottom left. 

- Ticket Properties

Next we'll be logging in as our agent 'John' that we created in the last walkthrough. First navigate back to the admin portal, and then enter the information for the agents username and password which we set and logged in our notepad earlier. Once logged in you should be taken to the open ticket page, and you should be able to see and open the specific ticket that we just created as our end user.

![ticketprop](https://github.com/user-attachments/assets/d078bb08-7a92-43a7-88c1-f4f996aed055)

Here we can observed all of the tickets properties. Including the priority, department, SLA, and Assigned To catagories. We're going to go through and set these properties. Starting with SLA, 



<br />
