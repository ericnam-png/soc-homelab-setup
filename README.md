# SOC Homelab Setup

## Summary
This project documents the setup of a personal SOC homelab environment designed to simulate real-world enterprise infrastructure for security monitoring and analysis.

## Overview
The lab includes a Windows-based environment, a SIEM solution (Splunk), and endpoint monitoring using Sysmon. The setup is designed to support security testing, log analysis, and attack simulation.

## Architecture
- Windows 11 Client
- Kali Linux (Attacker machine)
- Splunk (SIEM)
- Sysmon (Endpoint monitoring)

## Environment
- VirtualBox
- Windows 11
- Kali Linux

## Setup Steps
### 1. Virtual Machine Setup
- Created Win11,Kali using VirtualBox
- Configured network to let them speak only to each other

### 2. Active Directory Configuration
- Installed Windows Server
- Promoted to Domain Controller
- Created domain users and groups
- Configured Group Policy

### 3. Splunk Installation
- Installed Splunk Enterprise on Windows
- Configured data ingestion
- Enabled receiving logs

### 4. Sysmon Deployment
- Installed Sysmon on endpoints
- Configured logging for process creation and system activity

### 5. Log Forwarding
- Installed Splunk Universal Forwarder
- Forwarded logs to Splunk server

## Key Capabilities
- Centralized log collection via SIEM
- Endpoint monitoring using Sysmon
- Active Directory environment for authentication testing
- Attack simulation readiness

## What I Learned
- How to design and build a SOC-like lab environment
- Understanding of log pipelines and data ingestion
- Active Directory fundamentals and user management
- SIEM setup and integration with endpoints

## Next Step
This environment is used for detection-focused projects, including:
- Brute-force attack detection
- Remote command execution (RCE) detection
- Log-based threat analysis
