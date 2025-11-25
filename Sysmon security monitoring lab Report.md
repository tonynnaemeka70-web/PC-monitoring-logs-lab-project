PC Logs Monitoring Report – Sysmon Lab

 Setup Summary

Tool Installed: Sysmon64 v15.15 from Sysinternals

Configuration File: sysmonconfig-export.xml from SwiftOnSecurity GitHub repo

System: Windows 10 pro

User: tony nnaemeka

 Objective

To monitor basic security events on a personal PC using Sysmon and Windows Event Viewer, and analyze three types of incidents: process creation, PowerShell activity, and failed login attempts.

Activities Performed

Installed Sysmon64 using administrative Command Prompt:

Sysmon64.exe -i

Then applied the configuration:

Sysmon64.exe -c sysmonconfig-export.xml

Generated events:

Opened PowerShell and ran Get-Process it will display all the system logs from the window power shell

Launched Notepad and Calculator

Enter window + L button, Locked screen and entered incorrect password multiple times like up to 3-5 times

Viewed logs in Event Viewer:

Press window buton and enter event viewer and navigate to Applications and Services Logs and custom views

Also checked Windows Logs Securi



screenshot

My Findings
 I saw and identify events IDS for process start, power shell use, system failed login

Event Type ,       Event ID,     Description                                       timestamp
procss creation        1            Notepad.exe and calculator                        1:20pm
PowerShell commands    1             Get-process executd                               1:27pm                           
failed logon           12           incorrect password attempts                       1:43pm



 Recommendations

Enable account lockout policy after 5 failed login attempts to prevent brute-force attacks.

Restrict PowerShell access to administrators only.

Monitor USB activity and disable ports on sensitive machines.

Repository Notes

This report is part of my cybersecurity learning journey. All tools used are free and publicly available. Screenshots and config files are included in the /assets folder of this repo.

Author: Tony (SOOD ELIASER)
