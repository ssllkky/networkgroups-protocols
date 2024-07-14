# networkgroups-protocols
<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<!--<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com) -->

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

- Step 1 Create Virtual Machines with appropiate Operating Systems
- Step 2 Login to VM-1 with Windows OS using Remote Helpdesk.
- Step 3 Download Wireshark, run commands and observe the network protocols.
- Step 4 Connect to VM-2 with Ubuntu OS using SSH on VM-1, observe the connection on Wireshark.
- Step 5 Go back into Azure and cleanup (delete the VM's and and resource group)

<h2>Actions and Observations</h2>

<p>
<img height="80%" width="80%" alt="Screenshot 2024-07-11 at 11 06 39 AM" src="https://github.com/user-attachments/assets/cad35b5e-e061-4cdc-8b9f-3b7dc206bfc7">

</p>
<p>
After logging into Azure I created a Resource Group called "Grp" and created two Virtual Machines one with Windows and another with Linux. 
</p>
<br />

<p>
<img width="80%" alt="Screenshot 2024-07-11 at 10 46 05 AM" src="https://github.com/user-attachments/assets/73de2d32-a0f0-4b6a-aa66-adf81dd7d5b4">
</p>
<p>
After the making sure the Virtual Machines were up and running, I opened Microsft Remote Helpdesk and logged into VM-1 with the Windows OS. Then once available I opened the command-line and checked the user and machine I was on.
</p>
<br />

<p>
<img width="80%" alt="Screenshot 2024-07-11 at 10 58 03 AM" src="https://github.com/user-attachments/assets/0611cca2-927e-46b6-b5f4-2f98c62eeb6d">
<img width="80%" alt="Screenshot 2024-07-11 at 11 01 18 AM" src="https://github.com/user-attachments/assets/a83eccf5-a27a-43c2-aea2-301958cd88ad">
<img width="80%" alt="Screenshot 2024-07-11 at 11 14 47 AM" src="https://github.com/user-attachments/assets/d1a21ff4-3a01-4565-981c-57663d88098e">
</p>
<p>
Then I downloaded Wireshark and proceeded to run commands that executed certain network protocols so I could observe them.
</p>
<br />

<p>
<img width="80%" alt="Screenshot 2024-07-11 at 11 13 12 AM" src="https://github.com/user-attachments/assets/f4a3a2f3-7548-4b9e-93d3-29358912b7e4">
</p>
<p>
Once I completed running the previous commands I connected to the other Virtual Machine using the ssh command. Then I checked the user and machine name to verify.
</p>
<br>

<p>
<img width="80%" alt="Screenshot 2024-07-11 at 11 53 27 AM" src="https://github.com/user-attachments/assets/57d1ed8e-ef52-46fc-ab5f-5436e72978ed">
</p>
<p>
To finish up I logged back into Azure and went to Resource Groups. From there I deleted both the Virtual Machines, the related components, and the resouce group entirely.
</p>
