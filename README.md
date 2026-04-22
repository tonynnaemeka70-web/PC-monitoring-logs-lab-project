PC Monitoring & Security Log Analysis Lab (SOC Simulation)

Project Overview

This project simulates a Security Operations Center (SOC) monitoring environment where system logs are collected, analyzed, and investigated to detect suspicious activity and potential security incidents.

seconddly it demonstrates basic security monitoring on a Windows PC using [Sysmon](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon) and Windows Event Viewer. It was completed as part of my cybersecurity learning journey.


The objective is to demonstrate practical skills in:
Log analysis and interpretation
Incident detection and response simulation
Security monitoring workflows used in SOC environments

Objectives
Collect and review system activity logs from a monitored environment
2.Identify abnormal or suspicious behavior patterns
3.Simulate real-world security incident detection scenarios
4.Document findings in a structured incident report format

Tools & Technologies
1.Linux System Logs (auth.log / system logs)
2.Windows Event Viewer 
3.Log analysis techniques
4.Basic incident response methodology
5.Configuration File: `sysmonconfig-export.xml` from [SwiftOnSecurity](https://github.com/SwiftOnSecurity/sysmon-config)

Project Workflow
 -Log Collection
-System logs were gathered from monitored endpoints, focusing on:
-Authentication attempts
-System access events
-User activity logs
-Error and warning events

Log Analysis Process
-The logs were systematically reviewed to detect:
-Repeated failed login attempts
-Unusual access patterns
-Potential brute-force behavior
-Suspicious system activity spikes
Threat Detection Scenarios
-Simulated security incidents included:
-Brute Force Attempt Simulation
-Multiple failed login attempts from a single source
-Identification of potential unauthorized access attempts

Suspicious Activity Detection
-Abnormal login times
-Repeated system access failures
-Unexpected user behavior patterns

Findings Summary
-Key observations from the analysis:
-Failed login attempts may indicate brute-force activity
-Repeated authentication failures require escalation
-Log patterns are critical for early threat detection

Incident Response Actions (Simulated)
-For detected anomalies, the following SOC-style response actions were documented:
-Flagging suspicious IP/activity
-Reviewing affected system logs in detail
-Identifying potential attack patterns
-Recommending mitigation steps (account lockout, monitoring enhancement)

Key Skills Demonstrated
-Security log interpretation
-SOC-style monitoring and alert detection
-Basic threat identification techniques
-Incident reporting and documentation
-Analytical thinking in cybersecurity operations

Key Takeaway
This project demonstrates foundational SOC analyst capabilities in identifying and analyzing security events through log data. It 


simulates real-world monitoring tasks used in Security Operations Centers.
-Future Improvements
-Integrate ELK Stack for centralized logging
-Add automated alert detection scripts
-Simulate advanced persistent threats (APT scenarios)
-Expand into full SIEM-based monitoring lab

5 Report

See [`Sysmon Security Monitoring Lab Report`](Sysmon%20Security%20Monitoring%20Lab%20Report.md)

for full details on setup, findings, and recommendations.

AUTHOR

Tony Nnaemeka- cyber security specialist and SOC Analyst

