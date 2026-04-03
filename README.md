# Splunk Home Lab: Linux Log Analysis

## 🚀 Overview
This project demonstrates a security monitoring setup using **Splunk Enterprise** running on **Docker**. The goal was to analyze system authentication logs to identify potential security threats and failed login attempts.

## 🛠️ Tech Stack
* **OS:** Ubuntu 24.04 LTS
* **Platform:** Docker
* **SIEM:** Splunk Enterprise
* **Language:** SPL (Search Processing Language)

## 🔍 Key Activities
* **Data Ingestion:** Manually uploaded `/var/log/auth.log` for analysis.
* **Security Monitoring:** Monitored failed login attempts and "authentication failure" events.
* **Log Parsing:** Used SPL to filter events by `user`, `host`, and `event_type`.

## 📈 Search Query Example
index=main "authentication failure" | stats count by user
