# <h1>Python Packet Sniffer</h1>

<h3>A lightweight and beginner-friendly **Python-based Packet Sniffer** using the `Scapy` library.<br>  
This project captures live network traffic and displays important details like source/destination IP addresses, protocols, and packet size — helping you understand how data flows across a network.</h3>

---

<h1>Features</h1>

-  Real-time packet capturing using `Scapy`
-  Displays:
  - Timestamp of each packet
  - Source IP Address
  - Destination IP Address
  - Protocol used (TCP, UDP, ICMP, etc.)
  - Packet size in bytes
-  Beginner-friendly code structure
- Captures and displays the **first 5 packets** for learning and analysis

---

<h1>Objectives</h1>

- Understand how network traffic flows across a system
- Learn about IP packets and different protocols
- Gain hands-on experience with network sniffing in Python
- Use Scapy to explore raw packet data

---

<h1>Requirements</h1>

- Python 3.x
- Scapy library

Install Scapy using pip:

```bash
pip install scapy
```
---

<h1>How to Run</h1> 
Clone the repository:

```bash

git clone https://github.com/your-username/python-packet-sniffer.git
cd python-packet-sniffer
```
 ---
 
<h1>Run the script:</h1>

```bash

python packet_sniffer.py
```
---

<h1>Output will look like:</h1>

<p>Sniffing started. Waiting for packets...<br>

New Packet Captured<br>
Time: 2025-08-03 22:10:55<br>
Source IP: 192.168.1.2<br>
Destination IP: 172.217.194.142<br>
Protocol: TCP<br>
Packet Size: 66 bytes<br>
----------------------------------------<br></p>


---

<h1>Disclaimer</h1>
This tool is created for educational purposes only. Please ensure you use it only on networks you own or have explicit permission to analyze.

---

<h1>Author</h1>
Made with by Mumuksha Kashyap<br>
BCA Cybersecurity Student  


---

<h1>License</h1>
This project is licensed under the MIT License.<br>
Feel free to fork and modify it as per your learning goals.
