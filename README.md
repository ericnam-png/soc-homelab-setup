# SOC Homelab Setup

## Summary
This project documents the setup of a personal SOC homelab environment built to simulate endpoint monitoring and log analysis using SIEM tools.

## Overview
The lab includes a Windows-based environment, a SIEM solution (Splunk), and endpoint monitoring using Sysmon. It is designed to support security testing, log analysis, and attack simulation.

## Architecture
- Windows 11 (Target system)
- Kali Linux (Attacker machine)
- Splunk (SIEM)
- Sysmon (Endpoint monitoring)

## Environment
- VirtualBox
- Windows 11
- Kali Linux

## Setup Steps

### 1. Virtual Machine Setup
- Created Windows 11 and Kali Linux virtual machines using VirtualBox  
- Configured an isolated network to allow communication only between the machines  

### 2. Sysmon Deployment
- Installed Sysmon on the Windows system  
- Configured logging for process creation and system activity  

### 3. Splunk Installation
- Installed Splunk Enterprise on the Windows system  
- Configured log ingestion and data input  
- Enabled receiving logs from the endpoint  

## Key Capabilities
- Centralized log collection through Splunk  
- Endpoint visibility using Sysmon  
- Controlled environment for attack simulation and testing  

## What I Learned
- How to build a basic SOC-like lab environment
- How different Net settings speak to eachother/internet
- Understanding of log pipelines and data ingestion  
- SIEM setup and integration with endpoints  
- Basic search queries to identify suspicious activity  

## Next Step
This environment is used for detection-focused projects, including:
- Brute-force attack detection  
- Remote command execution (RCE) detection  
- Log-based threat analysis

## Reference
- [MyDFIR YouTube Channel](https://www.youtube.com/@MyDFIR)
