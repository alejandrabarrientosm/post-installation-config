<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Log into your Windows Virtual Machine
- Open osTicket as Admin
- Configure Roles
- Configure Departments
- Configure Teams
- Configure creation of tickets
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
<h2>Log into your Windows Virtual Machine</h2>
First of all log into your Windows Virtual Machine, using Remote Desktop Connection and using your credentials. 
<p align left>
<img width="301" height="187" alt="image" src="https://github.com/user-attachments/assets/3662e595-8577-4868-a9b3-a66425c006f1" />
<img width="335" height="328" alt="image" src="https://github.com/user-attachments/assets/8026b64a-8710-41d0-a944-864ee3fa565d" />
<img width="289" height="302" alt="Screenshot 2025-11-28 142041" src="https://github.com/user-attachments/assets/449aa276-e07b-4355-b5fd-d69026a5c301" />

<h2>Open osTicket as Admin</h2>
After installed all the dependencies and osTicket from scratch we are going to make some configuration before we start working on mock tickets. In your Windows Virtual Machine click on the Admin/Analyst Login Page http://localhost/osTicket/scp/login.php and use your admin credentials previously created. 
<p align left>
<img width="1301" height="741" alt="image" src="https://github.com/user-attachments/assets/7d47b78f-f51c-4f22-92a4-cd7841e7efce" />
<img width="1900" height="691" alt="image" src="https://github.com/user-attachments/assets/9e5e5875-a8ff-418f-bc25-efaa6deb53ce" />


<h2>Configure Roles</h2>
We can create our own role and configurate it for group permissions, to do that from our Admin Panel, click on Agents tab, Roles and +Add new Role
<p align left>
<img width="1474" height="724" alt="image" src="https://github.com/user-attachments/assets/b99a9639-7332-4509-865d-5a0fc6dc1190" />
<img width="1443" height="570" alt="image" src="https://github.com/user-attachments/assets/407be184-a3d7-4608-8d0b-a1a23ff81b82" />
click on Permissions tab and click in everything  in tickets, tasks and knowledgebase and then click on add role
<p align left> 
<img width="516" height="356" alt="Screenshot 2025-11-28 144523" src="https://github.com/user-attachments/assets/bf3797a9-292f-4648-966d-1c930b2095eb" />
<img width="1458" height="706" alt="image" src="https://github.com/user-attachments/assets/8b714634-eace-481a-abf4-b7f1b1ddcb9f" />

<h2>Configure Departments</h2>
Now we configure Departments for ticket visibility, we can create a new Department by clicking on Admin Panel, Agents, Departments and +Add New Department
<p align left>
<img width="520" height="230" alt="Screenshot 2025-11-28 145223" src="https://github.com/user-attachments/assets/67249028-91d2-4461-9b8f-20becc967be7" />
<img width="341" height="403" alt="Screenshot 2025-11-28 145935" src="https://github.com/user-attachments/assets/9ab79cba-378b-4492-9566-c682e0f6bcae" />
<img width="1441" height="699" alt="image" src="https://github.com/user-attachments/assets/e6cc1a04-f779-47c7-9fb2-1e3958096580" />

<h2>Configure Teams</h2>
After created the new Department, we are going to create a new Teams for the purpose of this lab we are going to create the Online Banking Teams. To configure Teams we click on Admin Panel, Agents, Teams and +Add New Team
<p align left>
<img width="560" height="211" alt="image" src="https://github.com/user-attachments/assets/df382895-a06d-49c9-a62b-c20034e4a48d" />
<img width="564" height="383" alt="Screenshot 2025-11-28 152048" src="https://github.com/user-attachments/assets/e5909304-5ee8-4e7c-bf1a-50d6708d812f" />
For now we do not have members yet but we will create them eventually. 
<p align left>
<img width="1316" height="523" alt="image" src="https://github.com/user-attachments/assets/4b6fe0e8-0ca6-4ddc-9472-60c1ca6e02b9" />

<h2>Configure creation of tickets</h2>
The next configuration allow anyone to create tickets, the end user can create tickets without being registered or having an account. To do that, click on Admin Panel, Settings, Users and then make sure Registration Required is UNCHECK: unregistered users can create tickets
<p align left>
<img width="560" height="394" alt="Screenshot 2025-11-28 154628" src="https://github.com/user-attachments/assets/b9477f42-288e-4c90-8713-77e797bb5554" />

<h2>Configure Agents (workers)</h2>
To continue, we are going to configuere agents (workers), to do that from Admin Panel, click on Agents tab, then +Add New Agent. In this lab we are going to create 2 agents (workers)
<p align left>
<img width="563" height="242" alt="Screenshot 2025-11-28 155309" src="https://github.com/user-attachments/assets/960188cc-0c62-4826-a683-1d11152d5d89" />

Our first agent will be: Jane Doe, click on Access and assign her to SysAdmins Department and Supreme Role (due to the Supreme Role, she has permission to everything) and assign her to the Online Banking, then click on Create
<p align left>
<img width="1289" height="860" alt="image" src="https://github.com/user-attachments/assets/a4d39b94-8fe1-4b88-b642-9d26c8bced70" />
<img width="1305" height="761" alt="image" src="https://github.com/user-attachments/assets/fb6f85cc-3765-4af0-885d-53151510eeed" />
<img width="1301" height="716" alt="image" src="https://github.com/user-attachments/assets/63f404b9-f20a-4178-b7b4-1356848b3fa9" />
<img width="1302" height="614" alt="image" src="https://github.com/user-attachments/assets/2d0c411c-a642-4d98-a085-d1ecbe9e9995" />
<img width="1298" height="668" alt="image" src="https://github.com/user-attachments/assets/e44d190f-dd46-4db4-94ae-f1ed7648b5a9" />

Now we procede to create our second Agent: John Doe, click on Access and assign him to Support Department, permissions leave everything as is and click on create
<p align left>
<img width="1299" height="888" alt="image" src="https://github.com/user-attachments/assets/c2b4e3da-038e-484d-9a41-6d3faf95c1b2" />
<img width="1297" height="763" alt="image" src="https://github.com/user-attachments/assets/5e986b0b-8431-4e4c-af59-ca16b534a567" />
<img width="1297" height="725" alt="image" src="https://github.com/user-attachments/assets/7d54c237-f2b0-4ff7-8ddf-5a7b59798581" />
<img width="1294" height="617" alt="image" src="https://github.com/user-attachments/assets/e0990cac-e987-4c9f-b01f-6a58278ae89d" />
<img width="1303" height="676" alt="image" src="https://github.com/user-attachments/assets/e236009d-0d48-4de0-ba89-e9df810318b4" />


<h2>Configure Users (customers)</h2>
To continue with our configuration we have to create our users (Karen and Ken), to create them we have to change from Admin Panel to Agent Panel on the top right corner, click on Users and then +Add User
<p align left>
<img width="562" height="227" alt="Screenshot 2025-11-28 162120" src="https://github.com/user-attachments/assets/fd9e2940-8d33-4605-81bd-3bbfc7d40168" />

Create first Karen, enter a fake email (just for this lab purpose) and then her full name, click on Add User
<p align left>
<img width="564" height="314" alt="Screenshot 2025-11-28 163437" src="https://github.com/user-attachments/assets/ccecfdb0-3be2-47d2-8b32-a68dc719490a" />
<img width="1295" height="543" alt="image" src="https://github.com/user-attachments/assets/02f842dd-ecbb-4e95-9be8-787c28420138" />


Our second user is Ken, enter a fake email (just for this lab purpose) and then his full name, click on Add User
<p align left>
<img width="561" height="338" alt="Screenshot 2025-11-28 163153" src="https://github.com/user-attachments/assets/9f504d75-9f8f-4cfb-902f-1b873bac1ba8" />
<img width="1305" height="597" alt="image" src="https://github.com/user-attachments/assets/8c1a7436-4ae7-4678-8dbb-a96bc08cc70f" />

<h2>Configure SLA</h2>
We finished with our Agents and Users configuration, now we configure our SLA (Service Level Agreement) which is basically the time we have to do an specific task, wether is responding to a ticket or completing the ticket, etc. To configure this we go back to the Admin Panel, click on Manage, SLA and +Add New SLA Plan (for this lab we are going to create 3 different) 
<p align left>
<img width="562" height="222" alt="Screenshot 2025-11-28 164535" src="https://github.com/user-attachments/assets/948a41c7-2aa2-42e0-8789-99b6196e4ac6" />

Name: Sev-A Grace Period: 1 hour, Schedule: 24/7 and click on Add Plan
<p align left>
<img width="562" height="395" alt="Screenshot 2025-11-28 164958" src="https://github.com/user-attachments/assets/dd578f80-55b9-46e7-9839-0dc8ebbd1a7f" />

Name: Sev-B, Grace Period: 4 hours, Schedule: 24/7 and click on Add Plan
<p align left>
<img width="562" height="389" alt="Screenshot 2025-11-28 200357" src="https://github.com/user-attachments/assets/5966a4b4-23ce-42a0-afcd-a0823f1794bd" />

Name: Sev-C, Grace Period: 8 hours, Business Hours and click on Add Plan
<p align left>
<img width="558" height="393" alt="Screenshot 2025-11-28 200752" src="https://github.com/user-attachments/assets/07005db6-296d-4a07-a587-ccc2f07cd5fb" />

All SLA's have been created
<p align left>
<img width="1296" height="659" alt="image" src="https://github.com/user-attachments/assets/0909131a-da5d-4fd6-80f5-cf106fd4e811" />


<h2>Configure Help Topics</h2>
Last configuration is: Help Topics (For when users create a ticket), this is kind of a category. To do this click on Admin Panel, Manage, Help Topics and +Add New Help Topics
<p align left>
<img width="564" height="285" alt="Screenshot 2025-11-28 201743" src="https://github.com/user-attachments/assets/39ec4620-6460-49b3-bee0-f986fef2897b" />

For the purpose of this lab we are going to create 5 Help Topics:

Topic: Business Critical Outage, Parent Topic: Report a Problem, click on Add Topic
<p align left>
<img width="563" height="384" alt="Screenshot 2025-11-28 202127" src="https://github.com/user-attachments/assets/86dc8048-d63b-46f4-a30a-9c35d99a7531" />
<img width="1301" height="659" alt="image" src="https://github.com/user-attachments/assets/1f8834ab-1ae9-42fb-96f6-fafe8beff372" />

Topic: Computer Issues, Parent Topic: Report a problem, click on Add Topic
<p align left>
<img width="562" height="387" alt="Screenshot 2025-11-28 202849" src="https://github.com/user-attachments/assets/527164e2-65eb-48d4-95ac-65ec68ba4ecf" />
<img width="1298" height="635" alt="image" src="https://github.com/user-attachments/assets/1c8968f2-220f-4848-b5f8-a7b016719690" />

Topic: Equipment Request, Parent Topic: General Inquiry, click Add Topic
<p align left>
<img width="562" height="386" alt="Screenshot 2025-11-28 203252" src="https://github.com/user-attachments/assets/3ac33ad1-0b74-4bba-851d-04fa0173a1ea" />
<img width="1296" height="665" alt="image" src="https://github.com/user-attachments/assets/a1dde697-10f4-4ea6-886c-1cb63ef400c4" />

Topic: Password Reset, Parent Ticket: Report a Problem, click on Add Topic
<p align left>
<img width="564" height="387" alt="Screenshot 2025-11-28 203715" src="https://github.com/user-attachments/assets/7217611f-aa4c-40f8-9c20-5cc1753f2531" />
<img width="1350" height="702" alt="image" src="https://github.com/user-attachments/assets/3b435408-04e2-41a1-83c0-89f9eef3025e" />

Topic: Other, Parent Ticket: General Inquiry, click on Add Topic
<p align left>
<img width="564" height="387" alt="Screenshot 2025-11-28 204130" src="https://github.com/user-attachments/assets/e042030e-a671-4788-98a5-76948803f8c7" />
<img width="1295" height="640" alt="image" src="https://github.com/user-attachments/assets/d998193e-4d9c-4a57-8897-788f795d3515" />
<img width="1295" height="887" alt="image" src="https://github.com/user-attachments/assets/a12a944d-c1c8-48c4-aa99-9453339abe48" />


For now this conclude our general initial set up of osTicket






