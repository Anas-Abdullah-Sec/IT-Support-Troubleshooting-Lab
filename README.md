# PC Hardware & Software Troubleshooting Lab

**Project Type:** Hands-on IT Support Practical Lab  
**Environment:** HP Pro 3330 MT | Windows 10 Home  
**Operating System:** Windows 10 Home  
**Hardware:** Intel Core i3-2120 | 4GB DDR3 RAM | 128GB SSD  
**Status:** Practical tasks completed; findings documented

## Project Overview

This project demonstrates hands-on IT support practice using a physical desktop computer running Windows 10. It focuses on system inspection, Windows troubleshooting, software inventory, driver inspection, network diagnostics and basic maintenance.

The purpose was to practice a structured troubleshooting approach and document findings with practical evidence.

## Lab Environment

| Component | Specification |
|---|---|
| Device | HP Pro 3330 MT |
| Processor | Intel Core i3-2120 |
| Memory | 4GB DDR3 |
| Storage | 128GB SSD |
| Operating System | Windows 10 Home |
| BIOS Mode | UEFI |

## Practical Tasks

### 01. System Hardware Inspection & Performance Analysis
- Inspected system specifications using System Information.
- Reviewed CPU, memory and disk utilization through Task Manager.
- Checked disk partitions using Disk Management.
- Inspected Device Manager for visible device warnings.

### 02. Windows Startup Application Analysis
- Reviewed startup applications.
- Examined startup impact indicators.
- Identified enabled and disabled startup entries.

### 03. Running Process & Resource Usage Analysis
- Reviewed running Windows processes.
- Monitored CPU, memory, disk and network utilization.
- Observed active Windows services and background processes.

### 04. Installed Software Inventory
- Reviewed installed applications through Programs and Features.
- Recorded application names, publishers and versions.

### 05. Windows Update Inspection
- Inspected Windows Update status.
- Identified the Windows 10 end-of-support notification.

### 06. Device Driver Inspection
- Inspected Wi-Fi, Ethernet and Display adapter drivers.
- Recorded driver providers, dates and versions.
- Checked Device Manager for visible warnings.

### 07. Network Troubleshooting
Performed basic network diagnostics using Windows command-line tools:

| Command | Purpose | Result |
|---|---|---|
| `ipconfig` | IPv4 configuration | Successful |
| `ipconfig /all` | Detailed network configuration | Inspected |
| `ping 127.0.0.1` | Loopback test | Successful |
| `ping 8.8.8.8` | External connectivity test | Successful |
| `nslookup google.com` | DNS resolution test | Successful |
| `ipconfig /flushdns` | Clear DNS resolver cache | Successful |

### 08. Disk Cleanup & Windows Maintenance
- Reviewed available cleanup categories using Disk Cleanup.
- Identified approximately 1.19 GB of potential cleanup space.
- Inspected Windows Storage usage.
- Reviewed Reliability Monitor and Event Viewer.

**Storage findings:**
- System & reserved: 21.2 GB
- Apps & features: 10.2 GB

**Maintenance findings:**
- Reliability Monitor recorded a critical event: "Windows was not properly shut down" on November 25, 2026.
- No recent Error entries were visible in the inspected System log list.
- DistributedCOM Event ID 10016 warnings were observed.

## Key Findings

- Basic IPv4 configuration, external IP connectivity and DNS resolution were working during testing.
- No visible Device Manager warnings were identified in the inspected categories.
- Windows 10 displayed an end-of-support notification.
- A previous improper shutdown was recorded in Reliability Monitor.
- Approximately 1.19 GB of potential disk cleanup space was identified.

## Evidence

Screenshots documenting the practical tasks are organized in the `evidence/` directory.

## Scope & Limitations

This was a hands-on diagnostic and maintenance lab. It documents inspections and tests actually performed.

It does not claim enterprise Active Directory administration, Windows Server management, driver replacement, advanced hardware repair or production-level helpdesk experience.

## Author

**Anas Abdullah**

- GitHub: https://github.com/Anas-Abdullah-Sec
- LinkedIn: https://www.linkedin.com/in/anas2abdullah/

