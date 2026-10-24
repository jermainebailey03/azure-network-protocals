<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Network Protocols </h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />





<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 11
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Step 1
- Step 2
- Step 3
- Step 4

<h2>Actions and Observations</h2>

<p>
<img width="1454" height="947" alt="Screenshot_23-10-2026_192041_coursecareers com" src="https://github.com/user-attachments/assets/c325b050-e654-495b-b3fe-801db2e50a7d" />


</p>
<p>
In this Lab, a Firewall needed to be Configured in Network Security Group. A perpetual/non-stop ping had to be Initiated from Windows 11 VM to the Ubuntu VM. Next step was to open the Network Security Group on the Ubuntu VM and disable incoming (inbound) ICMP traffic. Back in the Windows 11 VM, ICMP traffic was observed in Wireshark and the command line Ping activity. Next step was to Re-enable ICMP traffic for the Network Security Group that Ubuntu VM is using. Back in Windows 11 VM, ICMP traffic was observed in Wireshark and the command line activity to make sure it was configured correctly.
</p>
<br />

<p>
<img width="1603" height="919" alt="Screenshot_4-9-2026_185659_coursecareers com" src="https://github.com/user-attachments/assets/76c9188e-23d9-4338-a7d0-f92a9cad693f" />


</p>
<p>
A Windows 11 VM was created as well as a Resource Group needed to be Configured. The next step, was to create a Virtual Network, Subnet and a Linux (Unbuntu) VM. Remote Desktop was used to connect to Windows 11 VM, but within Windows 11 VM, Wire Shark needed to be installed. Wire Shark was opened and a filter for ICMP traffic only was configured. The next step was to retrieve the IPaddress of the Unbutu VM and ping it from the Windows 11 VM. The ping was observed and the replies and request within Wire Shark were observed. In conclusion, from a Windows 11 VM using Powershell, it was opened and a ping to a public website was open and observed traffic within Wire Shark.  
</p>
<br />

<p>
<img width="1660" height="936" alt="Screenshot_23-10-2026_194838_coursecareers com" src="https://github.com/user-attachments/assets/fe178a8a-1585-4fbc-90c5-44167fb0abb1" />

</p>
<p>
In this Lab SSH traffic was observed inside Wireshark, filtering for SSH traffic only inside the command line. From Windows 11 VM , "SSH into"  was placed into the Ubuntu Virtual Machine (via its private IP address). Next step was to type commands (username, pwd, ect) into the Linux SSH connection and observe SSH traffic spam in Wireshark on the back end. 
</p>
<br />
