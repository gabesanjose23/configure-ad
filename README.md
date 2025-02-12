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
<img src="Screenshot 2025-02-12 042436.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 8- Open up the Window server then on the window search for Active Directory User and Computers.Right click mydomain.com ,add new and organizational unit after that make a name for it.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 042832.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 9- After you make the organizational unit add a user.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 043027.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 10- Make the username and password and here you can set it so when they login next time you can make it so they have to put in a new password and other configurations.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 043316.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 11- Once you make the account you have to set it in a group. This one is an Admin so I right click on the user and make it a member of the admin group and apply the changes.Here you can also configure a lot of things about the account.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 044125.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 12- Go to remote desktop connection and connect to the window machine go to the setting and click on advance name change.Once your there click on change and make it from workgroup to Domain and change it to the name of your domain.Put in the username and password for one of the account in the domain.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 044500.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 13- You go back to the server and back into the Active Directory User and Computers then a new file name computers will pop up with the computer you just login on that domain.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 045327.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 14- While you are on the server or if you are an admin you can search up group Policy Management and set group policy for different organizational units or groups/people.
</p>
<br />

<p>
<img src="Screenshot 2025-02-12 045822.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Step 15- While you are on the server or an admin you can also check logs for security or troubleshooting by clicking on the window key and searching for the Event viewer.
</p>
<br />
