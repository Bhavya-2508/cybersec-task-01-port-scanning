<<<<<<< HEAD
#Task 01: Port Scanning on Local Network

Date:23rd June 2025  
Objective:Perform a TCP SYN scan using Nmap to identify open ports on devices within the local network.

---

#Tools Used

Nmap (Version 7.97, Windows)

---

#IP Range Scanned

Target IP Range:'192.168.0.0/24'  
This was based on my IPv4 address 192.168.0.105 with subnet mask 255.255.255.0.

---

#Commands Used

nmap -sS 192.168.0.0/24 -oN scan_results.txt

----------------------------------------------------------------------------------------------------
nmap -sS 192.168.0.0/24 -oN scan_results.txt
. -sS → TCP SYN scan (stealthy, fast, widely used)
. -oN → Save output to normal format text file

---

#Common Services Running
Port 80 (HTTP): Used for unsecured web traffic

Port 443 (HTTPS): Secured version of HTTP using SSL/TLS

Port 8080 (HTTP-Proxy): Often used for alternate web interfaces or proxy services

---

#Potential Security Risks
Port 80: No encryption; data can be sniffed by attackers

Port 443: Secure, but may still be misconfigured or use outdated certificates

Port 8080: Frequently runs admin panels or proxies — often overlooked in security hardening

If these ports are exposed to the internet:

 . Attackers may probe web apps for vulnerabilities

 . Man-in-the-middle attacks may occur on unencrypted ports

 . Outdated web services may be exploited via known CVEs

---

#Key Learnings
Understood how to use Nmap for basic reconnaissance

Learned how TCP SYN scans discover open ports without full connections

Discovered how networks may block ping/ARP scans, affecting Nmap results

---
=======
# cybersec-task-01-port-scanning
Scanning local network for open ports using Nmap (Elevate Labs Cybersecurity Internship Task 01)
>>>>>>> 4b3cf8c23a542e8287c91e79d77321c75f4b05a7
