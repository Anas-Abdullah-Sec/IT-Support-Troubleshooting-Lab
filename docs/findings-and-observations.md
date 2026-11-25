

\# Findings \& Observations



\*\*Project:\*\* IT Support Hardware \& Software Troubleshooting Lab  

\*\*Device:\*\* HP Pro 3330 MT  

\*\*Inspection Date:\*\* November 25, 2026



\## 1. System Baseline



| Component | Observation |
|---|---|
| Processor | Intel Core i3-2120 |
| CPU Configuration | 2 Cores / 4 Logical Processors |
| Memory | 4 GB DDR3, 1333 MHz |
| Storage | 128 GB SSD |
| Operating System | Windows 10 Home |
| BIOS Mode | UEFI |
| BIOS Version | AMI 7.05 |



\## 2. Performance Observations



Two separate performance snapshots were recorded during inspection.



| Metric | Snapshot 1 | Snapshot 2 |
|---|---:|---:|
| CPU | 6% | 2% |
| Memory | 56% | 45% |
| Disk | 0% active time | 0% |
| Network | Not recorded | 0 Mbps |



Snapshot 1 also showed CPU speed of 3.18 GHz, approximately 1.7 GB available memory, and SSD response time of 1.0 ms.



These are time-specific observations and do not represent long-term performance benchmarks.



\## 3. Startup Application Observations



| Entry | Startup Status | Displayed Impact |
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



No startup configuration changes were performed.



The identity of Starter Module was not independently verified.



\## 4. Installed Software Inventory



| Application | Publisher | Version |
|---|---|---|
| Brave | Brave Software Inc | 158.1.100.59 |
| Copilot | Microsoft Corporation | 158.0.4370.33 |
| Lightshot | Skillbrains | 5.5.0.7 |
| qBittorrent | The qBittorrent project | 5.2.3 |



No installation or uninstallation was performed.



\## 5. Operating System Support



Windows Update displayed an end-of-support notification.



Windows 10 general support ended on October 14, 2025. An ESU option was visible, but enrollment was not verified.



\*\*Observation:\*\* The operating system's support status should be considered when planning future maintenance and security updates.



\## 6. Device Driver Inventory



| Adapter | Provider | Date | Version |
|---|---|---|---|
| Qualcomm Atheros AR9485 Wi-Fi | Qualcomm Atheros Communications Inc. | 19 Jun 2017 | 10.0.0.352 |
| Realtek PCIe GBE Family Controller | Realtek | 23 Jul 2015 | 10.3.723.2015 |
| Intel HD Graphics | Intel Corporation | 19 May 2016 | 9.17.10.4459 |



No driver updates, rollbacks, or uninstallations were performed.



Older driver dates alone do not prove a driver fault.



\## 7. Network Diagnostic Results



| Diagnostic | Result |
|---|---|
| IPv4 address inspection | Address present |
| Default gateway inspection | Gateway present |
| `ping 127.0.0.1` | Successful |
| `ping 8.8.8.8` | Successful |
| `nslookup google.com` | Successful |
| `ipconfig /flushdns` | Successful |



\*\*Observation:\*\* Basic IP connectivity and DNS resolution were functioning during the tests.



\## 8. Storage Observations



| Category | Reported Usage |
|---|---:|
| System \& reserved | 21.2 GB |
| Apps \& features | 10.2 GB |



Disk Cleanup displayed approximately 1.19 GB of potential cleanup space:

\- Temporary files: approximately 1.16 GB

\- Thumbnails: approximately 30.1 MB



Actual reclaimed space was not verified.



\## 9. Reliability and Event Log Observations



Reliability Monitor recorded:



\- Event: Windows was not properly shut down.

\- Date: November 25, 2026.

\- Time: 5:11 PM.

\- Severity: Critical.



This confirms that an improper shutdown was logged. Its root cause was not established.



Event Viewer inspection showed:

\- No recent Error entries visible in the inspected System log list.

\- DistributedCOM Event ID 10016 warnings were observed.

\- Information-level events were also visible.



These observations are limited to the inspected entries.



\## 10. Recommended Follow-up Actions



1\. Review the improper shutdown event if it recurs.

2\. Plan migration to a supported operating system or platform.

3\. Maintain regular data backups.

4\. Review startup applications periodically.

5\. Monitor storage capacity.

6\. Verify driver compatibility before making updates.



\## 11. Scope



This document records findings from the eight practical inspection tasks.



It does not claim that repairs, driver updates, software changes, or enterprise administration activities were performed.



\---



\*\*Prepared by:\*\* Anas Abdullah



