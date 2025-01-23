# SOC-Lab-Simulation-Detection

## Overview
This lab project is based on Eric Capuano's blog series, *"So You Want to Be a SOC Analyst?"*. The lab replicates real-world scenarios in a controlled environment to enhance my skills in adversary simulation, threat detection, and incident response. Using tools like Sliver C2 and LimaCharlie, I conducted hands-on experiments to understand the behavior of attackers and craft detection rules to mitigate potential threats.

---

## Objectives
- Simulate adversarial activities to understand common tactics, techniques, and procedures (TTPs).
- Configure and monitor a secure virtualized environment.
- Craft and test custom detection rules using YARA and LimaCharlie.
- Analyze telemetry data to detect and respond to malicious activities.
- Automate threat detection and improve response time.

---

## Lab Environment

### Virtualization Setup
- **VMware Workstation Pro**: Managed two virtual machines.
  - **Windows 11 Development VM**: Used as the victim machine.
  - **Ubuntu Server 22.04.1**: Set up as the attacker machine hosting the Sliver C2 server.

### Network Configuration
- Configured static IPs on the Linux VM to ensure consistent connectivity.
- Used NAT networking for seamless communication between the virtual machines.

---

## Skills Gained
- **SIEM Implementation and Log Analysis**: Configured and analyzed logs using LimaCharlie EDR.
- **Network Traffic Monitoring and Attack Detection**: Monitored malicious activity using telemetry and process tracking tools.
- **Security Automation**: Developed YARA rules to automate detection and response workflows.
- **Incident Response and Threat Mitigation**: Simulated adversarial behaviors and responded with tailored detections.
- **Adversary Simulation**: Used Sliver C2 to generate and execute payloads, mimicking real-world attack scenarios.

---

## Tools Used

### Virtualization and Infrastructure
- **VMware Workstation Pro**: Managed virtual machines.
- **Ubuntu Server 22.04.1**: Hosted attacker tools and command-and-control (C2) framework.
- **Windows 10 Development VM**: Configured for telemetry collection and detection rule testing.

### Endpoint Detection and Response (EDR)
- **LimaCharlie**: Real-time telemetry and detection rule management.
- **Sysmon**: Captured detailed event logs for process, network, and file activity.
- **YARA**: Developed detection rules for malware and malicious processes.

### Adversary Simulation
- **Sliver C2**: Simulated command-and-control activities.
- **Mingw-w64**: Compiled tools for adversarial testing.

### Log Analysis and Forensics
- **LimaCharlie Timeline**: Analyzed system events in near real-time.
- **Artifact Collection**: Gathered and reviewed Sysmon and other logs.

### Automation and Scripting
- **PowerShell**: Automated administrative tasks and simulated attacker actions.
- **Python HTTP Server**: Delivered payloads between the attacker and victim systems.

---

## Key Projects

### 1. Adversary Simulation with Sliver C2
- **Objective**: Simulate a C2 attack and analyze the telemetry.
- **Process**:
  - Generated a C2 payload on the Ubuntu VM.
  - Delivered the payload to the Windows VM using Python HTTP Server.
  - Observed malicious behaviors in LimaCharlie and crafted detection rules.

### 2. Automated Threat Detection with YARA
- **Objective**: Detect malicious files and processes automatically.
- **Process**:
  - Created YARA rules to scan for known patterns in Sliver payloads.
  - Integrated YARA with LimaCharlie for real-time detection.
  - Tested the rules against the deployed payloads.

### 3. Custom Detection Rules with LimaCharlie
- **Objective**: Build and test detection and response rules.
- **Process**:
  - Monitored process telemetry to identify suspicious behaviors (e.g., LSASS memory dumps, Volume Shadow Copy deletions).
  - Created D&R rules to detect and block these activities in real time.

### 4. Incident Response Simulation
- **Objective**: Practice responding to adversarial activities.
- **Process**:
  - Simulated credential dumping and network exploitation.
  - Investigated alerts and developed strategies to mitigate future threats.

---

## Steps & Screenshots
Comming Soon

---

## Results
- Successfully configured a functional lab environment that mimics a real-world SOC.
- Developed and tested detection rules that identified malicious activity with high accuracy.
- Gained practical experience in endpoint monitoring, adversary simulation, and incident response.
- Enhanced skills in automating detection processes and writing robust YARA rules.

---

## Future Enhancements
- Expand the lab by introducing additional virtual machines for lateral movement simulations.
- Integrate a SIEM platform for more comprehensive log analysis.
- Experiment with additional EDR tools for broader detection coverage.

---

## Acknowledgments
This lab was inspired by Eric Capuano's SOC training blog series, *"So You Want to Be a SOC Analyst?"*. Special thanks to the open-source tools and platforms that made this project possible.

---

## Contact
Feel free to reach out with questions or feedback!

<a href="https://github.com/philigator/"><img src="https://img.shields.io/badge/-GitHub-181717?&style=for-the-badge&logo=github&logoColor=white" /></a>
<a href="https://linkedin.com/in/philipabryant/"><img src="https://img.shields.io/badge/-LinkedIn-0072b1?&style=for-the-badge&logo=linkedin&logoColor=white" /></a>
