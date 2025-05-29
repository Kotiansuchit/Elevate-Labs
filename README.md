# Elevate-Labs
TASK 1


# 🔐 Network Scanning and Traffic Analysis using Nmap & Wireshark

## 📌 Project Overview

This project demonstrates the practical use of **Nmap** (Network Mapper) for scanning live hosts and open ports within a network and **Wireshark** for capturing and analyzing network traffic. The goal is to understand how scanning activity appears on the wire and to visualize real-time data communication from a host device.

---

## 📁 Tools Used

- **Nmap**: A network scanning tool used to identify hosts and services.
- **Wireshark**: A packet analyzer used for real-time network traffic capture and analysis.
- **Windows CMD / PowerShell**: For network interface checks and IP configuration.

---

## 🧪 Objective

- Scan a local network to identify active hosts and open ports using Nmap.
- Capture and analyze network packets (HTTP and QUIC) generated during or after scanning.
- Learn how scanning and browsing activities manifest at the packet level.

---

## 🖥️ Environment Setup

### ✅ System Used
- OS: Windows 10/11
- Local IP: `192.168.0.106`
- Wi-Fi Network with Gateway: `192.168.0.1`

---

## 🔍 Nmap Scanning Procedure

### Step 1: Identify Your IP Address
```bash
ipconfig
Step 2: Run Nmap to Scan the Local Network
bash
Copy
Edit
nmap -sP 192.168.0.0/24 -oN scan_result.txt
Output
Lists active hosts on the subnet.

Stores result in scan_result.txt.

🧪 Wireshark Packet Capture Procedure
Step 1: Start Wireshark
Choose the active Wi-Fi adapter.

Step 2: Apply Filter
bash
Copy
Edit
ip.addr == 192.168.0.106 && tcp.port == 80
Step 3: Perform Browsing / Scanning Activity
Use a browser or run Nmap while Wireshark is capturing.

Step 4: Stop Capture and Analyze
Observe QUIC, TCP, and possibly HTTP traffic.

Analyze packet content and payloads.

🖼️ Example Output
Wireshark Captured Traffic:
Source: 192.168.0.106

Destination: 142.250.183.100 (Google Server)

Protocol: QUIC, TCP

Port: 80

Status: Data exchanged with ACKs, Handshakes, and Payloads.




TASK2

# 📧 Phishing Email Analysis – Task 2

## 🔍 Project Title
**Phishing Email Header and Body Analysis for Cybersecurity Awareness**

## 📄 Project Description
This project focuses on analyzing a suspicious email that mimics a government notification regarding a FaceTime vulnerability. The goal is to demonstrate how to identify phishing indicators using both manual inspection and security tools.

## 🎯 Objectives
- Understand the structure of phishing emails
- Analyze email headers for spoofing or forged information
- Use tools to detect phishing techniques
- Generate a detailed technical report with findings
- Create awareness of phishing threats

## 🧰 Tools Used
| Tool | Purpose |
|------|---------|
| **MXToolbox** | Email header analysis
## 🧪 Steps Followed

1. **Collected a Sample Phishing Email**  
   - Subject: *Apple Facetime Information Disclosure*
   - Spoofed sender: “National Security Department”  
   - Contained a suspicious link disguised as a “verification” page

2. **Email Header Analysis**  
   - Used MXToolbox & Google's Message Header Analyzer  
   - Identified inconsistencies in Return-Path and sender IP  
   - Verified mismatch in domain ownership

3. **Body Analysis**  
   - Detected social engineering tactics (urgency, fear, and time pressure)  
   - No personalized greeting or contact details  
   - Link embedded in a “Facetime Verification” button

4. **Generated Screenshot of Email**  
   - Created realistic-looking phishing email screenshot for training/demo purposes

5. **Created a Detailed Report**  
   - Summarized header details, phishing indicators, and recommended actions  
   - Compiled into a downloadable document

## ✅ Outcome
- Successfully identified phishing indicators in the email
- Demonstrated usage of tools for header and link analysis
- Created a training-style phishing simulation email
- Report generated for academic or training documentation

## 📁 Files Included
- `Phishing_Email_Analysis_Report.docx` – Final analysis report
- `phishing_email_screenshot.png` – Simulated email screenshot
- `README.md` – Project documentation

## 🛡️ Recommendations
- Never trust urgent emails with links from unknown senders
- Use technical tools to validate suspicious emails
- Educate users regularly on common phishing tactics
