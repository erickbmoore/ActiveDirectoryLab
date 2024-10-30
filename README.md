<h1>Active Directory Home Lab</h1>

Test. Update in progress...

<h2>Description</h2>
Create Virtual Machine as domain controller which will house active directory. Then add two network adaptors which one will be used to connect to the outside internet and the other will be used to connect to the virtual box private network that clients can connect to. Then assign ip addressing for the internal network and name the server and create a domain. Then configure that and routing so that the clients on the private network can reach the internet through the domain controller. Next we are going to set a DHCP on the domain controller so that the windows 10 machine can automatically get an IP address. THen run a powershell script that will automatcally create a thousand users in active directory. then going to create another virtual machine that will be connected to the private virtual box network. It will be named CLIENT1 and join it to the domain. Then we are going to login to it with one of the domain accounts.

<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 

<h2>Environments Used </h2>

- <b>Oracle Virtual Box</b>
- <b>Windows 10 ISO</b>
- <b>Server 2019 ISO</b>

<h2>Program walk-through:</h2>

<p align="center">
Powershell Script Create Users:  <br/>
<img src="https://imgur.com/bufvIEo.png" height="80%" width="80%" alt="Active Directory Home Lab"/>
<br />
<br />
Users Created: <br/>
<img src="https://imgur.com/a6k3cR9.png" height="80%" width="80%" alt="Active Directory Home Lab"/>
<br />
<br />
Client1 Connection to Internal Network with domain account:  <br/>
<img src="https://imgur.com/TEd5Xr1.png" height="80%" width="80%" alt="Active Directory Home Lab"/>
<br />
<br />
Domain Controller Connections:  <br/>
<img src="https://imgur.com/8fNn0kZ.png" height="80%" width="80%" alt="Active Directory Home Lab"/>
<br />
<br />

  
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
