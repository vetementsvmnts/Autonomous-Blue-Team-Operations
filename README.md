# Autonomous Blue Team Operations

End-to-End Threat Detection and Incident Response Lab

## Overview
A self-contained SOC home lab built to simulate, detect, and investigate cyber attacks using Wazuh, Sysmon, and Kali Linux.

## Architecture
| Machine | IP Address | Role |
| :--- | :--- | :--- |
| Wazuh Server (Ubuntu 24.04) | 192.168.56.10 | SIEM |
| Windows Victim (Win 10) | 192.168.56.20 | Endpoint (Sysmon + Wazuh Agent) |
| Kali Attacker | 192.168.56.30 | Attack Simulation |

See `Lab-Architecture/topology.png` for the diagram.

## Tools Used
- Oracle VirtualBox
- Ubuntu Server 24.04 LTS
- Wazuh 4.14 (SIEM)
- Sysmon + Olaf Hartong's sysmonconfig.xml
- Windows 10 Home
- Kali Linux 2026.2

## Project Phases
- [x] Phase 1: Planning & Architecture
- [ ] Phase 2: Core Infrastructure Deployment
- [ ] Phase 3: Telemetry Verification & Attack Simulation
- [ ] Phase 4: Triage, Investigation, and Incident Response
- [ ] Phase 5: Portfolio Packaging & GitHub Polish

## Repository Structure
- `Assets/` — Screenshots and visual evidence
- `Configuration-Files/` — Sysmon config and custom rules
- `Incident-Reports/` — Mock IR tickets and reports
- `Lab-Architecture/` — Network diagrams and design docs
