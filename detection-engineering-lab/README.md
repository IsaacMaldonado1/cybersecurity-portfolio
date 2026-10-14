# Detection Engineering Lab

## Overview

A hands-on cybersecurity lab focused on Windows endpoint monitoring,
security event analysis, SIEM operations, and detection engineering.

This repository documents the lab environment, configurations,
detection rules, controlled security tests, and investigation findings.

## Lab Environment

| Component | Technology |
|---|---|
| Host Operating System | Ubuntu 24.04 LTS |
| Virtualization | QEMU/KVM with Virtual Machine Manager |
| Security Testing VM | Kali Linux |
| Monitored Endpoint | Windows 11 |
| Endpoint Telemetry | Sysmon |
| Security Monitoring | Wazuh |
| Detection Rules | Sigma |
| Attack Framework | MITRE ATT&CK |
| Version Control | Git and GitHub |

## Project Status

- [x] Set up Ubuntu host environment
- [x] Install Kali Linux virtual machine
- [x] Install Windows 11 virtual machine
- [ ] Configure lab networking
- [ ] Install and configure Sysmon
- [ ] Configure Wazuh monitoring
- [ ] Collect and analyze Windows events
- [ ] Create and test Sigma detection rules
- [ ] Conduct controlled security simulations
- [ ] Document investigations and findings

## Repository Structure

```text
detection-engineering-lab/
├── README.md
├── docs/
├── setup/
├── detections/
├── attack-scenarios/
├── investigations/
└── screenshots/
