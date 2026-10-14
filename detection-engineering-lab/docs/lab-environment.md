# Lab Environment

## Host
- OS: Ubuntu Linux 24.04 LTS
- Virtualization: QEMU/KVM with libvirt and Virtual Machine Manager
- CPU: AMD Ryzen 5 PRO 4650U (6 cores / 12 threads)
- RAM: 24 GB
- Storage: 512 GB total; check available space before adding more VMs

## Virtual Machines
### Windows 11 endpoint
- VM name: `win11`
- vCPU: 4
- RAM: 8 GiB
- Virtual disk: 80 GiB
- Firmware: UEFI
- TPM: emulated TPM 2.0
- Network: default libvirt NAT; lab isolation not yet verified
- Intended local account: `labuser`
- Intended device name: `CyberLab-Win11` (verify in guest)

### Kali Linux
- Installed in Virtual Machine Manager
- CPU, RAM, and disk allocations: verify before documenting

## Validation Checklist
- [ ] Verify Windows device name and updates
- [ ] Record Kali VM resource allocations
- [ ] Confirm lab network design before running simulations
- [ ] Install Sysmon and document its configuration
- [ ] Deploy log collection / SIEM and verify events arrive

*Only record a setting as verified after checking it in the VM or hypervisor.*
