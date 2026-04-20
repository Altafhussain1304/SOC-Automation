# SOC Automation & Threat Monitoring System

## 🔹 Overview

This project demonstrates the implementation of a Security Operations Center (SOC) environment for real-time threat detection, analysis, and automated response.

The system integrates SIEM and SOAR technologies to detect malicious activities and automate incident response workflows.

---

## 🔹 Tech Stack

* Wazuh (SIEM for log collection & correlation)
* Sysmon (Windows endpoint monitoring)
* TheHive (Incident response & case management)
* Shuffle (SOAR - Security Orchestration Automation & Response)
* Mimikatz (Attack simulation - credential dumping)

---

## 🔹 Architecture

The SOC pipeline follows this flow:

1. Sysmon collects system activity from Windows endpoint
2. Logs are forwarded to Wazuh agent
3. Wazuh analyzes logs using rules and detects suspicious activity
4. Alerts are sent to TheHive for incident creation
5. Shuffle automates response actions (alert enrichment, response)

(Add architecture diagram image here)

---

## 🔹 Features

* Real-time log monitoring and analysis
* File Integrity Monitoring (FIM)
* Detection of credential dumping attacks
* Automated incident creation in TheHive
* Alert enrichment and response using Shuffle
* Active response (blocking malicious activity)

---

## 🔹 Attack Simulation (Mimikatz)

* Executed credential dumping using Mimikatz
* Sysmon generated logs for process activity
* Wazuh detected suspicious behavior
* Alert triggered based on rule matching
* Incident created in TheHive
* Shuffle automated the response workflow

---

## 🔹 Detection Logic

Wazuh detects malicious activity using:

* Predefined rules
* Custom rules (if added)
* Sysmon event logs (Process creation, access events)

Example:

* Detection triggered when suspicious process behavior matches known attack patterns

---

## 🔹 Screenshots


<img width="3795" height="1688" alt="image" src="https://github.com/user-attachments/assets/3188038f-b30b-4211-99e2-4009bf5797e5" />
<img width="3803" height="1671" alt="image" src="https://github.com/user-attachments/assets/2f26dd6f-0dd1-4ee6-a729-692d273ee4dd" />


---

## 🔹 Project Structure

```bash
SOC-Automation-Project/
│── README.md
│── architecture/
│── configs/
│── scripts/
│── screenshots/
│── docs/
```

---

## 🔹 Future Improvements

* AI-based threat detection
* Cloud SIEM integration
* Advanced correlation rules
* Threat intelligence integration

---

## 🔹 Conclusion

This project demonstrates how SOC operations can be automated to reduce manual effort and improve incident response time using SIEM and SOAR tools.

---

## 🔹 Author

Mohammed Altaf Hussain
