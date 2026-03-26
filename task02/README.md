# VAPT Week 2 Task

This repository contains the report, screenshots and workflow of the Week 2 VAPT task completed during the internship.

The task was performed in a controlled lab environment using Kali Linux as the attacker machine and Metasploitable2 as the target system.

## Tools Used
- Kali Linux
- Nmap
- Nikto
- theHarvester
- Metasploit Framework
- SHA256 hashing

## Workflow / Steps Performed

1. First, a network scan was performed using Nmap to identify open ports and services running on the target machine.

2. After identifying the services, a web vulnerability scan was conducted using Nikto to check for possible web server vulnerabilities.

3. Reconnaissance was performed using theHarvester to gather publicly available information related to the target.

4. From the Nmap scan results, the IRC service running on port 6667 was identified as potentially vulnerable.

5. The vulnerability was exploited using the Metasploit module for the UnrealIRCd backdoor.

6. After successful exploitation, a reverse shell session was obtained on the target machine.

7. Post-exploitation enumeration was performed using commands like `id`, `uname -a`, `cat /etc/passwd`, and `ps aux` to gather system information.

8. As part of evidence collection, a sample file was created and its SHA256 hash was generated to demonstrate file integrity verification.

## Target Machine
Metasploitable2 Virtual Machine

## Attacker Machine
Kali Linux
