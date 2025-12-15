# 🧠 Full SIEM & SOC Lab — Splunk Implementation (Coffely Scenario)

A hands-on cybersecurity project simulating the deployment and configuration of a full **Security Information and Event Management (SIEM)** and **Security Operations Center (SOC)** environment using **Splunk**. This lab replicates an enterprise-style monitoring setup and demonstrates a complete SOC workflow.

---

## ☕ Scenario: The Coffely Case

This lab is based on the **TryHackMe Splunk Lab**, which introduces a fictional company, **Coffely**, facing an insider data breach.  

After the breach, Coffely decided to build an **in-house SOC** to continuously monitor security logs and detect malicious activities within its network. The SOC team selected **Splunk** as their SIEM platform to establish centralized visibility across Windows and Linux systems.

As a security engineer, I was tasked with:
- Setting up **Splunk Enterprise** locally  
- Configuring log ingestion from both **Linux and Windows endpoints**  
- Implementing **forwarders and listening ports** for log transport  

---

## ⚙️ Lab Overview

| Component | Description |
|------------|-------------|
| **SIEM Platform** | Splunk Enterprise |
| **Operating Systems** | Ubuntu (Linux) and Windows 10 |
| **Log Sources** | Sysmon, Windows Event Logs, Auth Logs, System Logs, Web Logs |
| **Data Transport** | Universal Forwarder, TCP/UDP listening ports |
| **Objective** | Establish a working SIEM setup to monitor, visualize, and correlate multi-source security events |

---

## 🧩 Project Objectives

- **Deploy and configure Splunk** on both Linux and Windows hosts.  
- **Ingest logs** from multiple systems and normalize data for analysis.  
- **Visualize data** through dashboards and correlation searches.  

---

## 🧰 Tools and Technologies

| Category | Tools Used |
|-----------|------------|
| **SIEM Platform** | Splunk Enterprise |
| **Log Sources** | Sysmon, Windows Event Logs, Linux Auth Logs, Web Logs |
| **Data Collection** | Splunk Universal Forwarder, Syslog |
| **Threat Detection** | Custom SPL Queries, Correlation Searches |
| **Virtualization** | VirtualBox / VMware Workstation |

---

## 🧠 Learning Outcomes

- Gained hands-on experience configuring **Splunk SIEM** in a hybrid environment.  
- Learned to **ingest and parse multi-source security logs**.  
- Practiced **building correlation searches** to detect attack patterns.  
- Understood **SOC workflows** — alert generation, triage, and reporting.

---


