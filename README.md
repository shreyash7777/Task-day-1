# Task-day-1
Nmap Recon Summary

Installed Nmap on a Linux system for network scanning.

Identified local IP range: 192.168.1.0/24 using ip a.

Ran a TCP SYN scan: sudo nmap -sS 192.168.1.0/24.

Found active Windows host (192.168.1.9) with ports 135, 139, 445 open (RPC, NetBIOS, SMB).

Ran default SMB vulnerability scripts—some failed due to firewall or SMB version issues.

Captured traffic with Wireshark on eth0.

Used filter ip.addr == 192.168.1.11 to isolate relevant packets.

Saved capture as .pcapng for further analysis.
