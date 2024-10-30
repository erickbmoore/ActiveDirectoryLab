<h1>Active Directory Home Lab</h1>

<h2>Description</h2>

#### Overview
This project involves creating a Virtual Machine (VM) configured as a domain controller, which houses Active Directory. The setup includes establishing a private network for clients and configuring various network services to facilitate connectivity.

#### Steps Completed

1. **Create Virtual Machine as Domain Controller**:
   - Set up a VM to function as the domain controller for Active Directory.

2. **Configure Network Adaptors**:
   - Added two network adaptors: 
     - One for connecting to the external internet.
     - Another for connecting to a VirtualBox private network for client connections.

3. **IP Addressing and Domain Creation**:
   - Assigned IP addressing for the internal network.
   - Named the server and created a domain within Active Directory.

4. **Routing Configuration**:
   - Configured routing to ensure clients on the private network can access the internet through the domain controller.

5. **DHCP Configuration**:
   - Set up DHCP on the domain controller to automatically assign IP addresses to Windows 10 machines on the private network.

6. **Bulk User Creation**:
   - Executed a PowerShell script to automatically create one thousand user accounts in Active Directory.

7. **Client VM Setup**:
   - Created an additional VM named `CLIENT1`, connecting it to the private VirtualBox network.
   - Joined `CLIENT1` to the domain.

8. **Domain Account Login**:
   - Logged into `CLIENT1` using one of the newly created domain accounts.

#### Outcome
This project successfully established a domain controller with Active Directory, implemented DHCP for automated IP assignment, and facilitated client connectivity within a secure private network, enhancing the organizational infrastructure.


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
