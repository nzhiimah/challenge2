# Challenge 2 - Fast Nmap Scan

## Objective :

- To identify active hosts in the network
- To perform a fast port scan using Nmap
- To analyse basic network accessibility of the target system

### Tools Used:

| Tool       | Purpose                             |
| ---------- | ----------------------------------- |
| Nmap       | Network scanning and host discovery |
| Kali Linux | Penetration testing environment     |

### Steps:

1. Network Discovery (Identify live hosts)

Command used:
```
nmap -sn 192.168.83.0/24
```
Functions:
- Scans the network range
- Detects which devices are online (without scanning ports)

<img width="576" height="209" alt="Screenshot 2026-05-08 150504" src="https://github.com/user-attachments/assets/80c03dd2-919b-4ca0-a437-9f2450dc6835" />
<br>
Figure 1: Host discovery using Nmap (-sn scan)

---
2. Target Identification

From the scan results:

- ```192.168.83.128``` was selected as the target host
- It is the only non-network infrastructure machine

<img width="576" height="209" alt="Screenshot 2026-05-08 150504" src="https://github.com/user-attachments/assets/a6e88736-b364-42dd-8ced-5e6c8bc7f415" />
<br>

---
3. Fast Port Scan (Challenge requirement)

Command used:
```
nmap -F 192.168.83.128
```

Functions:
- Scans the top 100 commonly used ports
- Provides quick overview of open/filtered ports
