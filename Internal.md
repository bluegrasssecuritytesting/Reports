# Internal Walk Through

This machine is from Offensive Security's Proving Grounds. The practitioner can expect to hone their skills in:

- Service and port enumeration
- OS Identification
- Vulnerability and exploit research
- Metasploit

## Port Scan
<img width="703" height="588" alt="image" src="https://github.com/user-attachments/assets/d3ecbef9-2d35-4af8-a68b-611989906b98" />
<img width="592" height="362" alt="image" src="https://github.com/user-attachments/assets/99ce9c51-ed8e-4b4f-8220-98ade59e695b" />

**Ports of Interest**
| Service Name | Port Number |
| ------------ | ----------- |
|     SMB      |     445     |

## OS Identification
With SMB enabled, and the allowance of NULL sessions it is very trivial to obtain the OS version with Netexec.

<img width="1580" height="80" alt="image" src="https://github.com/user-attachments/assets/80fb558c-011a-481c-bfbb-eb79a755bf9f" />


## Access

A google search looking for vulnerabilities affecting Windows Server 2008 Standard 6001 Service Pack1 x32 reveals an exploit readily available on Kali through Metasploit. This is about as "Point and click" as we can get in terms of ease of exploitation. 

### MS09-050 Microsoft SRV2.SYS SMB Negotiate ProcessID Function Table Dereference

**Vulnerability Summary**
This is a critical vulnerability (CVE-2009-3103) affecting the Server Message Block (SMB) implementation in the srv2.sys driver for Windows. 

Once you have Metasploit and the appropriate module loaded, you must first set your target and local options as imaged. Once these are set, it is as simple as running the exploit. 

<img width="1419" height="946" alt="image" src="https://github.com/user-attachments/assets/8d60a080-4521-4395-89fb-b13e97fbcac4" />


### Flag

Since this exploit lands us on this box as system, there is nothing further to do but collect your loot. 

<img width="686" height="921" alt="image" src="https://github.com/user-attachments/assets/9d0ef00f-6c86-4097-9b65-099b2f817552" />

