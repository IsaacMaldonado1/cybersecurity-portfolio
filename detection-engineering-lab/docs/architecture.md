# Lab Architecture

## Current design
- **Host:** Ubuntu Linux 24.04 LTS running QEMU/KVM through libvirt and Virtual Machine Manager.
- **Windows endpoint:** Windows 11 VM used to generate and collect endpoint telemetry.
- **Kali Linux:** Separate VM for controlled security testing against lab assets.

## Planned detection stack
- **Sysmon:** Detailed Windows process, network, and other system telemetry.
- **Wazuh:** Centralized endpoint monitoring and event analysis.
- **Sigma:** Portable detection-rule format; rules will be tested against the available event data and converted/adapted for the chosen backend as needed.
- **MITRE ATT&CK:** Technique mapping for relevant tests and detections.

## Network and safety
The Windows VM currently uses the default libvirt NAT network. Confirm the final network topology and isolation before running simulations. Only test systems owned by the lab. Do not run destructive or uncontrolled activity.

## Data flow (target)
1. Generate a benign, controlled test action on the Windows endpoint.
2. Collect relevant telemetry with Sysmon.
3. Forward and analyze events in Wazuh or the selected log platform.
4. Write and validate a detection, document false positives and limitations, and map it to ATT&CK.
5. Save sanitized evidence and an investigation report in this repository.
