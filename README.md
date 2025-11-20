Wireshark Packet Capture & Analysis (Task 5)
🎯 Objective

Capture live network traffic using Wireshark, analyze different protocols, apply filters, and identify key packet details. Export the captured data as a .pcap file and summarize protocol behavior.

🛠 Tools Used

Wireshark (latest version)

Windows/Linux/macOS system

Web browser (for generating traffic)

Command Prompt / Terminal (for ping tests)

📌 Steps Performed
1. Installed Wireshark

Downloaded and installed Wireshark with Npcap support for live packet capturing.

2. Started Packet Capture

Launched Wireshark

Selected active network interface (Wi-Fi/Ethernet)

Started live capture

3. Generated Traffic

Performed actions to generate packets:

Browsed websites (Google, YouTube, etc.)

Ran command:

ping google.com
4. Applied Filters

Used various protocol filters to isolate packets.

5. Analyzed Packets

Inspected individual packet layers including Ethernet, IP, TCP/UDP, DNS, and HTTP.

6. Exported Capture

Saved the captured packets as:

traffic_capture.pcap
🔍 Filters Used
Purpose	Filter
Show DNS packets	dns
Show TCP packets	tcp
Show UDP packets	udp
Show ICMP packets	icmp
Show HTTP packets	http
📊 Protocol Analysis
1. TCP (Transmission Control Protocol)

Connection-oriented

Three-way handshake observed

Reliable delivery with ACK packets

2. UDP (User Datagram Protocol)

Connectionless and faster

No handshake or retransmission

Used for DNS queries

3. DNS (Domain Name System)

Resolves domain names into IP addresses

Observed standard DNS query and response packets

4. HTTP/HTTPS Traffic

HTTP shows readable headers (if not encrypted)

HTTPS appears as TLS-encrypted packets

5. ICMP

Used during ping tests

Echo request and echo reply packets visible

🧪 Findings Summary

Multiple protocols detected including TCP, UDP, DNS, ICMP, and HTTP/HTTPS.

DNS packets showed domain lookups (e.g., google.com).

TCP packets indicated reliable communication with ACKs and SYN/ACK handshake.

HTTPS traffic appeared encrypted through TLS.

Ping tests generated clear ICMP traffic.

📁 Screenshots Included

Screenshots folder contains:

01_wireshark_home.png – Wireshark home interface

02_capture_running.png – Live capture in progress

03_dns_filter.png – DNS filter applied

04_tcp_details.png – TCP packet expanded

05_protocol_hierarchy.png – Protocol hierarchy window

06_pcap_saved.png – Export .pcap file confirmation

✅ Task Output

Completed packet capture

.pcap file exported

Protocol analysis documented

Screenshots captured
