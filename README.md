# Creating a Virtual Private Network
<h1>Network Design</h1>

<p align="center">
Topology: <br/>
<img src="https://i.imgur.com/9NbTunt.png" height="80%" width="80%" alt="Virtual Cloud Network"/>

<br />
<br />

<h2>Description</h2>
In this Project I designed and set up a virtual private cloud network utilizing Microsoft Azure Services. This Network is secured by firewall and contains a Virtual Machine acting as a jumpbox that connects to 2 other virtual machines (Web-1 & Web-2) through SSH.  

<h2>Languages and Utilities Used</h2>

- <b>Linux</b> 
- <b>Microsoft Azure services</b>
- <b>Terminal<b>

<h2>Environments Used </h2>

- <b>Mac OS</b>

<h2>Program walk-through:</h2>  

First I established a Resource Group, and created a network security group (King Security) to protect the virtual network. After that I proceeded to deploy a virtual machine (Jumpbox) to the cloud network.








Then I created 2 Virtual Machines (Web 1 & Web 2) to connect to the Jumpbox by SSH.







Install and run containers using Docker.
Set up Ansible connections to VMs inside your VNet.
Write Ansible playbooks to configure VMs.
Create a load balancer on the Azure platform.
Create firewall and load balancer rules to allow traffic to the correct virtual machines.

Virtual Networking: In this activity, you will set up a resource group and a cloud network using the Azure Portal.
Security Groups: In this activity, you will create a network security group to control access to any resources in the subnet that you created in the last activity.
Virtual Computing: In this activity, you will set up the first three virtual machines inside your cloud network, protected by your network security group. You will use one of these machines as a jump box to access your cloud network, and the other machines will be web servers. 

Cloud Architecture: In this option, you'll choose the best network options for each of several scenarios.
Jump Box Administration: In this activity, you will configure a virtual machine on your network as a jump box that you will connect to and use to configure other machines that will be added to the network. You will need to create a security group rule to allow SSH connections only from your current IP address and connect to your new virtual machine for management.
Containers: In this activity, you will configure your jump box to run Docker containers and then install a container.
Provisioners: In this activity, you will launch a new VM from the Azure portal that can only be accessed using a new SSH key from the container running inside your jump box.
Ansible Playbooks: In this activity, you will create an Ansible playbook that installs Docker and configures a VM with the DVWA web app.
Load Balancing: In this activity, you will install a load balancer in front of the VM to distribute the traffic across more than one VM.
Security Configuration: In this activity, you'll configure the load balancer and security group to work together to expose port 80 of the VM to your Home IP address.
<br />






<h2>Program walk-through:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
