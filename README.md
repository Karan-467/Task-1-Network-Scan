\# Task 1 - Scan Your Local Network for Open Ports



\## Objective

To identify active devices and discover open TCP ports on the local network using Nmap.



\## Tools Used

\- Nmap 7.98

\- Windows Command Prompt



\## Command Used



```bash

nmap -sS 172.20.10.0/28

```



\## Scan Results



\### Host: 172.20.10.1



| Port | Service |

|------|---------|

| 21 | FTP |

| 53 | DNS |

| 49152 | Unknown |

| 62078 | iPhone Sync |



\### Host: 172.20.10.2



| Port | Service |

|------|---------|

| 135 | MSRPC |

| 139 | NetBIOS |

| 445 | Microsoft-DS |

| 902 | ISS RealSecure |

| 912 | Apex Mesh |



\## Security Risks



\- FTP can expose files if not secured.

\- SMB (Port 445) is a common attack target.

\- Unnecessary open ports should be closed.

\- Firewalls should be enabled.

\- Systems should be updated regularly.



\## Conclusion



The scan successfully identified two active hosts on the local network and several open TCP ports. Proper firewall configuration and disabling unnecessary services can reduce security risks.

