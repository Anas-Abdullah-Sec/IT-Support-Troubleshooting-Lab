

# IT Support Hardware & Software Troubleshooting Lab



**Author:** Anas Abdullah  

**Project Type:** Hands-on IT Support Practical Lab  

**Environment:** Physical Desktop Lab  

**Operating System:** Windows 10 Home  

**Status:** Completed — Practical Inspection & Documentation



---



## 1. Executive Summary



This project demonstrates practical IT Support skills through the inspection, analysis, and documentation of a physical Windows desktop environment.



The lab involved eight practical tasks covering hardware inspection, Windows performance monitoring, startup application analysis, software inventory, Windows Update inspection, device driver verification, network diagnostics, and Windows maintenance.



A structured troubleshooting approach was followed using built-in Windows utilities and command-line tools. Findings were recorded and supported by screenshots.



The objective was to develop practical experience in identifying system conditions, performing basic diagnostic checks, interpreting results, and documenting technical observations.



## 2. Lab Environment



| Component | Specification |
|---|---|
| Device | HP Pro 3330 MT |
| Processor | Intel Core i3-2120 |
| CPU Configuration | 2 Cores / 4 Logical Processors |
| Memory | 4 GB DDR3 |
| Storage | 128 GB SSD |
| Operating System | Windows 10 Home |
| BIOS Mode | UEFI |
| BIOS Version | AMI 7.05 |



## 3. Project Objectives



- Inspect desktop hardware and system configuration.

- Analyze Windows startup applications and running processes.

- Review CPU, memory, and disk utilization.

- Inventory installed software.

- Inspect Windows Update status and device drivers.

- Perform basic network connectivity and DNS diagnostics.

- Review disk storage and Windows maintenance information.

- Document diagnostic procedures and findings with evidence.



## 4. Tools & Utilities



| Tool | Purpose |
|---|---|
| System Information (`msinfo32`) | Hardware and system configuration |
| Task Manager | Performance and process analysis |
| Device Manager | Hardware and driver inspection |
| Disk Management | Disk and partition inspection |
| Programs and Features | Installed software inventory |
| Windows Update | Update status inspection |
| Command Prompt | Network diagnostics |
| Disk Cleanup (`cleanmgr`) | Disk cleanup assessment |
| Storage Settings | Storage usage analysis |
| Reliability Monitor (`perfmon /rel`) | System reliability review |
| Event Viewer (`eventvwr.msc`) | Windows event log inspection |



## 5. Practical Tasks



### Task 01 — System Hardware Inspection & Performance Analysis



**Objective:** Inspect hardware specifications, storage configuration, and system resource utilization.



**Activities:**

- Reviewed hardware and OS information using System Information.

- Inspected CPU, memory, and disk utilization through Task Manager.

- Examined disk partitions using Disk Management.

- Checked Device Manager for visible device warnings.



**Result:** System configuration and resource utilization were successfully inspected and documented.



**Evidence:** `evidence/01-system-information/`



### Task 02 — Windows Startup Application Analysis



**Objective:** Review applications configured to launch during Windows startup.



**Activities:**

- Inspected enabled and disabled startup entries.

- Reviewed available startup impact indicators.

- Recorded startup application information.



**Result:** Startup entries and their displayed impact indicators were documented. No startup configuration changes were made.



**Evidence:** `evidence/02-startup-analysis/`



### Task 03 — Running Process & Resource Usage Analysis



**Objective:** Examine running processes and current system resource utilization.



**Activities:**

- Reviewed running applications and background processes.

- Monitored CPU, memory, disk, and network utilization.

- Observed Windows background processes and services.



**Result:** A performance snapshot was recorded, including CPU, memory, disk, and network utilization.



**Evidence:** `evidence/03-process-analysis/`



### Task 04 — Installed Software Inventory



**Objective:** Review software installed on the desktop.



**Activities:**

- Inspected installed applications through Programs and Features.

- Recorded application names, publishers, and versions.



**Result:** Installed software inventory was reviewed and documented.



**Evidence:** `evidence/04-installed-software/`



### Task 05 — Windows Update Inspection



**Objective:** Review Windows Update status and operating system support information.



**Activities:**

- Inspected Windows Update settings.

- Reviewed the displayed Windows 10 end-of-support notification.



**Result:** Windows 10 general support ended on October 14, 2025. The system displayed an end-of-support notification.



**Evidence:** `evidence/05-windows-update/`



### Task 06 — Device Driver Inspection



**Objective:** Inspect installed network and display adapter drivers.



**Activities:**

- Reviewed Wi-Fi adapter driver information.

- Inspected Ethernet adapter driver details.

- Reviewed Intel display adapter driver information.

- Checked inspected Device Manager categories for visible warnings.



**Result:** Driver providers, dates, and versions were recorded. No driver updates, rollbacks, or uninstallations were performed.



**Evidence:** `evidence/06-driver-inspection/`



### Task 07 — Network Troubleshooting



**Objective:** Perform basic network configuration, connectivity, and DNS diagnostics.



**Commands Used:**



| Command | Diagnostic Purpose | Result |
|---|---|---|
| `ipconfig` | IPv4 configuration | Successful |
| `ipconfig /all` | Detailed network configuration | Inspected |
| `ping 127.0.0.1` | Loopback connectivity | Successful |
| `ping 8.8.8.8` | External IP connectivity | Successful |
| `nslookup google.com` | DNS resolution | Successful |
| `ipconfig /flushdns` | DNS resolver cache flush | Successful |



**Observations:**

- IPv4 address was present.

- Default gateway was present.

- Loopback test succeeded.

- External IP connectivity test succeeded.

- DNS resolution succeeded.

- DNS cache flush completed successfully.



**Result:** Basic IPv4 configuration, connectivity, and DNS tests completed successfully during the inspection.



**Evidence:** `evidence/07-network-troubleshooting/`



### Task 08 — Disk Cleanup & Windows Maintenance



**Objective:** Review available disk cleanup opportunities, storage utilization, and Windows maintenance events.



**Activities:**

- Inspected cleanup categories through Disk Cleanup.

- Reviewed Windows Storage usage.

- Examined Reliability Monitor.

- Inspected recent entries in Windows Event Viewer.



**Storage Observations:**



| Category | Reported Usage |
|---|---:|
| System & reserved | 21.2 GB |
| Apps & features | 10.2 GB |



**Maintenance Findings:**

- Disk Cleanup displayed approximately 1.19 GB of potential cleanup space.

- Reliability Monitor recorded a critical event: "Windows was not properly shut down" on November 25, 2026, at 5:11 PM.

- No recent Error entries were visible in the inspected System log list.

- DistributedCOM Event ID 10016 warnings were observed.



**Result:** Storage usage and maintenance records were inspected. The improper shutdown event was documented for further investigation if it recurs.



**Evidence:** `evidence/08-disk-cleanup-maintenance/`



## 6. Key Technical Findings



1. Basic network configuration and connectivity tests were successful.

2. DNS resolution was working during testing.

3. No visible device warnings were identified in the inspected Device Manager categories.

4. Windows 10 displayed an end-of-support notification.

5. Reliability Monitor recorded an improper shutdown event.

6. System & reserved was the largest reported storage category.

7. Approximately 1.19 GB of potential cleanup space was identified.



## 7. Recommendations



- Consider migrating to a supported Windows operating system or an appropriate supported alternative.

- Review the cause of the improper shutdown if similar events recur.

- Maintain regular backups of important files.

- Periodically review startup applications and installed software.

- Monitor available storage capacity.

- Keep device drivers and operating system components appropriately maintained.



## 8. Scope & Limitations



This project focused on practical system inspection, basic diagnostics, maintenance review, and technical documentation.



The work does not claim:

- Enterprise Active Directory administration.

- Windows Server administration.

- Advanced hardware component repair.

- Production environment incident response.

- Driver replacement or update procedures.

- Software installation or uninstallation.



Findings represent observations from the inspected system at the time of testing and should not be interpreted as a comprehensive hardware or security audit.



## 9. Evidence & Documentation



The `evidence/` directory contains screenshots organized by practical task.



The `docs/` directory contains supporting technical documentation, and the `reports/` directory contains the final project report.



## 10. Conclusion



This practical lab provided hands-on experience with Windows desktop inspection, system performance monitoring, software inventory, device driver review, network diagnostics, and maintenance analysis.



It also provided experience in following a structured troubleshooting process, interpreting diagnostic results, identifying observations, and maintaining technical evidence.



The project demonstrates foundational practical skills relevant to entry-level IT Support, Help Desk, and Desktop Support roles.



---



## Author



**Anas Abdullah**



- GitHub: https://github.com/Anas-Abdullah-Sec

- LinkedIn: https://www.linkedin.com/in/anas2abdullah/



