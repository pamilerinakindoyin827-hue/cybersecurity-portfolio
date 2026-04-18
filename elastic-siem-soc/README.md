# Cloud SOC Deployment using Elastic SIEM (AWS & Windows)

## Overview
This project demonstrates the deployment of a Security Operations Center (SOC) environment using Elastic SIEM to monitor cloud and endpoint activity, detect threats, and investigate security incidents.

The environment simulates real-world SOC operations by ingesting AWS logs, configuring detection rules, integrating threat intelligence, and validating alerts through controlled attack simulations.

---

## Objectives
- Deploy and configure Elastic SIEM for centralized security monitoring  
- Ingest and analyze AWS logs (CloudTrail, EC2, VPC Flow Logs)  
- Integrate threat intelligence using AlienVault OTX  
- Create and validate detection rules for security events  
- Perform basic endpoint forensics using Windows Event Viewer  

---

## Tools & Technologies
- Elastic SIEM (Kibana)  
- AWS (EC2, CloudTrail, VPC Flow Logs)  
- AlienVault OTX (Threat Intelligence)  
- Windows Event Viewer  
- Security detection rules and log analysis  

---

## Implementation

### 1. Environment Setup
- Deployed Elastic SIEM instance for centralized log monitoring  
- Configured ingestion of AWS logs:
  - CloudTrail logs  
  - EC2 system logs  
  - VPC Flow Logs  
- Integrated AlienVault OTX for threat intelligence enrichment  

---

### 2. Detection Engineering
- Enabled built-in AWS security detection rules:
  - IAM Group Creation  
  - IAM User Added to Group  
  - SSH Authentication Events  
- Developed a custom detection rule to monitor SSH activity on port 22  
- Verified rule triggering through controlled testing  

---

### 3. Attack Simulation
- Simulated IAM privilege escalation activity in AWS  
- Created IAM users and groups with administrative permissions  
- Performed SSH access to EC2 instance  
- Validated detection of all simulated activities in Elastic SIEM  

📊 Results:
- Alerts generated successfully for all test scenarios  
- Each alert included timestamp, rule name, and event details  

---

### 4. Endpoint Forensics (Windows)
- Deployed Windows instance for endpoint monitoring  
- Used Event Viewer to analyze system logs  
- Created custom view for Event ID 1102 (Security Log Cleared)  
- Simulated log clearing activity for detection validation  

 Results:
- Event ID 1102 successfully detected and recorded  
- Activity logged and visible in system event history  

---

## Incident Summary

**Timeline:**
- IAM activity simulation: Feb 2, 2026  
- SSH access event: Feb 2, 2026  
- Security log clearing event: Feb 10, 2026  

**Detection Summary:**
- AWS IAM changes detected successfully  
- SSH activity detected via custom detection rule  
- Windows log clearing activity detected (Event ID 1102)  

**Assessment:**
- Controlled lab environment  
- No real-world risk exposure  
- No false negatives observed during testing  

---

## Key Security Insights
- SIEM systems are critical for detecting unauthorized cloud activity  
- Monitoring SSH access is essential in cloud environments  
- Event ID 1102 is a strong indicator of potential log tampering  
- Threat intelligence improves detection accuracy and context  
- Combining cloud + endpoint logs provides full visibility  

---

## Evidence
This project includes supporting evidence such as:
- Elastic SIEM dashboards showing detected alerts  
- AWS security event logs  
- Custom detection rule outputs  
- Windows Event Viewer logs (Event ID 1102)  

All evidence demonstrates successful detection and monitoring of simulated security incidents.

---

## Conclusion
This project demonstrates hands-on experience in building a functional SOC environment using Elastic SIEM. It showcases practical skills in cloud security monitoring, threat detection, incident analysis, and endpoint forensics.

It reflects real-world SOC workflows including log ingestion, detection engineering, and security event investigation.
