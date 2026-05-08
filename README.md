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

<img width="564" height="208" alt="Screenshot 2026-05-08 151523" src="https://github.com/user-attachments/assets/dae454e8-bc9c-40f0-be83-90a78995ad05" />

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

<img width="553" height="157" alt="Screenshot 2026-05-08 150522" src="https://github.com/user-attachments/assets/c0402012-a68e-4ea9-a2ec-070deb4b9822" />
<br>
Figure 3: Fast Nmap scan (-F) on target host

---

