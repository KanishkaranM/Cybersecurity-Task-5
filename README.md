# Task 5 – Wireshark Packet Capture & Analysis

## 🎯 Objective
Capture live network packets using Wireshark and analyze basic network protocols such as TCP, UDP, DNS, and HTTP.

---

## 🛠 Tools Used
- Wireshark (Latest Version)
- Windows 10/11 Laptop
- Command Prompt (for ping testing)

---

## 📌 Steps Performed

### 1. Installed Wireshark
Downloaded from the official website and installed with Npcap support.

### 2. Started Packet Capture
Selected the active Wi-Fi adapter and began capturing live packets.

### 3. Generated Network Traffic
- Browsed Google and YouTube
- Used command: `ping google.com`

### 4. Applied Filters
Used:
- `dns`
- `tcp`
- `http`
- `udp`

### 5. Identified Protocols
Found:
- **TCP** – Reliable transport
- **UDP** – Fast, connectionless transport
- **DNS** – Domain name resolution
- **HTTP/HTTPS** – Web browsing traffic
- **ICMP** – Ping echo requests

### 6. Exported Capture
Saved as: `traffic_capture.pcap`

---

## 📊 Findings Summary

### ✔ TCP Traffic
- Three-way handshake observed.
- Multiple acknowledgment packets.

### ✔ UDP Traffic
- Faster, no handshake.
- Used by DNS queries.

### ✔ DNS Packets
- Queried domains like google.com
- Request/response structure visible.

### ✔ HTTP/HTTPS Traffic
- Encrypted TLS packets for HTTPS.

---

## 📁 Repository Structure

