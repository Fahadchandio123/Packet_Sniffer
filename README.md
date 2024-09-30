# Packet_Sniffer
Overview
This project is a Packet Sniffer written in Python that captures and analyzes network traffic in real-time. Packet sniffers are powerful tools used in cybersecurity to monitor network activity, detect unusual behavior, and analyze the data transmitted through a network interface.

GitHub Repository: Packet Sniffer

Features
Real-time Packet Capture: Captures incoming and outgoing packets on the network.
Protocol Analysis: Supports common protocols like TCP, UDP, and ICMP, and provides detailed packet information.
Easy-to-Read Output: Displays captured packet details in a human-readable format.
Requirements
To run this project, you’ll need:

Python 3.x
Admin/root privileges (to capture network packets)
The socket module (included in Python's standard library)
Installation
Clone the repository to your local machine:

bash
Copy code
git clone https://github.com/Fahadchandio123/Packet_Sniffer.git
Navigate to the project directory:

bash
Copy code
cd Packet_Sniffer
Run the packet sniffer with administrator privileges:

bash
Copy code
sudo python3 packet_sniffer.py
Note: Administrator or root privileges are required to capture network traffic.

How It Works
The packet sniffer listens for network packets and captures each one as it passes through the network interface. It breaks down the packet’s structure, displaying details such as:

Source and destination IP addresses
Protocol type (e.g., TCP, UDP, ICMP)
Source and destination ports
Packet size and flags
Example Output
yaml
Copy code
Ethernet Frame:
- Destination MAC: ff:ff:ff:ff:ff:ff
- Source MAC: 00:1b:44:11:3a:b7
- Protocol: IPv4

IP Packet:
- Source IP: 192.168.1.100
- Destination IP: 192.168.1.1
- Protocol: TCP

TCP Packet:
- Source Port: 80
- Destination Port: 52345
- Sequence: 123456789
- Flags: SYN, ACK
Customization
You can customize the packet sniffer by modifying the script to:

Capture specific types of packets (e.g., only TCP or UDP)
Filter by IP address or port
Save the captured packet data to a file for further analysis
Future Enhancements
Some potential improvements include:

Adding a filtering option for specific IP addresses or ports.
Allowing packet export to a file for post-analysis.
Enhancing the display for protocol-specific analysis.
License
This project is licensed under the MIT License. See the LICENSE file for more details.
