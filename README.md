# Metasploit-for-reconnaissance
## Metasploit for reconnaissance in pentesting

## AIM:
To get introduced to Metasploit Framework and to perform reconnaissance in pentesting .

## DESIGN STEPS:
Step 1:
Install kali linux either in partition or virtual box or in live mode

Step 2:
Investigate on the various categories of tools as follows:

Step 3:
Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:
Find out the ip address of the attackers system

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/d35e863c-0d73-4e4c-8b6a-198974027eb8)

Invoke msfconsole

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/0338e438-a2a1-4abb-b1c5-2ccc9c3e3bd2)

Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/816708e2-64ab-407d-8cd2-32d20e9ae8e5)

### Port scanning:
msf > nmap -sT 192.168.1810/24-p1-1000

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/0b29f637-0b74-4f36-b09c-00b1072bca60)

msf > db_nmap 192.168.181.0/24

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/d6b3d490-6ba6-4c04-9a43-a9495976aedb)

kali > ls-l

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/d53b759d-1cfc-46ff-8c3e-b90d00086364)

search

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/3afe0b00-d9e0-444b-9201-3f59dd272ad8)

info

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/2b0ebfe4-f06a-4449-aaab-d8237d488c06)

### MYSQL ENUMERATION
db_nmap -sV -sC -p 3306 <metasploitable_ip_address>

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/6253bd66-296c-4379-a576-6ebd64d72e47)

search

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/cfc37b9d-a150-4f43-9cf5-e25f4152007a)

use 11 Or: use auxiliary/scanner/mysql/mysql_version

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/cbb3b647-f45e-4e32-b17c-1f5e77bebe1c)

Use the set rhosts command to set the parameter and run the module, as follows:

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/7f3ae6d5-b0d0-4a37-8450-d7053d30732e)

After scanning, you can also brute force MySQL root account via Metasploit's auxiliary(scanner/mysql/mysql_login) module

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/12e1d68a-f819-4b45-aba7-c00bca5a1158)

/usr/share/wordlists: set PASS_FILE /usr/share/wordlistss/rockyou.txt

![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/82378a27-8d40-4601-a53d-a202948e17e9)
![image](https://github.com/Yamunaasri/Metasploit-for-reconnaissance/assets/115707860/435cc73a-61de-453b-90d7-1db5f7357f47)


## RESULT:
The Metasploit framework for reconnaissance is examined successfully.
