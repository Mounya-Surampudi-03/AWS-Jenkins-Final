# AWS Jenkins Monitoring & Automated Alerting System using CloudWatch and SNS

## 📌 Project Overview
This project demonstrates how to monitor Jenkins availability on an AWS EC2 instance using a custom Bash script, automate monitoring using cron jobs, and trigger alerts using AWS CloudWatch and SNS when Jenkins goes down.

---

## 🎯 Objective
- Monitor Jenkins status (UP/DOWN)
- Automate health checks using cron
- Capture logs for analysis
- Send real-time email alerts on failure using AWS services

---

## 🛠 Tools & Technologies
- AWS EC2 (Ubuntu 22.04)
- Jenkins
- Bash Scripting
- Cron Jobs
- AWS CloudWatch
- AWS SNS (Simple Notification Service)
- IAM Roles

---

## 🏗️ Architecture
- EC2 hosts Jenkins server
- Monitoring script checks Jenkins availability
- Logs are sent to CloudWatch
- CloudWatch triggers alarms on failure
- SNS sends email alerts to users

---

## ⚙️ Implementation Steps

### ✅ 1. EC2 Setup
- Launch Ubuntu 22.04 instance
- Open ports: 22 (SSH), 8080 (Jenkins)

### ✅ 2. Install Dependencies
- Install Java (required for Jenkins)
- Install Jenkins and access via browser

### ✅ 3. Jenkins Setup
- Unlock Jenkins using initial admin password
- Install plugins and access dashboard

### ✅ 4. Monitoring Script
- Create Bash script to check Jenkins status
- Store output logs (UP/DOWN)

### ✅ 5. Automation using Cron
- Schedule script execution at regular intervals
- Verify logs for continuous monitoring

### ✅ 6. Failure & Recovery Testing
- Stop Jenkins service → detect DOWN
- Restart Jenkins → detect UP

### ✅ 7. CloudWatch Integration
- Create IAM role for EC2
- Install and configure CloudWatch agent
- Send logs to CloudWatch

### ✅ 8. Log Monitoring
- Create metric filters from logs
- Convert logs into CloudWatch metrics

### ✅ 9. Alerting System
- Create CloudWatch Alarm for Jenkins downtime
- Configure SNS topic and email subscription

### ✅ 10. Alert Trigger
- Stop Jenkins service
- CloudWatch alarm triggers
- SNS sends email notification

---

## 📊 Key Features
- Automated Jenkins health monitoring
- Real-time failure detection
- Cloud-based log tracking
- Instant email alerts via SNS
- Minimal manual intervention

---

## 📄 Documentation
Detailed step-by-step implementation is available in:
- 📄 PDF file

---

## ✅ Outcome
Successfully implemented a monitoring and alerting system that detects Jenkins downtime and notifies users via email automatically.

---

## 🚀 Conclusion
This project ensures high availability monitoring of Jenkins using AWS services, combining automation, logging, and alerting to create a reliable DevOps solution.

---
``
