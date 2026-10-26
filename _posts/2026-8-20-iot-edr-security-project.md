
---
layout: post
title: "IoT-EDR: Multi-Protocol IoT Security Monitoring and Response"
date: 2026-10-26 19:00:00 +0200
categories: [Projects, Cybersecurity]
tags: [iot-security, edr, suricata, machine-learning, docker, mqtt, coap, soar]
description: "An independent IoT security project combining network intrusion detection, machine-learning anomaly detection, threat intelligence, and automated response."
---

## Overview

**IoT-EDR** is an independent cybersecurity research and implementation project designed to monitor IoT environments, detect suspicious activity, and support automated security responses.

The system combines signature-based network intrusion detection with machine-learning anomaly detection and monitoring of MQTT and CoAP traffic. It runs in a Docker-based lab environment.

**Project Repository:** [View IoT-EDR on GitHub](https://github.com/muhmmod0-max/iot-edr)

## Key Features

- **Multi-Protocol Monitoring:** Security monitoring for MQTT and CoAP traffic.
- **Network Intrusion Detection:** Suricata rules for detecting port scans and flooding attacks.
- **Machine Learning:** Isolation Forest-based anomaly detection for suspicious sensor data.
- **Authentication Monitoring:** Detection of suspicious login attempts and unauthorized MQTT subscriptions.
- **Replay Attack Detection:** Analysis of repeated message patterns.
- **Network Integrity Monitoring:** Detection of potential ARP spoofing and man-in-the-middle activity.
- **Automated Response (SOAR):** Tiered responses, including automatic blocking and escalation of repeated events.
- **Threat Intelligence:** Integration with AbuseIPDB.
- **Secure Communication:** Support for MQTT over TLS.
- **Security Dashboard:** A web interface for reviewing incidents and managing responses.
- **Containerized Deployment:** Docker Compose orchestration for the lab environment.

## Attack Scenarios

The project covers eight detection scenarios:

1. Port scanning and reconnaissance.
2. Malicious sensor-data injection.
3. Brute-force attempts and default credentials.
4. MQTT flooding and DDoS-related activity.
5. Unauthorized MQTT subscriptions.
6. Replay attacks.
7. ARP spoofing and potential MITM activity.
8. CoAP flooding and unauthorized access.

Detection and response depend on the attack scenario and configured rules.

## Technology Stack

| Component | Technologies |
|---|---|
| Network IDS | Suricata |
| IoT Messaging | Eclipse Mosquitto, MQTT, CoAP |
| Anomaly Detection | Python, scikit-learn, Isolation Forest |
| Packet Analysis | Python, Scapy |
| Threat Intelligence | AbuseIPDB |
| Automated Response | Python, SOAR, iptables |
| Dashboard | Flask, Chart.js |
| Storage | SQLite |
| Deployment | Docker Compose |
| Secure Transport | MQTT over TLS |

## What I Learned

Building this project helped me develop practical skills in network security monitoring, attack detection, MQTT security, Docker networking, troubleshooting, and incident response.

It also provided hands-on experience integrating multiple detection methods into a single security monitoring workflow.

## Security Testing Environment

The project was developed for educational and research purposes in an isolated virtual lab. Attack simulations should only be performed against systems and networks that you own or have explicit permission to test.

## Explore the Project

**GitHub Repository:** [github.com/muhmmod0-max/iot-edr](https://github.com/muhmmod0-max/iot-edr)

**Author:** Mahmoud Ijbeerat

Cybersecurity | Network Security | Threat Detection | IoT Security
