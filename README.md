<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)


<h2>Deployment and Configuration Steps</h2>

<p>
<img src="Screenshot 2025-02-12 032328.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 1- Make a Window virtual machine and a Window server 2022.Once both are made go into the network setting of the server and set it so the IP address is static.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 035015.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 2- Go to the network setting and change the DNS servers from default to the IP address of the server.(the static IP address)
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 034720.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 3- Remote connect into the Window server and click on add roles and features. 
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 040321.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 4- Click next until you get to the server role tab click the Active Directory Domain Service an make sure the box is checked.Then click next and finish installing the features.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 040912.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 5- After you click on the flag on the top right of the screen.Click on the promote this server to a domain controller.
</p>
<br />


<p>
<img src="Screenshot 2025-02-12 041005.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 6- Click on add a forest and set the forest to mydomain.com.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 041539.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 7- Click next on the rest and then after it finishes installation it will reset the server. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
