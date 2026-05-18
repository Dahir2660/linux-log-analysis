# Linux Log Analysis & SSH Brute-Force Detection Lab

## Overview
This project demonstrates Linux authentication log analysis and SSH brute-force detection techniques using common cybersecurity tools and Linux commands.

## Objectives
- Analyze Linux authentication logs
- Detect failed and successful SSH login attempts
- Identify suspicious login behavior
- Simulate brute-force attacks
- Understand basic incident detection and response

## Tools Used
- Kali Linux
- journalctl
- Hydra
- fail2ban
- OpenSSH
- Wireshark
- Nmap

## Skills Demonstrated
- Linux administration
- Log analysis
- Threat detection
- SSH security
- Network analysis
- Incident investigation

## Lab Activities
### Authentication Log Analysis
Used journalctl commands to identify:
- Failed SSH logins
- Successful SSH logins
- Source IP addresses
- Suspicious authentication activity

### SSH Brute-Force Simulation
Simulated SSH brute-force attacks using Hydra against a Linux VM in a controlled lab environment.

### Fail2ban Configuration
Configured fail2ban to automatically detect and block repeated failed login attempts.

## Sample Commands
```bash
sudo journalctl | grep "Failed password"

sudo journalctl | grep "Accepted password"

hydra -l kali -P passwords.txt ssh://127.0.0.1

nmap -sV 127.0.0.1
```

## Key Takeaways
This lab improved my understanding of Linux security monitoring, authentication logs, brute-force detection, and basic defensive security practices used in SOC environments.
