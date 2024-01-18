# Creating a Virtual Private Network
<h1>Network Design</h1>

<p align="center">
Topology: <br/>
<img src="https://i.imgur.com/9NbTunt.png" height="80%" width="80%" alt="Virtual Cloud Network"/>

<br />
<br />

<h2>Description</h2>
In this Project I designed and set up a virtual private cloud network utilizing Microsoft Azure Services. This Network is secured by firewall and contains a Virtual Machine acting as a jumpbox that connects to 2 other Virtual Machines acting as Servers (Web-1 & Web-2) through SSH.  

<h2>Languages and Utilities Used</h2>

- <b>Linux</b> 
- <b>Microsoft Azure services</b>
- <b>Terminal<b>
- <b>Draw.io<b>

<h2>Environments Used </h2>

- <b>Mac OS</b>

<h2>Project walk-through:</h2>  

First I established a Resource Group, and created a network security group (King Security) with rule to block all connections to protect the virtual network. 

<p align="center">
Creating Resource Group: <br/>
<img src="https://i.imgur.com/YJ8gaVh.png" height="80%" width="80%" alt="Create a Resource"/>

<br />
<br />


Secondly I used Terminal to generate public SSH Key.

<p align="center">
Generating SSH Key: <br/>
<img src="https://i.imgur.com/kyMKdGE.png" height="80%" width="80%" alt="SSH"/>

<br />
<br />



Next I proceeded to deploy a virtual machine (Jumpbox) to the cloud network.

<p align="center">
Jumpbox Creation: <br/>
<img src="https://i.imgur.com/8AQhVyA.png" height="80%" width="80%" alt="SSH"/>

<br />
<br />




After that I created 2 Virtual Machines to act as web servers (Web 1 & Web 2) that connect to the Jumpbox by SSH. 


<p align="center">
Server Creation: <br/>
<img src="https://i.imgur.com/4NkFxJz.png" height="80%" width="80%" alt="SSH"/>

<br />
<br />


To allow Jumpbox to connect to Web-1 and Web-2 Virtual Machines, I added a security group rule that allows SSH connections only from my current IP.


<p align="center">
SSH Security Rule: <br/>
<img src="https://i.imgur.com/9grLrCz.png" height="80%" width="80%" alt="SSH"/>

<br />
<br />


In order to manage Servers effectively I SSHed into the Jumpbox and proceeded to install docker and pull container.


<p align="center">
Install Docker: <br/>
<img src="https://i.imgur.com/vfN5yKw.png" height="80%" width="80%" alt="SSH"/>

<br />
<br />


<p align="center">
Pulling Container: <br/>
<img src="https://i.imgur.com/QnnWfZL.png" height="80%" width="80%" alt="SSH"/>

<br />
<br />


Lastly I ran container to verify everything was set up properly.


<p align="center">
Running container: <br/>
<img src="https://i.imgur.com/fkQgAVO.png" height="80%" width="80%" alt="SSH"/>

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
