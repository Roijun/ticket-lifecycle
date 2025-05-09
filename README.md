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

- Ticket Creation

Admin Login Page - http://localhost/osTicket/scp/login.php

End User Portal - http://localhost/osTicket

We're going to be creating a ticket as an end user. We'll want to navigate to the end user portal for osTicket so we can sign in as a user. I provided the link here just in case you lost or forgot it when osTicket diplsayed it for us earlier after we successfully completed the installation process. Once at the end user portal we just have to hit 'Open a New Ticket' from the right hand side. The only information we need to create a help ticket is the users name, and their email address. For this ticket we'll create we'll just say that the entire mobile/online banking system is down. In the box below I'll fill out the issue with a bit more depth. 

![opennewticket](https://github.com/user-attachments/assets/e991e26f-8797-47c8-a6c0-ebb7e7655d28)

With everything we need in order we can go ahead and select 'Create Ticket' in all red in the bottom left. 

- Ticket Properties

Next we'll be logging in as our agent 'John' that we created in the last walkthrough. First navigate back to the admin portal, and then enter the information for the agents username and password which we set and logged in our notepad earlier. Once logged in you should be taken to the open ticket page, and you should be able to see and open the specific ticket that we just created as our end user.

![ticketprop](https://github.com/user-attachments/assets/d078bb08-7a92-43a7-88c1-f4f996aed055)

Here we can observe all of the tickets properties. Including the priority, department, SLA, and Assigned To catagories. We're going to go through and set these properties. Starting with the SLA, we're going to change it from default to Sev-A. For the reason we'll just put 'customers unable to do online banking'. Sev-A fits this issue well, since the severity is impacting an entire department. We'll also change the help topic from 'Report a Problem' to 'Business Critical Outage', since this help topic fits the issue more accurately. The final setting that we'll change is the 'Assigned To' category, and assign it to the 'Online Banking' team that we had previously created. This is all that we're going to configure for this ticket, it should look like the picture below once we're finished.

![properties overview](https://github.com/user-attachments/assets/fcc06b6d-3651-49bd-aa5c-358762aae361)

- Working Tickets

We're going to now 'work' the ticket as our other agent 'Jane' that we created some time ago. We'll want to logout as john, and use the username and password that we saved to login to Jane's account. Once logged in we should see the same ticket as the first thing that we see. We'll want to click on the ticket and go down to the bottom to reply to the ticket with an update on potential fixes. You'll also notice the 'Ticket Thread' section, this is where we'll see every update to the ticket, whether that be assigning it to a specific team, or replying with potential fixes to the ongoing issue at hand.

![ticket thread](https://github.com/user-attachments/assets/5aefa6cd-de37-4aa2-ac72-fed6f9ded23f)

At the bottom we can reply with something like 'the problem might be related to recent updates, we tested them sufficiently but I'm going to look into it further and roll them back if I determine that they were the cause' once finished hit reply. Our update will be added into the ticket thread, and everyone who has access will be able to see that we are looking into the issue. We're going to pretend that we went onto the backened as Jane and that we found that the issue was indeed caused by the recent updates that we made. So in our mock scenario we would uninstall the update and roll back the system to a previous version to fix the online banking issue. Once we fix the issue we want to update the ticket thread with a new reply stating what we did, and continue on to change the status of the ticket to resolved. Im going to reply with 'It was determined that the root cause of the issue was derived from the recent updates. We rolled it back and notified the vender, the online banking system should now be up and running'. 

![issueresolved](https://github.com/user-attachments/assets/ac651a2b-098a-4260-87ef-fc48b19b27ff)

After replying to the thread that the issue has been resolved we can proceed with closing out the ticket. At the top of the page there should be a flag icon, when you hover over it, it reads 'Change Status'. Click on the icon and change the ticket status to 'Resolved'. It will ask for a reason, and you can enter how the issue was fixed and that the banking system is back online. That's the end of the process for the first mock ticket we'll be going over.

- Ticket Creation Pt.2

We're going to create another ticket using the user we just previously used. This one we'll throw under 'General Inquiry'. For this mock scenario the accounting department will be having some issues with using the adobe software. As we create the ticket we'll fill in the issue summary title with an intially vauge titleW, sometimes tickets aren't always concise or logical, and it's up to the agent who's assigned to the ticket to diagnose what the actual issue may be. For the title we'll say 'accounting department needs adobe upgrade' and for the larger box we'll fill it in with a more detailed explanation of the issue such as 'It looks like multiple people in the accounting department are unable to use their adobe software'. With this information in place we can go ahead and create our ticket.

![accounting](https://github.com/user-attachments/assets/9f05f21e-28fd-4ecb-b566-e92567e464a0)

- Ticket Properties Pt.2

We're going to sign in to the agent panel and work this ticket as John. In this mock scenario if I was John I would want to get in touch with the user who created the ticket, preferably call them to clarify the issue. Let's say we called them and they tell us that whenever they try and open the adobe software it closes right away, and when we clarify who 'they' is we find out that it's only two individuals within the accounting department wrestling with this issue. We go ahead and ask that the two individuals restart their systems to see if it's enough to fix the issues. Our point of contact within the accounting department says he'll try it and get back to us after lunch. Now that we have the stage set we can go ahead and configure some of the properties based on our information. So the impact is actually not as bad as it may have seemed when the ticket first appeared, we'll go in and set the SLA to a class Sev-C. Reason shall be 'only two people in the accounting department having issues'. We're going to assign it to the support team, and then assign the actual ticket to our agent John. 

-Working Tickets Pt.2

Below will be our first update to our ticket.

![ticketupdate](https://github.com/user-attachments/assets/1389632f-575b-4369-8596-49b5a6795bb0)

In our mock scenario we waited until after lunch, and the point of contact notifed us that the restart fixed whatever issue was occuring with the employees adobe software. We'll update our ticket with the information before changing the status of the help ticket to resolved. We'll reply to the thread one last time, 'Point of contact states that restart of the affected computers fixed the issue, closing out the ticket' and change the status to resolved. 

![finished](https://github.com/user-attachments/assets/814e4623-fc92-410a-8058-821e61e032ae)

This concludes this walkthrough on tickets and the ticket lifecycle. We went through and created some mock tickets as end users and configured their properties, we also 'solved' these mock tickets as agents through the agent portal. You should have gotten a decent feel for what the ticket process entails and for the osTicket software as well. Experience with the software may be extremely vaulable when dealing with real world scenarios and adjacent softwares that work similarly, easing the learning process to new individuals taking up work as agents.





<br />
