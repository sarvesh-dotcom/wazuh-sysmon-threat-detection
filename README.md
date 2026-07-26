# wazuh-sysmon-threat-detection

A beginner-friendly cybersecurity home lab demonstrating Windows endpoint monitoring and threat detection using **Wazuh SIEM** and **Microsoft Sysmon**.

This project showcases how Sysmon telemetry is collected by the Wazuh agent, forwarded to the Wazuh Manager, and analyzed through the Wazuh Dashboard to detect common Windows activities and security events.

---

## Project Objectives

- Deploy a Wazuh Manager on Ubuntu
- Install and configure a Wazuh Agent on Windows 11
- Install Sysmon using the SwiftOnSecurity configuration
- Forward Sysmon logs to Wazuh
- Simulate common Windows activities
- Observe and analyze alerts in the Wazuh Dashboard
- Gain hands-on experience with endpoint monitoring and SIEM workflows

---

## Lab Architecture

```text
Windows 11
├── Sysmon
└── Wazuh Agent
        │
        │ Event Logs
        ▼
Ubuntu Server
├── Wazuh Manager
├── Wazuh Indexer
└── Wazuh Dashboard
```

---

## Technologies Used

- Wazuh 4.12
- Ubuntu Server
- Windows 11
- Microsoft Sysmon
- SwiftOnSecurity Sysmon Configuration
- Windows Event Viewer

---

## Detection Scenarios

The following Windows activities were monitored using Sysmon and analyzed in Wazuh:

- Process Creation (Event ID 1)
- PowerShell Execution
- Command Prompt Execution
- User Enumeration (`net user`)
- File Integrity Monitoring (existing Wazuh feature)
- Windows Security and System Events

---

## Repository Structure

```text
wazuh-sysmon-threat-detection/
│
├── README.md
├── LICENSE
│
├── report/
│   └── Wazuh-Sysmon-Threat-Detection-Report.md
│
├── screenshots/
│   ├── architecture.png
│   ├── dashboard-overview.png
│   ├── process-creation.png
│   ├── powershell-alert.png
│   ├── net-user-alert.png
│   └── alert-details.png
│
└── config/
    ├── ossec.conf
    └── sysmonconfig.xml
```

---

## Screenshots

### Wazuh Dashboard

*Add screenshot here*

---

### Process Creation Detection

*Add screenshot here*

---

### PowerShell Detection

*Add screenshot here*

---

### User Enumeration Detection

*Add screenshot here*

---

## Configuration

This repository includes:

- `ossec.conf` (modified Wazuh Agent configuration)
- `sysmonconfig.xml` (Sysmon configuration used for the lab)

---

## Skills Demonstrated

- SIEM Deployment
- Endpoint Monitoring
- Windows Event Logging
- Sysmon Configuration
- Security Event Analysis
- Threat Detection
- Log Collection
- Linux Administration
- Windows Security
- Cybersecurity Home Lab

---

## Learning Outcomes

Through this project I learned how to:

- Deploy and configure a Wazuh SIEM environment
- Collect Windows telemetry using Sysmon
- Configure Wazuh to ingest Sysmon logs
- Analyze endpoint activity in the Wazuh Dashboard
- Investigate security events generated from common Windows commands
- Understand how SIEM solutions collect and correlate endpoint data

---

## Future Improvements

- MITRE ATT&CK mapping
- Custom Wazuh detection rules
- Active Response automation
- Brute-force detection lab
- Sigma rule integration
- Multi-endpoint monitoring

---

## Disclaimer

This project was created for educational purposes in a personal cybersecurity home lab. All activities were performed in an isolated environment on systems owned by the author.

---

## Author

**Sarvesh Khanal**

Aspiring SOC Analyst | Cybersecurity Enthusiast

Feel free to connect or provide feedback!
