# Phase 1: Planning & Architecture

## Objective
Define the architecture and prepare all installation files before building VMs.

## Final Architecture
Wazuh is deployed via Docker Desktop + WSL2 instead of a VirtualBox VM 
due to VirtualBox CPU scheduling conflicts with the Intel i7-13620H hybrid CPU.

| Component | Platform | Access |
| :--- | :--- | :--- |
| Wazuh SIEM | Docker + WSL2 | https://localhost |
| Windows Victim | VirtualBox | 192.168.56.20 |
| Kali Attacker | VirtualBox | 192.168.56.30 |

## Tools Downloaded
- Oracle VirtualBox 7.x + Extension Pack
- Windows 10 Home ISO
- Kali Linux VM (2026.2)
- Sysmon v15.22
- Olaf Hartong's sysmonconfig.xml (v13.34, schemaversion 4.60)
- Docker Desktop + WSL2 Ubuntu
- Wazuh Docker (v4.9.2)

## Key Decisions
- Windows 10 Home (no functional difference from Pro for this lab)
- Wazuh via Docker after VirtualBox VM failures (CPU stalls, disk-full)
- No LVM partitions (previous LVM caused disk-full errors)
- Windows Defender exclusions added for VirtualBox performance
- High Performance power plan enabled

## Status
Phase 1 COMPLETE 
