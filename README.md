# Wazuh SOC Home Lab

## Project Overview

This project demonstrates the deployment of a Security Operations Center (SOC) home lab using Wazuh on Ubuntu and a Windows 11 endpoint. The objective was to simulate real-world cyber attack techniques, detect them using Wazuh, and investigate the generated alerts.

The lab was built to gain hands-on experience with Security Information and Event Management (SIEM), Windows event logging, Sysmon, threat hunting, and incident investigation.

---

## Project Objectives

- Deploy a Wazuh SIEM environment
- Connect a Windows 11 endpoint to Wazuh
- Install and configure Sysmon
- Simulate attacker techniques based on the MITRE ATT&CK framework
- Detect and investigate security events
- Develop practical SOC analyst skills

---

## Lab Architecture

```
Windows 11 Endpoint
        │
        │
   Wazuh Agent
        │
        │
Ubuntu Server
        │
        │
 Wazuh Manager
        │
        │
Wazuh Dashboard
```

---

## Technologies Used

- Wazuh SIEM
- Ubuntu Linux
- Windows 11
- Sysmon
- PowerShell
- Windows Event Viewer
- MITRE ATT&CK Framework

---

## Skills Demonstrated

- SIEM Deployment
- Wazuh Configuration
- Windows Security Monitoring
- Sysmon Deployment
- Threat Hunting
- Incident Investigation
- File Integrity Monitoring (FIM)
- Registry Monitoring
- Windows Event Log Analysis
- MITRE ATT&CK Mapping

---

# Attack Simulations

| Exercise | MITRE ATT&CK Technique | Status |
|-----------|------------------------|--------|
| Discovery | T1087, T1033 | Done |
| Failed Login Detection | Authentication | Done |
| PowerShell Execution | T1059 | Done |
| File Integrity Monitoring | FIM | Done |
| Registry Persistence | T1547 | Done |
| Administrator Group Modification | T1098 | Done |
| Scheduled Task Persistence | T1053 | Done |

---

## What I Learned

During this project I learned:

- How a SIEM collects and analyzes security logs.
- How Wazuh agents communicate with the Wazuh manager.
- How Sysmon enhances Windows event logging.
- How to investigate alerts using Wazuh Threat Hunting.
- How Windows Event Logs and Sysmon logs work together.
- How to map security events to the MITRE ATT&CK framework.
- The importance of file integrity monitoring and registry monitoring.
- That not every Windows event automatically generates a Wazuh alert; detections depend on Sysmon configuration and Wazuh rules.

---

## Challenges Faced

During this project I encountered several challenges, including:

- Reinstalling and reconnecting the Wazuh agent after configuration issues.
- Troubleshooting missing Sysmon process creation events.
- Configuring File Integrity Monitoring for custom directories.
- Understanding why some commands (such as `certutil`) generated Windows events but did not produce Wazuh alerts.
- Learning the relationship between Windows logs, Sysmon, and Wazuh detection rules.

Resolving these issues improved my troubleshooting and security monitoring skills.

---

## Screenshots

The `screenshots` folder contains images of:

- Wazuh Dashboard
- Threat Hunting
- Discovery Alert
- PowerShell Alert
- File Integrity Monitoring Alert
- Registry Persistence Alert
- Administrator Group Modification Alert
- Scheduled Task Alert

---

## Repository Structure

```
Wazuh-SOC-Home-Lab/
│
├── README.md
├── docs/
├── attack-simulations/
├── screenshots/
└── sysmon/
```

---

## Future Improvements

- Add Active Directory integration
- Build a multi-endpoint SOC lab
- Create custom Wazuh detection rules
- Develop custom Sysmon configurations
- Simulate additional MITRE ATT&CK techniques
- Integrate threat intelligence feeds

---

## Author

**Hafsah Yasir**

Cybersecurity Student

This project was created as part of my hands-on cybersecurity learning journey to develop practical SOC Analyst skills.
