# Lab 01 — Network Reconnaissance

## Objective
Identify open ports and services on target machine

## Environment
- Attacker: Kali Linux 192.168.4.45
- Target: Metasploitable 2 192.168.4.219

## Command Used
nmap -sV -Pn 192.168.4.219

## Key Findings
- 21/tcp vsftpd 2.3.4 — known backdoor CVE-2011-2523
- 23/tcp telnet — unencrypted protocol
- 1524/tcp bindshell — unauthenticated root shell
- 3306/tcp MySQL — database exposed to network
- (list the rest)

## What I Learned
(write in your own words what each service is
and why it's dangerous)

## Defender Perspective
What would this nmap scan look like in logs?
How would a SOC analyst detect someone 
running this scan?

## References
- CVE-2011-2523 (vsftpd backdoor)
- nmap documentation: nmap.org/docs
