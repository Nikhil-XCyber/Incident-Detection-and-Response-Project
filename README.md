# Incident-Detection-and-Response-Project
Hands-on cybersecurity project utilizing Splunk for SIEM and UFW for defense. I configured Splunk to ingest SSH logs and performed Log Analysis to identify events consistent with a brute-force attack. This detection instantly triggered an automated response that leveraged the victim machine's firewall, UFW, to block the attacker's IP.

##🌟 Summary

Used Splunk for Log Analysis of SSH logs to detect a brute-force attack.

The core of this project was the integration of a SIEM system with a Linux firewall for real-time defense:

SIEM Detection: Splunk was used to monitor SSH authentication logs from a victim server. We used a powerful Splunk Search Processing Language (SPL) rule to identify log patterns consistent with a network brute-force attack.

Automated Defense: The detection instantly triggered an automated script.

Real-Time Mitigation: The script commanded the target machine's firewall, UFW (Uncomplicated Firewall), to insert a new rule and immediately block the attacker's source IP address, thus successfully neutralizing the ongoing threat.

This setup showcases the ability to transition from passive log monitoring to active, automated threat containment.

##🛠️ Key Technologies

SIEM: Splunk Enterprise

Log Source/Victim: Ubuntu Linux

Attacker Tool: Hydra (used for attack simulation)

Targeted Service: SSH (Secure Shell Protocol)

Detection Language: Splunk Search Processing Language (SPL)

Defense Mechanism: UFW (Uncomplicated Firewall)

For a detailed breakdown of the Splunk Search and UFW logic, please see the project_report.md file.
