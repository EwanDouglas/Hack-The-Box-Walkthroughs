# HackTheBox-Meow
A quick guide on the first HTB machine in the starting point path.

My first step in this situation is to ping my target to make sure everything is set up correctly. 

<img src="https://i.imgur.com/tKTIRcI.png" height="80%" width="80%" alt="aaa"/>

Next I will perform a scan with Nmap, the extremely popular network mapping tool. There are so many options for an Nmap scan, but for this one I will use an agressive scan.

<img src="https://i.imgur.com/yi3Esja.png" height="80%" width="80%" alt="aaa"/>

If you ever want to learn more about a tool youu can use the "man {insert tool name}" command, in this case typing "man nmap" into the terminal will give us tons of useful information about the types of services avaliable. Also, when in doubt, the "help" command is invaluable.

<img src="https://i.imgur.com/HousNZG.png" height="80%" width="80%" alt="aaa"/>

During my scan, I see that Telnet is open on port 23. Telnet is an old port that is used to remotely control a computer, perfect for a hacker to exploit. 

<img src="https://i.imgur.com/4SaAdFt.png" height="80%" width="80%" alt="aaa"/>

I open the Telnet connection and see there is a username and password. Sometimes you can get lucky and access a system by using default usernames, such as "root", "admin", or "administrator". After testing the "root" username, we are granted access. It looks like this administrator forgot to configure their login!

<img src="https://i.imgur.com/eby9N6r.png" height="80%" width="80%" alt="aaa"/>

We are now connected remotely via Telnet to our target, we have full root permission and total freedom to capture the flag! 

<img src="https://i.imgur.com/TDb6EDc.png" height="80%" width="80%" alt="aaa"/>
