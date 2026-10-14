# Detection Engineering Lab

## Overview

A hands-on blue-team cybersecurity lab focused on Windows endpoint telemetry, security event analysis, SIEM operations, and detection engineering. The goal is to build and validate detections using documented, controlled tests—not to claim tools or detections work before they are verified.

## Lab Environment

| Component | Technology / status |
|---|---|
| Host | Ubuntu Linux 24.04 LTS |
| Virtualization | QEMU/KVM, libvirt, Virtual Machine Manager |
| Security testing VM | Kali Linux (installed; resource allocation to verify) |
| Monitored endpoint | Windows 11 VM (`win11`) |
| Endpoint telemetry | Sysmon (planned) |
| Security monitoring | Wazuh (planned) |
| Detection rules | Sigma (planned; validate against target backend) |
| Technique mapping | MITRE ATT&CK |
| Version control | Git and GitHub |

## Project Status

- [x] Ubuntu host prepared
- [x] Kali Linux VM installed
- [x] Windows 11 VM installed
- [x] Initial project documentation and repository structure created
- [ ] Verify VM configuration and Windows updates
- [ ] Confirm safe lab networking and isolation
- [ ] Install and validate Sysmon
- [ ] Deploy Wazuh and verify endpoint events arrive
- [ ] Create and test detections against collected telemetry
- [ ] Run controlled simulations and record evidence
- [ ] Write investigation reports and document limitations

## Documentation

- [Lab environment](docs/lab-environment.md)
- [Architecture and event flow](docs/architecture.md)
- [Setup instructions](setup/README.md)
- [Detection rules](detections/README.md)
- [Controlled simulations](attack-scenarios/README.md)
- [Investigation reports](investigations/README.md)
- [Screenshots and evidence](screenshots/README.md)

## Repository Structure

```text
detection-engineering-lab/
├── README.md
├── .gitignore
├── docs/
│   ├── architecture.md
│   └── lab-environment.md
├── setup/
│   ├── windows/README.md
│   ├── sysmon/README.md
│   └── wazuh/README.md
├── detections/
├── attack-scenarios/
├── investigations/
└── screenshots/
```

## Safety and Accuracy

All testing is limited to systems owned by this lab. Network isolation must be verified before simulations. Keep credentials, tokens, VM disk images, and raw logs out of Git. Record only verified configuration and results; label planned work as planned.
