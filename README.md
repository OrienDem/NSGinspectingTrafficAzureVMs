<p align="center">
<img src="https://i.imgur.com/AeiqMDZ.png" alt="Traffic Examination"/>
</p>

<h1>Network-File-Shares-and-Permissions</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />

<h2>Environments and Technologies Used</h2>

* Microsoft Azure (Virtual Machine Instances)
* Microsoft Remote Desktop
* Shared Network Files

<h2>Operating Systems Used </h2>

* Windows 10</b> (21H2)
* Windows Server 2022
</p>

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/UH5XBX5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 1 in DC1 create 4 folders and give varying levels of domain user access to each one
</p>
<br />

<p>
<img src="https://i.imgur.com/RKCtdn3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 2 in Client-1 go to the shared folders section and check to see if the permissions show/ restrict access
</p>

<img src="https://i.imgur.com/YoajKTM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

<p>



<p>
<img src="https://i.imgur.com/BnILVGk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 3 In Active Directory  on DC1 create new Security Group folder and new group Accountants
</p>
<br />

<p>
<img src="https://i.imgur.com/TOxuuM6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 4 navigate to accounting folder and give group accountants read and write access
</p>
<br />

<p>


<p>
<img src="https://i.imgur.com/M4A9aTE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 5 click on accounting folder as normal user verify that access is denied
</p>
<br />

<p>
<img src="https://i.imgur.com/IfqFey2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 6 add normal user to accountants group. logoff and log back in client one and he should now have the correct permissions
</p>
<br />

<p>
























