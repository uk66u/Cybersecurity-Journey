# Windows Logging for SOC

## Lab Information

**Topic:** Windows Security Monitoring  
**Focus:** Windows Event Logs, Sysmon, Authentication, Process Monitoring, Network Activity, and PowerShell Analysis

## Key Concepts Learned

- Windows Event Viewer
- Security Event Logs
- Successful and Failed Logons
- RDP Authentication Analysis
- User Account Management
- Event Correlation using Logon IDs
- Sysmon Monitoring
- Process Creation Analysis
- Parent and Child Process Analysis
- File Creation Monitoring
- Network Connection Analysis
- DNS Query Analysis
- PowerShell History Analysis

## Important Windows Event IDs

- **4624** — Successful Logon
- **4625** — Failed Logon
- **4720** — User Account Created
- **4724** — Password Reset Attempt
- **4732** — User Added to a Security Group
- **4733** — User Removed from a Security Group

## Important Sysmon Event IDs

- **1** — Process Creation
- **3** — Network Connection
- **11** — File Creation
- **13** — Registry Value Set
- **15** — FileCreateStreamHash
- **22** — DNS Query

## Investigation Workflow

1. Review authentication events.
2. Identify repeated failed login attempts.
3. Correlate failed and successful logins.
4. Review the Logon Type and source IP address.
5. Use the Logon ID to correlate related activity.
6. Investigate account creation and group membership changes.
7. Analyze process creation with Sysmon.
8. Trace parent and child processes.
9. Review file, network, and DNS activity.
10. Review PowerShell history for suspicious commands.

## Practical Skills Practiced

- Windows Event Log Analysis
- Authentication Investigation
- RDP Activity Analysis
- Event Correlation
- User and Group Monitoring
- Sysmon Analysis
- Process Monitoring
- Network Connection Analysis
- DNS Analysis
- PowerShell Investigation

## Summary

This lab provided hands-on practice with Windows Security Logs and Sysmon to investigate authentication activity, account changes, process execution, file creation, network connections, DNS activity, and PowerShell usage.

The investigation focused on correlating multiple events to reconstruct suspicious activity instead of relying on a single alert or log entry.
