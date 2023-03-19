<h1>Active Directory Home Lab</h1>

<h2>Description</h2>
In this lab I created an Active Directory home lab Environment using Oracle Virtual Box. Configuring and running this lab helped devolop my understanding of how active directory and windows networking works.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Server 2019</b>
<h2>Lab walk-through:</h2>

<p align="center">
After setting up the VM server 2019 in Oracle VM I went and identified the main network and internal network: <br/>
<img src="https://i.imgur.com/A8iMtUH.png" height="80%" width="80%" alt="Internet Identification"/>

<p align="center">
Setting up the IP for the internal network giving the loop back IP for the preferred DNS: <br/>
<img src="https://i.imgur.com/q7qb7ix.png" height="80%" width="80%" alt="I.P. Set up"/>
 
<p align="center">
Setting up Active Directory Domain Role using Server Manager: <br/>
<img src="https://i.imgur.com/VoR0laW.png" height="80%" width="80%" alt="Domain Services"/>
 
<p align="center">
Post deployment configuration - now that the software is installed I went ahead and created the domain: <br/>
<img src="https://i.imgur.com/GwQDmAO.png" height="80%" width="80%" alt="Domain Services"/>

<p align="center">
Using the Windows Adminstation Tools under Active Directory Users and Computers - Created an Organizational Unit in the created Active directory >mydomain.com< named "_ADMINS" so I could set myself up with an admin account within the environment: <br/> 
<img src="https://i.imgur.com/oQenl3r.png" height="80%" width="80%" alt="Admin Creation"/>

 <p align="center">
Configuring and Enabling Routing and Remote Access - installing NAT to connect to the internet on our client side: <br/> 
<img src="https://i.imgur.com/YOKvsgJ.png" height="80%" width="80%" alt="NAT setup"/>

 
<p align="center">
Next I setup a DHCP server on the domain controller:  <br/> 
<img src="https://i.imgur.com/YBoxMZU.png" height="80%" width="80%" alt="DHCP"/>
 
   
<p align="center">
I then set up the DCHP scope so that the client computers on the network get their IP from the network automatically:  <br/> 
<img src="https://i.imgur.com/lh08jo0.png" height="80%" width="80%" alt="DHCP"/>
 
 
 
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
