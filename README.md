<h1>Active Directory Home Lab</h1>

<h2>Description</h2>
For this project, I created an Active Directory Home Lab environment using Oracle Virtual Box.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Server 2019 </b>

<h2>Program walk-through:</h2>

<p align="center">

<img src="https://i.imgur.com/DY1Z6H2.png" height="80%" width="80%" />
<br />
<br />







1. **Installing VirtualBox and Obtaining ISO Files**: Download and install Oracle VirtualBox. Obtain the Windows Server 2019 and Windows 10 ISO files for creating virtual machines (VMs). 

2. **Creating the Domain Controller VM**: Set up a VM for Windows Server 2019, configuring two network adapters—one set to NAT for internet access and another to Internal Network for internal communication. 
   <br />
   <img src= "https://i.imgur.com/3mWEY0V.png" height="80%" width="80%"/>
   <img src= "https://i.imgur.com/qN9cHFX.png" height="80%" width="80%"/>
   <br />
   <br />
   <br />
3. **Installing and Configuring Active Directory**: Install the Active Directory Domain Services (AD DS) role on the Windows Server 2019 VM, promote it to a domain controller, and create a new domain. 

4. **Setting Up Routing and Remote Access**: Configure the Routing and Remote Access role to enable Network Address Translation (NAT), allowing client machines on the internal network to access the internet through the domain controller.

5. **Configuring DHCP**: Install and configure the Dynamic Host Configuration Protocol (DHCP) role on the domain controller to assign IP addresses to client machines automatically. 

6. **Automating User Account Creation with PowerShell**: Use a PowerShell script to create multiple user accounts in Active Directory, streamlining the process of populating the domain with users.

<img src="https://github.com/user-attachments/assets/5590e9b5-47e7-4f98-ad11-d6325ad78c8c" height="80%" width="80%" />
<br />

7. **Setting Up a Windows 10 Client VM**: Create a Windows 10 VM, configure its network settings to connect to the internal network, and join it to the newly created domain. 

8. **Verifying Domain Functionality**: Log in to the Windows 10 client using one of the domain user accounts to confirm successful integration and functionality of the Active Directory environment. 


</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
