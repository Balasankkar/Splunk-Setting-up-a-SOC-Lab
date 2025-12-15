# 🧩 Lab 1 — Introduction 

In this project, I will be setting up **Splunk Enterprise** as the central SIEM platform for collecting, analyzing, and correlating security logs in real-time. This project will cover installing Splunk on Linux/Windows and configuring different log sources from both OS into Splunk. Each lab covers the following topics:

---

## ⚙️ Linux Lab

Tasks:
- Install **Splunk Enterprise** on the Ubuntu server.  
- Install and configure the **Splunk Universal Forwarder**.  
- Collect logs from key sources such as:
  - `/var/log/syslog`
  - `/var/log/auth.log`
  - `/var/log/audit/audit.log`
- Verify that all Linux logs are being forwarded and indexed properly in Splunk.

---

## 🪟 Windows Lab

Tasks:
- Install **Splunk Enterprise** on a Windows machine.  
- Install and configure the **Splunk Universal Forwarder**.  
- Integrate and monitor:
  - **Windows Event Logs** (Application, Security, and System)  
  - **Coffely web logs** (THM’s internal web server logs)
- Confirm that events are visible and searchable from the Splunk dashboard.

---
