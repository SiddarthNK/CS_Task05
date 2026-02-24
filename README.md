# 📡 Task 5 – Capture and Analyze Network Traffic Using Wireshark

## 📌 Problem Statement

Capture live network traffic using Wireshark and analyze different protocols observed during browsing and ping activity. Identify at least three protocols and export the capture file in `.pcap` format.

---

## 🎯 Objective

- Capture live packets
- Identify different protocols
- Apply protocol filters
- Analyze packet details
- Export `.pcap` file

---

## 🛠 Tool Used

- Wireshark (Network Protocol Analyzer)

---

## 🧪 Procedure

### Step 1: Install Wireshark
Downloaded and installed Wireshark from official website.

---

### Step 2: Start Capture

- Open Wireshark
- Select active network interface (Wi-Fi)
- Click Start

![Start Capture](screenshots/01_start_capture.png)

---

### Step 3: Generate Traffic

- Open browser and visit google.com
- Run:

![Live Traffic](screenshots/02_live_traffic.png)

---

### Step 4: Stop Capture

Capture was stopped after 1 minute.

---

### Step 5: Apply Filters

#### DNS Filter

![DNS Filter](screenshots/03_dns_filter.png)

---

#### TCP Filter
![TCP Filter](screenshots/04_tcp_filter.png)

Observed TCP three-way handshake:
- SYN
- SYN-ACK
- ACK

---

#### ICMP Filter
![ICMP Filter](screenshots/05_icmp_filter.png)

Observed:
- Echo Request
- Echo Reply

---

#### HTTP Filter
![HTTP Filter](screenshots/06_http_filter.png)

Observed:
- HTTP GET request
- HTTP 200 OK response

(Note: If HTTPS is used, traffic appears as TLS.)

---

## 🔎 Protocols Identified

| Protocol | Layer | Port | Purpose |
|----------|--------|------|----------|
| DNS | Application | 53 (UDP) | Domain resolution |
| TCP | Transport | Various | Reliable data transfer |
| HTTP | Application | 80 | Web communication |
| ICMP | Network | N/A | Connectivity testing |

---

## 📁 Output File

Export Steps:
File → Export Specified Packets → Save as `.pcap`

---

## ✅ Result

- Successfully captured network traffic.
- Identified DNS, TCP, HTTP, and ICMP protocols.
- Observed TCP handshake and ICMP echo messages.
- Gained practical packet analysis experience.

---

## 🎓 Conclusion

This task improved understanding of:

- Packet structure
- TCP/IP model
- Network protocols
- Wireshark filtering and analysis
