# Network-Anomaly-Detection-Wireshark
This project focuses on detecting suspicious devices and identifying anomalous network behavior using Wireshark and Nmap within a local network.
# Network Anomaly Detection using Wireshark & Nmap

## Overview

This project focuses on detecting suspicious devices and identifying anomalous network behavior using Wireshark and Nmap within a local network.

## Objectives

* Identify all active devices in the network
* Establish a baseline of known devices
* Detect unknown or unauthorized devices
* Analyze network traffic for anomalies
* Identify unusual ports and communication patterns

## Tools Used

* Wireshark
* Nmap
* Windows Command Prompt

## 🔍 Methodology

### 1. Device Discovery

Used Nmap to identify active devices:

nmap -sn 192.168.0.0/24

### 2. Baseline Creation

Classified devices as known (router, laptop, phone).

### 3. Traffic Capture

Captured traffic using Wireshark:

ip.addr == 192.168.0.0/24

### 4. ARP Analysis

Filtered ARP replies:

arp.opcode == 2

### 5. DNS Monitoring

dns

### 6. Unusual Traffic Detection

Filtered non-standard ports:

!(tcp.port == 80) && !(tcp.port == 443)

## Key Findings

* Identified active devices including router and host machine
* Observed ARP-based device discovery
* Detected background system traffic (Windows Update on port 7680)
* Identified multicast traffic (mDNS – 224.0.0.251)
* Majority of traffic was encrypted (HTTPS)

## Security Analysis

* No unknown devices detected
* No suspicious ports or malicious activity observed
* Network traffic patterns were normal

## Conclusion

The network environment appears secure with no anomalies detected. Background system and multicast traffic were identified and classified as normal.

## Learning Outcomes

* Understanding ARP-based device discovery
* Identifying normal vs abnormal traffic patterns
* Analyzing ports and protocols
* Basic anomaly detection techniques

## Screenshots
<img width="1920" height="1080" alt="6" src="https://github.com/user-attachments/assets/76385e03-843b-43b7-9083-fb9656b89492" />
<img width="1920" height="1080" alt="5" src="https://github.com/user-attachments/assets/abd58bf0-dd72-4c76-a84e-0045f7d272af" />
<img width="1920" height="1080" alt="4" src="https://github.com/user-attachments/assets/94a21d5a-52ab-423c-be06-a397581609ce" />
<img width="1920" height="1080" alt="3" src="https://github.com/user-attachments/assets/5488d2e9-d001-45e6-956c-34b4eb2b9b5f" />




