<h1>Ethical Penetration Testing Project</h1>
<img src="https://img.hotimg.com/1_eb5oE6h-djckn-zp_O1Gvw.png" alt="1_eb5oE6h-djckn-zp_O1Gvw.png" border="0" />
<h2>Description</h2>
In this project, we delve into the realm of cybersecurity by setting up a virtual environment to explore penetration testing techniques. 
<br />

<h2>Environments Used </h2>

- <b>Kali Linux</b> 
- <b>Metasploitable</b>

<h2>Program walk-through:</h2>
<p align="center">
Initiate the virtual machines running Kali Linux and Metasploitable to establish our simulated network environment. By launching both the Kali Linux VM, equipped with a plethora of penetration testing tools, and the Metasploitable VM, designed to be vulnerable to various exploits, we create a dynamic platform for exploring cybersecurity concepts and conducting hands-on exercises in penetration testing and vulnerability assessment: <br/>
<img src="https://img.hotimg.com/Screenshot-2024-02-21-203448.png" alt="Screenshot-2024-02-21-203448.png" border="0" />
<br />
<br />
First, identify the victim machine's IP address using the 'ip a' command. Then, on the attacker machine, use the ping command followed by the victim's IP address to verify connectivity between the two. This ensures that both machines are connected: <br/>
<img src="https://img.hotimg.com/Screenshot-2024-02-21-203751.png" alt="Screenshot-2024-02-21-203751.png" border="0" />
<br />
<br />
Perform an Nmap scan with the options '-sC' for script scanning (which checks for vulnerabilities on the server) and '-sV' to retrieve version information for the scanned ports. Specify the target machine's IP address as the argument for the scan. This comprehensive scan will help identify potential vulnerabilities and provide insights into the services running on the target machine: <br/>
<img src="https://img.hotimg.com/Screenshot-2024-02-21-204408.png" alt="Screenshot-2024-02-21-204408.png" border="0" />
<br />
<br />
Execute the command `msfconsole` to launch the Metasploit Framework. This powerful tool provides a platform for conducting various penetration testing activities, including vulnerability scanning, exploit development, and post-exploitation tasks. <br/>
<img src="https://img.hotimg.com/Screenshot-2024-02-21-204809.png" alt="Screenshot-2024-02-21-204809.png" border="0" />
<br />
<br />
Copy the version number: <br/>
<img src="https://img.hotimg.com/Screenshot-2024-02-21-205523.png" alt="Screenshot-2024-02-21-205523.png" border="0" />
<br />
<br />
Sanitization complete:  <br/>
<img src="https://imgur.com/WO3XErP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
