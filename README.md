# azure-network-protocols<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>
<p>

- Create a Resource Group 
- Create Windows 10 Virtual Machine
- Create Linux (Ubauntu) Virtual Machine
- Observe Virtual Machine within Network Watcher 

<p>

</p>
<p>
<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/zPsA6n2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
A Resource Group is a container for Azure resources. It helps you manage and organize your resources.
Go to the Azure portal (https://portal.azure.com/).
Click on "+ Create a resource" button on the left menu.
Select "Resource group" under the "Featured" section.
Enter a unique name for your Resource Group, select a region, and click on "Review + create" button.
Click on "Create" button to create the Resource Group.
</p>
<br />

<p>
<img src="https://i.imgur.com/nLk0aep.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
A Virtual Machine is a computer in the cloud. It runs an operating system and allows you to install and run software.
Go to the Azure portal.
Click on "+ Create a resource" button on the left menu.
Search for "Windows 10 Pro" and select it.
Enter a unique name for your Virtual Machine, select a subscription, and choose your Resource Group.
Choose a username and password for your Virtual Machine.
Under the "Networking" section, select "Create new" for the Virtual Network and Subnet options.
Enter a unique name for your Virtual Network and Subnet, select a region, and click on "Create".
Click on "Review + create" button, and then click on "Create" to create the Windows 10 VM.
</p>
<br />

<p>
<img src="https://i.imgur.com/oE2TKbp.png"80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to the Azure portal.
Click on "+ Create a resource" button on the left menu.
Search for "Ubuntu Server" and select it.
Enter a unique name for your Virtual Machine, select a subscription, and choose your Resource Group.
Choose a username and password for your Virtual Machine.
Under the "Networking" section, select "Use existing" for the Virtual Network and Subnet options.
Select the Virtual Network and Subnet that you created earlier.
Click on "Review + create" button, and then click on "Create" to create the Ubuntu VM.
</p>
<br />

<p>
<img src="https://i.imgur.com/3iFSn8f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Network Watcher is a monitoring and diagnostics service for Azure networking.
Go to the Azure portal.
Search for "Network Watcher" and select it.
Click on "Virtual Network" in the left menu.
Select your Virtual Network from the list.
You can now view the details and status of your Virtual Network, such as its subnets, security groups, and flow logs.  

 <p>
<img src="https://i.imgur.com/GrQNOpk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install Wireshark on your Windows 10 Virtual Machine

Wireshark is a free and open-source network protocol analyzer.
Connect to your Windows 10 Virtual Machine using Remote Desktop.
Download Wireshark from https://www.wireshark.org/.
Install Wireshark on your Windows 10 Virtual Machine.  
