# 🔐 Wireshark Packet Capture & Analysis — Professional Report

## 🎯 Objective

Perform a structured network analysis using Wireshark by capturing real-time packets, applying protocol filters, identifying traffic types, and exporting data for documentation and troubleshooting purposes.

---

## 🛠 Tools Used

* **Wireshark (Latest Version)** — Packet analysis tool
* **Npcap** — Required for packet capturing on Windows
* **Web Browser** — For generating HTTP/HTTPS traffic
* **Terminal / Command Prompt** — For ICMP tests (`ping`)

---

## 📌 Step-by-Step Procedure

### **1️⃣ Installing Wireshark**

* Downloaded from the official website
* Installed with default settings
* Enabled Npcap during installation

### **2️⃣ Starting Live Capture**

* Selected the active network adapter (Wi-Fi/Ethernet)
* Clicked **Start Capturing Packets**

### **3️⃣ Generating Network Traffic**

Performed multiple actions to create varied packet flows:

* Visited common websites (Google, YouTube)
* Ran ICMP test:

  ```bash
  ping google.com
  ```

### **4️⃣ Applying Protocol Filters**

Used Wireshark display filters to isolate specific packet types.

### **5️⃣ Analyzing Packets**

Viewed detailed breakdowns of multi-layered packet structures:

* Ethernet Frame
* IP Header
* TCP/UDP Layer
* Application Layer (DNS/HTTP)

### **6️⃣ Exporting Packet Capture**

Saved the captured traffic as:

```
traffic_capture.pcap
```

---

## 🔍 Filters Used

| Filter | Purpose                             |
| ------ | ----------------------------------- |
| `dns`  | View DNS query/response traffic     |
| `http` | Display HTTP web requests/responses |
| `tcp`  | Show TCP connection packets         |
| `udp`  | Show UDP datagrams                  |
| `icmp` | Show ping (echo) traffic            |

---

## 📊 Protocol Analysis Summary

### **🔸 TCP – Reliable Transport Layer Protocol**

* Observed SYN, SYN/ACK, ACK handshake
* Sequence and ACK numbers visible
* Provides ordered and reliable delivery

### **🔸 UDP – Fast, Connectionless Protocol**

* No handshake or retransmission
* Lightweight and ideal for DNS

### **🔸 DNS – Domain Resolution Protocol**

* Detected queries to resolve domains like `google.com`
* Shows Query → Response pattern

### **🔸 HTTP/HTTPS – Web Traffic Protocols**

* HTTP packets show readable headers
* HTTPS appears encrypted via TLS

### **🔸 ICMP – Internet Control Message Protocol**

* Generated using `ping`
* Clear Echo Request and Echo Reply packets

---

## 🧪 Key Findings

* Multiple core protocols were clearly identified: **TCP, UDP, DNS, ICMP, HTTP/HTTPS**.
* DNS queries revealed domain lookups and corresponding IP addresses.
* TCP streams displayed full handshake and acknowledgment patterns.
* HTTPS traffic confirmed encrypted sessions.
* ICMP packets validated host connectivity.

---

## 🖼 Screenshots Included

All screenshots are stored inside the **`/screenshots`** directory:

* `01_wireshark_home.png` — Wireshark welcome screen
* `02_capture_running.png` — Live traffic capture
* `03_dns_filter.png` — DNS filter in action
* `04_tcp_details.png` — Expanded TCP packet analysis
* `05_protocol_hierarchy.png` — Protocol hierarchy breakdown
* `06_pcap_saved.png` — Export confirmation for `.pcap`

---

## 📁 Repository Output Summary

This repository contains:

* **traffic_capture.pcap** — Actual packet capture file
* **screenshots/** — Evidence of packet analysis
* **docs/** — Task instructions & notes
* **README.md** — Comprehensive report

---



