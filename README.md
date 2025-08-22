<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Installation Setup and Configuration</h1>
This project documents the post-install configuration of the open-source help desk ticketing system osTicket. I configure departments, roles, SLA plans, users and user permissions to simultate realistic IT support structure. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

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
     <img src="https://github.com/user-attachments/assets/201c210f-9dc5-41ec-8de9-43a33e06972a" />
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
      <img src="https://github.com/user-attachments/assets/29ebeafd-a8a0-4e5f-830a-3b751ddf3ab5" />
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/f99cb707-d277-45ea-8e26-6afedbcc5683" width=1200 />
 </td>
  </tr>
</table>

  - Next, I created another agent named "John Doe".
  - I assigned him to the "Support" department with the role of "Expanded Access".
  - The Expanded Access role allows him to view and manage tickets across multiple departments, but with limited administrative privileges.

</p>
<br />

<h3> Section 6: Configuring Users </h3>
<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/8bd07365-8059-4ba8-8704-42a7e32eabef" />
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/51c59f5b-ff5c-47a9-ae1c-5ec3c7cd21c8" />
  </td>
  </tr>
</table>
   
  - Users in osTicket represent the end-users who submit support tickets to report issues or request assistance.
  - I created two users named "Karen" and "Ken", who will both be used to submit support tickets in a later project.

</p>
<br />

<h3> Section 7: Configuring SLA (Service Level Agreement) </h3>
<p>
<img src="https://github.com/user-attachments/assets/6cc7bd3b-3848-41a4-b88b-392a8d587b88" width=800/>
</p>
<p>

  - In osTicket, an SLA (Service Level Agreement defines the expected response and resolution time for support tickets based on priority or issue type.
  - I created my first SLA plan named "Sev-A", representing high-severity problems that require faster response and resolution times.
  - I set a 1-hour grace period to ensure tickets are marked overdue quickly if not addressed within the expected timeframe.
  - I selected a 24/7 schedule so the SLA applies even outside of business hours.


</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/b7651224-44f1-4531-bcd7-228d1236c7f4" width=800 />
</p>
<p>

  - Next, I created another SLA plan named "Sev-B", representing medium-severity issues which are less urgent than Sev-A.
  - I set a 4-hour grace period to ensure timely responses without the urgency level of Sev-A
  - I applied a 24/7 schedule to ensure ongoing support.

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/100ead50-7710-4631-b2b5-782ff93eb9bf" width=800 />
</p>
<p>

   - Lastly, I created another SLA plan named "Sev-C" for low-severity tickets such as general inquiries or non-urgent issues.
   - I assigned a grace period of 8 hours to allow agents to prioritize more critical tasks first.
   - I also set the schedule to operate during business hours only.

</p>
<br />

<h3> Section 8: Configuring Help Topics </h3>

<p>
<img src="https://github.com/user-attachments/assets/8bcefef6-d4da-4f4f-b605-3842aee58219" width=800 />
</p>
<p>

  - Help Topics in osTicket are used to categorize tickets based on the type of issue reported by the end-user.
  - I created a series of Help Topics to categorize support requests by issue type and priority such as "Password Reset", "General Inquiry", and "Business Critical Outage".

</p>
<br />

<h2>Conclusion</h2>
This project gave me the hands-on experience in setting up a functional help desk system tailored to an IT support workflow. I developed a deeper understanding of the IT support structure and how effective configurations improves ticket management and team efficiency. This laid the groundwork for simulating a real-world help desk environment.
   
   



