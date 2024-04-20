<h1>Microsoft Azure Sentinel With a Map of Live Cyber Attacks! </h1>

<h2>Description</h2>

-Created a honeypot server On Microsoft Azure to record RDP brute force attempts:

-Crafted a tailored PowerShell script to extract metadata from the Windows Event Viewer using event ID 4425 which contains information such as ip address Failed Login attempts. This script seamlessly forwarded crucial data to a third-party API (http://ipgeolocation.io) for geolocation analysis, enhancing our understanding of potential threats.

-Configured Log Analytics Workspace in Azure to ingest custom logs containing geographic information (latitude, longitude, state/province, and country)

-Configured Custom Fields in Log Analytics Workspace with the intent of mapping geo data in
Azure Sentinel

-Configured Azure Sentinel to display global RDP brute force attacks on world map according to physical location and magnitude of attacks.

<h2>Languages Used</h2>

- <b>PowerShell</b>
- <b>Splunk SPL</b> 

<h2>Technologies Used </h2>

- <b>Windows 10</b> 
- <b>Microsoft Azure</b>
- <b>Microsoft Sentinel</b> 

<h2>Program walk-through:</h2>

<p align="center">
Overview of Azure environment: <br/>
<img src="https://i.imgur.com/yj7748s.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
PowerShell Script:  <br/>
<img src="https://i.imgur.com/RXVmTnq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Custom Fields based on geographic information (lattitude, longitude, stave/province, and country): <br/>
<img src="https://i.imgur.com/QojY7p2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Failed RDP txt file:  <br/>
<img src="https://i.imgur.com/azlY2C4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
PowerShell script automating failed RDP login attempts into a log and exporting it into a txt file:  <br/>
<img src="https://i.imgur.com/X7AhEc7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Map of Live Cyber Attack attempts:  <br/>
<img src="https://i.imgur.com/TqQP7Yg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h2>Conclusion</h2>

The biggest eye opening moment was how quickly the Virtual Machine was attempted to get attacked. Within minutes there were dozens of failed attemps recorded on the log. No matter what type of device it is, you can be a target of opportunity. This lab reenforced the idea of why it is important to use uncommon username and passwords as many of the recorded brute force attempts were common usernames such as "admis", "administrator" and "user" and common passwords such as "password" and "123456". Throughout the course of the project, over 10,000 login attempts from aorund the world were attempted. Furthermore, it stresses how important it is to safeguard your data. In essence, the trifecta of good cloud security practices—vigilance, unique usernames, and robust passwords—acts as a fortress, ensuring that your digital assets remain safe and secure amidst an increasingly complex cyber landscape.


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
