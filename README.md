<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This project outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>Post-Install Configuration Objectives</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Walkthrough</h2>
<h3> Section 1: osTicket Overview </h3>
<p>
<img src="https://github.com/user-attachments/assets/d7324a14-b016-42c1-af72-efdcc87487e5" width=800 />
</p>
<p>

  - For this project, I installed an open-source ticketing system called "osTicket".
  - It is commonly used by IT teams to manage incoming support requests, organize issue tracking, and ensure timely resolution through a centralized ticketing system.
  - I used it in this project to simulate a real-world help desk environment and demonstrate my ability to configure and manage support workflows.

</p>
<br />

<h3> Section 2: Configuring Roles </h3>
<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/480e7364-2c51-4e80-a64a-1739c438b2bd" width=400 />
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/c216ca00-de6a-48c5-8596-217404efb45a" width=400/>
  </td>
  </tr>
</table>

  - In osTicket, roles are used to define what actions agents can perform, such as assigning tickets, closing issues, or managing departments.
  - I created a custom role named "Supreme Admin" to serve as the primary administrator.
  - I granted this role full permissions to simulate an administrator with unrestricted access to tickets and system settings.

</p>
<br />

<h3> Section 3: Configuring Departments </h3>
<p>
<img src="https://github.com/user-attachments/assets/d47e9621-1eef-4ab0-afb4-a43947de76c5" width=500/>
</p>
<p>

  - I created a department named "SysAdmins" to organize and route tickets specifically related to system administration tasks.
  - Departments in osTicket are used to determine ticket visibility and routing across the help desk system.
</p>
<br />

<h3> Section 4: Configuring Teams </h3>
<p>
<img src="https://github.com/user-attachments/assets/cb8c6cfe-62b1-4492-83b9-59423cb76136" width=800 />
</p>
<p>

  - Next, I created a team called "Online Banking" to simulate a specialized support group responsible for banking-related inquiries.
  - Teams in osTicket are used to organize agents from different departments to handle specific types of ticket issues.

<h3> Section 5: Configuring Agents </h3>
<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/4a8e0089-ac9b-4ce5-98a7-5c8cc559b13a" />
  </td>
    <td>
      <img src="https://github.com/user-attachments/assets/3ad78acd-7dab-4421-a5b4-686437616784" width=1200/>
  </td>
  </tr>
</table>
  
    

  - Agents in osTicket represent the support staff responsible for responding to tickets.
  - I created an agent named "Jane Doe" too represent a support staff member.
  - I assigned her to the "SysAdmins" department as a "Supreme Admin" on the Online Banking Team.
  - The Supreme Admin role grants full access to manage users, tickets, departments, and settings within osTicket.

</p>
<br />

<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/d8a038cd-0755-43dd-97de-43611b2a9c6e" width=1400/>
</td>
    <td>
      <img src="https://github.com/user-attachments/assets/e1730ec4-a11c-4eeb-b2fa-2b2603f4dcbf" width=1800 />
 </td>
  </tr>
</table>

  - Next, I created another agent named "John Doe".
  - I assigned him to the "Support" department with the role of "View-only".
  - The View-only role limits his access to viewing tickets without the ability to edit, respond, or manage settings.




