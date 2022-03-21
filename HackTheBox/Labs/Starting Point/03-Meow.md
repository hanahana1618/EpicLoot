Initial Enum
nmap -sV {targetIP}
sudo nmap -sV 10.129.4.12
Starting Nmap 7.92 ( https://nmap.org ) at 2022-03-21 23:30 GMT
Nmap scan report for 10.129.4.12
Host is up (0.086s latency).
Not shown: 999 closed tcp ports (reset)
PORT   STATE SERVICE VERSION
23/tcp open  telnet  Linux telnetd
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 13.63 seconds


Possible Vulns 
OS: Linux
Anything related to telnet, which is a pretty faulty and old protocol
Found: 	ProFTPd 1.3.2 rc3 < 1.3.3b (Linux) - Telnet IAC Buffer Overflow (Metasploit) in exploit db
searchsploit returned too many results

Exploit
Trying connecting using telnet root and there was no password set :/
After 'ls' the flag was in flag.txt
