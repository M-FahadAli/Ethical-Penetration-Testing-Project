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
Execute the command `msfconsole` to launch the Metasploit Framework. This powerful tool provides a platform for conducting various penetration testing activities, including vulnerability scanning, exploit development, and post-exploitation tasks: <br/>
<img src="https://img.hotimg.com/Screenshot-2024-02-21-204809.png" alt="Screenshot-2024-02-21-204809.png" border="0" />
<br />
<br />
Copy the version number: <br/>
<img src="https://img.hotimg.com/Screenshot-2024-02-21-205523.png" alt="Screenshot-2024-02-21-205523.png" border="0" />
<br />
<br />
In the Metasploit console (`msfconsole`), enter the `search` command followed by the version number obtained from the Nmap scan results. This will filter the available modules to find any exploits targeting the specific version of the service or software identified on the target machine: <br/>
<img src="https://img.hotimg.com/Screenshot-2024-02-21-2154166baa727eca76e97e.png" alt="Screenshot-2024-02-21-2154166baa727eca76e97e.png" border="0" />
<br />
<br />
After identifying the appropriate exploit module from the search results, utilize the `use` command followed by the corresponding module number to select the desired vulnerability. If the desired module is listed as the first result, you can simply use `use 0` to select it: <br/>
<img src="https://img.hotimg.com/Screenshot-2024-02-21-210041.png" alt="Screenshot-2024-02-21-210041.png" border="0" />
<br />
<br />
 After selecting the exploit module, use the `show options` command to display the list of configurable options for the chosen module. Among these options, you'll typically find `RHOSTS`, which represents the target host's IP address. Set this option by typing `set rhosts` followed by the victim's IP address. This ensures that the exploit is targeted at the correct machine: <br/>
<img src="https://img.hotimg.com/Screenshot-2024-02-21-210342.png" alt="Screenshot-2024-02-21-210342.png" border="0" />
 <br />
<br />
 After configuring the exploit module with the appropriate options, simply type the `exploit` command to execute the attack. If successful, you will see a message indicating "Command shell session 1 opened," confirming that the exploit has been successful, and a command shell session has been established on the victim machine. This signifies the completion of the attack: <br/> 
 <img src="https://img.hotimg.com/Screenshot-2024-02-21-210507.png" alt="Screenshot-2024-02-21-210507.png" border="0" />
 <br/>
 <br/>
In conclusion, this project has provided practical insights into penetration testing methodologies within a virtual environment. By conducting Nmap scans, utilizing the Metasploit Framework, and establishing command shell sessions, we've explored fundamental techniques used in cybersecurity. Through this hands-on approach, we've gained valuable experience in identifying and mitigating vulnerabilities, ultimately contributing to a better understanding of network security principles: <br/>
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
