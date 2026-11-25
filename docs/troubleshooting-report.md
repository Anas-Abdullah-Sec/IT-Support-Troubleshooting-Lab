

\# Technical Troubleshooting Report



\*\*Project:\*\* IT Support Hardware \& Software Troubleshooting Lab  

\*\*Author:\*\* Anas Abdullah  

\*\*Lab Device:\*\* HP Pro 3330 MT  

\*\*Operating System:\*\* Windows 10 Home  

\*\*Inspection Date:\*\* November 25, 2026



\---



\## 1. Executive Summary



This report documents the results of eight practical IT Support tasks performed on a physical Windows desktop.



The inspection covered hardware specifications, system performance, startup applications, running processes, installed software, Windows Update status, device drivers, network connectivity, disk storage, and Windows maintenance records.



The work focused on identifying system conditions, performing basic diagnostics, recording observations, and maintaining supporting evidence.



No hardware repairs, driver updates, software installations, or advanced system configuration changes were performed.



\## 2. Lab Environment



| Component | Specification |
|---|---|
| Manufacturer / Model | HP Pro 3330 MT |
| Processor | Intel Core i3-2120 |
| CPU | 2 Cores / 4 Logical Processors |
| RAM | 4 GB DDR3, 1333 MHz |
| Storage | 128 GB SSD |
| Operating System | Windows 10 Home |
| BIOS Mode | UEFI |
| BIOS Version | AMI 7.05 |
| Visible SSD Capacity | 119.23 GB |



\## 3. Task-wise Technical Findings



\### Task 01 — System Hardware Inspection \& Performance Analysis



\*\*Activities performed:\*\*

\- Inspected hardware and operating system information using System Information.

\- Reviewed CPU, memory, and disk utilization in Task Manager.

\- Inspected disk partitions through Disk Management.

\- Reviewed visible device status in selected Device Manager categories.



\*\*Performance observations:\*\*



| Metric | Recorded Observation |
|---|---|
| CPU Usage | 6% in one recorded snapshot |
| CPU Speed | 3.18 GHz in that snapshot |
| Memory Usage | 2.2 / 3.9 GB (56%) |
| Available Memory | Approximately 1.7 GB |
| SSD Active Time | 0% |
| SSD Response Time | 1.0 ms |



A separate performance snapshot recorded CPU usage at 2%, memory usage at 45%, disk usage at 0%, and network activity at 0 Mbps.



These values represent observations at specific points in time, not continuous performance measurements.



\*\*Disk partition observations:\*\*



| Partition | Capacity / Size | File System / Purpose |
|---|---:|---|
| EFI System Partition | 100 MB | EFI |
| C: | 69.76 GB | NTFS |
| D: | 48.83 GB | NTFS |
| Recovery Partition | 546 MB | Recovery |



\*\*Finding:\*\* The system hardware, resource utilization, and partition layout were successfully inspected and documented.



\*\*Evidence:\*\* `evidence/01-system-information/`



\### Task 02 — Windows Startup Application Analysis



\*\*Activities performed:\*\*

\- Inspected startup applications through Task Manager.

\- Recorded enabled and disabled entries.

\- Reviewed the displayed startup impact indicators.



\*\*Recorded observations:\*\*



| Startup Entry | Status | Displayed Impact |
|---|---|---|
| Copilot | Disabled | None |
| Intel hkcmd Module | Enabled | Low |
| Intel igfxTray Module | Enabled | Low |
| Microsoft Edge | Enabled | Not measured |
| Intel Persistence Module | Enabled | Medium |
| Phone Link | Disabled | None |
| RobloxPlayerBeta | Enabled | Not measured |
| Starter Module | Enabled | Medium |
| Windows host process | Enabled | Medium |
| Windows Security Notification | Enabled | Low |



\*\*Finding:\*\* Startup configuration was inspected. No startup entries were enabled or disabled during the task. The identity and purpose of Starter Module were not independently verified.



\*\*Evidence:\*\* `evidence/02-startup-analysis/`



\### Task 03 — Running Process \& Resource Usage Analysis



\*\*Activities performed:\*\*

\- Reviewed running applications and background processes.

\- Observed CPU, memory, disk, and network utilization.

\- Recorded a system performance snapshot.



\*\*Recorded snapshot:\*\*



| Resource | Observed Usage |
|---|---:|
| CPU | 2% |
| Memory | 45% |
| Disk | 0% |
| Network | 0 Mbps |



\*\*Finding:\*\* Running processes and resource utilization were inspected. The recorded values reflect the system state at the time of observation.



\*\*Evidence:\*\* `evidence/03-process-analysis/`



\### Task 04 — Installed Software Inventory



\*\*Activities performed:\*\*

\- Reviewed installed applications.

\- Recorded application names, publishers, and displayed versions.



\*\*Inventory:\*\*



| Application | Publisher | Version |
|---|---|---|
| Brave | Brave Software Inc | 158.1.100.59 |
| Copilot | Microsoft Corporation | 158.0.4370.33 |
| Lightshot | Skillbrains | 5.5.0.7 |
| qBittorrent | The qBittorrent project | 5.2.3 |



\*\*Finding:\*\* The listed installed applications were identified and documented. No software was installed or uninstalled.



\*\*Evidence:\*\* `evidence/04-installed-software/`



\### Task 05 — Windows Update Inspection



\*\*Activities performed:\*\*

\- Inspected Windows Update settings.

\- Reviewed the operating system support notification.



\*\*Finding:\*\* Windows Update displayed a Windows 10 end-of-support notification. Windows 10 general support ended on October 14, 2025.



An Extended Security Updates (ESU) option was visible. Enrollment in ESU was not verified.



\*\*Evidence:\*\* `evidence/05-windows-update/`



\### Task 06 — Device Driver Inspection



\*\*Activities performed:\*\*

\- Inspected Wi-Fi, Ethernet, and display adapter driver details.

\- Recorded driver providers, dates, and versions.

\- Reviewed selected Device Manager categories for visible warnings.



\*\*Driver inventory:\*\*



| Device | Driver Provider | Driver Date | Version |
|---|---|---|---|
| Qualcomm Atheros AR9485 Wi-Fi | Qualcomm Atheros Communications Inc. | June 19, 2017 | 10.0.0.352 |
| Realtek PCIe GBE Family Controller | Realtek | July 23, 2015 | 10.3.723.2015 |
| Intel HD Graphics | Intel Corporation | May 19, 2016 | 9.17.10.4459 |



\*\*Finding:\*\* Driver information was successfully inspected and recorded. No driver update, rollback, or uninstallation was performed.



Older driver dates alone do not establish that a driver is faulty or incompatible.



No visible yellow warning or unknown device was observed in the inspected Device Manager categories.



\*\*Evidence:\*\* `evidence/06-driver-inspection/`



\### Task 07 — Network Troubleshooting



\*\*Activities performed:\*\*

The following Windows command-line diagnostics were executed:



| Command | Purpose | Result |
|---|---|---|
| `ipconfig` | Inspect IPv4 configuration | IPv4 information present |
| `ipconfig /all` | Review detailed configuration | Inspected |
| `ping 127.0.0.1` | Test loopback connectivity | Successful |
| `ping 8.8.8.8` | Test external IP connectivity | Successful |
| `nslookup google.com` | Test DNS resolution | Successful |
| `ipconfig /flushdns` | Clear DNS resolver cache | Successful |



\*\*Additional observations:\*\*

\- An IPv4 address was present.

\- A default gateway was present.

\- The loopback connectivity test succeeded.

\- External IP connectivity succeeded.

\- DNS resolution succeeded.

\- DNS cache flush completed successfully.



\*\*Finding:\*\* Basic network configuration, IP connectivity, and DNS resolution were working during the tests.



These tests do not constitute a complete network security or performance assessment.



\*\*Evidence:\*\* `evidence/07-network-troubleshooting/`



\### Task 08 — Disk Cleanup \& Windows Maintenance



\*\*Activities performed:\*\*

\- Inspected Disk Cleanup categories.

\- Reviewed Windows Storage usage.

\- Examined Reliability Monitor.

\- Inspected the visible System log entries in Event Viewer.



\*\*Disk Cleanup observation:\*\*



Disk Cleanup displayed approximately 1.19 GB of potential cleanup space. The selected categories included:

\- Temporary files: approximately 1.16 GB

\- Thumbnails: approximately 30.1 MB



This was recorded as potential cleanup space. The amount of disk space actually reclaimed was not verified.



\*\*Storage usage:\*\*



| Category | Reported Usage |
|---|---:|
| System \& reserved | 21.2 GB |
| Apps \& features | 10.2 GB |



\*\*Reliability Monitor observation:\*\*



A critical event was recorded on November 25, 2026, at 5:11 PM:



`Windows was not properly shut down.`



The event confirms that an improper shutdown was logged. The underlying cause was not established during this inspection.



\*\*Event Viewer observation:\*\*

\- No recent Error entries were visible in the inspected System log list.

\- DistributedCOM Event ID 10016 warnings were observed.

\- The inspection was limited to the visible entries and does not establish that no other errors exist.



\*\*Finding:\*\* Storage usage and Windows maintenance records were reviewed. The improper shutdown event was documented for further investigation if it recurs.



\*\*Evidence:\*\* `evidence/08-disk-cleanup-maintenance/`



\## 4. Consolidated Findings



1\. Basic IPv4 configuration was present.

2\. Loopback and external IP connectivity tests succeeded.

3\. DNS resolution worked during testing.

4\. No visible device warnings were observed in the inspected Device Manager categories.

5\. Windows 10 displayed an end-of-support notification.

6\. Driver information was collected for three inspected adapters.

7\. Reliability Monitor recorded an improper shutdown event.

8\. Disk Cleanup displayed approximately 1.19 GB of potential cleanup space.

9\. Installed software and startup entries were inventoried.



\## 5. Recommendations



Based on the observations, the following actions are recommended:



\- Plan migration to a supported operating system or another supported platform.

\- Review the cause of the improper shutdown if the event occurs repeatedly.

\- Maintain regular backups of important data.

\- Periodically review installed software and startup applications.

\- Monitor available disk capacity.

\- Review driver compatibility and vendor-supported updates when required.

\- Continue monitoring system performance during normal usage.



These are recommendations only. The actions listed above were not all performed as part of this lab.



\## 6. Scope and Limitations



This practical lab covered foundational Windows desktop inspection and basic IT Support diagnostics.



The project did not include:

\- Hardware component replacement or physical repair.

\- Windows Server administration.

\- Active Directory administration.

\- Enterprise endpoint management.

\- Advanced malware analysis or incident response.

\- Driver updates, rollbacks, or replacements.

\- Software installation or uninstallation.

\- Root-cause analysis of the improper shutdown event.



All findings represent observations from the inspected device at the time of testing.



\## 7. Conclusion



The lab provided practical experience in inspecting Windows desktop hardware, monitoring system resources, reviewing startup applications and installed software, examining device drivers, performing basic network diagnostics, and reviewing Windows maintenance information.



The work also emphasized structured troubleshooting, evidence collection, accurate interpretation of diagnostic results, and technical documentation.



The completed tasks demonstrate foundational practical skills relevant to entry-level IT Support, Help Desk, and Desktop Support roles.



\---



\*\*Prepared by:\*\* Anas Abdullah  

\*\*Project:\*\* IT Support Hardware \& Software Troubleshooting Lab  

\*\*GitHub:\*\* https://github.com/Anas-Abdullah-Sec  

\*\*LinkedIn:\*\* https://www.linkedin.com/in/anas2abdullah/



