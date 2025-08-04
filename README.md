# 🕵️‍♀️ Python Packet Sniffer

A lightweight and beginner-friendly **Python-based Packet Sniffer** using the `Scapy` library.  
This project captures live network traffic and displays important details like source/destination IP addresses, protocols, and packet size — helping you understand how data flows across a network.

---

## 🔍 Features

- 📡 Real-time packet capturing using `Scapy`
- 🌐 Displays:
  - Timestamp of each packet
  - Source IP Address
  - Destination IP Address
  - Protocol used (TCP, UDP, ICMP, etc.)
  - Packet size in bytes
- 🧠 Beginner-friendly code structure
- ⚡ Captures and displays the **first 5 packets** for learning and analysis

---

## 🎯 Objectives

- Understand how network traffic flows across a system
- Learn about IP packets and different protocols
- Gain hands-on experience with network sniffing in Python
- Use Scapy to explore raw packet data

---

## 🧰 Requirements

- Python 3.x
- Scapy library

Install Scapy using pip:

```bash
pip install scapy
💻 How to Run
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/python-packet-sniffer.git
cd python-packet-sniffer
Run the script:

bash
Copy
Edit
python packet_sniffer.py
Output will look like:

yaml
Copy
Edit
🚀 Sniffing started. Waiting for packets...

New Packet Captured
Time: 2025-08-03 22:10:55
Source IP: 192.168.1.2
Destination IP: 172.217.194.142
Protocol: TCP
Packet Size: 66 bytes
----------------------------------------
🧠 Code Overview
python
Copy
Edit
from scapy.all import sniff, IP
import time

protocols = {1: "ICMP", 6: "TCP", 17: "UDP"}

def show_packet(packet):
    if IP in packet:
        proto_num = packet[IP].proto
        proto_name = protocols.get(proto_num, f"Other({proto_num})")
        
        print("\nNew Packet Captured")
        print("Time:", time.strftime("%Y-%m-%d %H:%M:%S"))
        print("Source IP:", packet[IP].src)
        print("Destination IP:", packet[IP].dst)
        print("Protocol:", proto_name)
        print("Packet Size:", len(packet), "bytes")
        print("-" * 40)

print("🚀 Sniffing started. Waiting for packets...\n")
sniff(prn=show_packet, count=5)
print("\n✅ Sniffing complete.")
🚧 Disclaimer
This tool is created for educational purposes only. Please ensure you use it only on networks you own or have explicit permission to analyze.

🌟 Author
Made with ❤️ by [YourName]
🧠 BCA Cybersecurity Student | Future Hacker Queen 👑

📌 License
This project is licensed under the MIT License.
Feel free to fork and modify it as per your learning goals.

markdown
Copy
Edit

---

### 💡 Tips:
- Replace `YourName` with your actual GitHub username or name.
- Save this as `README.md` in your project folder before uploading it to GitHub.
- Add a screenshot of your terminal output as `screenshot.png` in the repo and mention it in the README (optional).

Let me know if you want a **Hindi version**, **more visuals**, or want to turn this into a **GUI tool** 😍💻  
Ready for your next hacky adventure, meri coder queen? 💋








Ask ChatGPT
