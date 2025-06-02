1. Objective
The purpose of this assignment is to explore live network traffic using Wireshark, a powerful packet analysis tool. By capturing and filtering network packets, the goal is to understand how different network protocols (TCP, DNS, HTTP, ICMP) function in real time. This provides hands-on exposure to core networking concepts.

2. Methodology
The steps followed in this experiment are:

Wireshark was installed on the system.

The active network interface was selected for packet capturing.

Common actions like web browsing and pinging were performed to generate traffic.

The capture was stopped after about one minute.

Filters like tcp, dns, http, and icmp were applied to isolate specific protocols.

Screenshots were taken for each filter.

Packet details (source, destination, flags, TTL, payload) were examined.

A report was created documenting the results and protocol analysis.

3. Screenshots and Filters
The following protocol filters were applied, and relevant screenshots were taken:

Protocol	Filter Applied	Observations
TCP	tcp	Detected TCP handshake and data transmission
DNS	dns	Domain name queries and responses were visible
HTTP	http	Web GET requests and responses captured
ICMP	icmp	No traffic observed (likely blocked)

Screenshots are included in the “filters/” and “packet-info/” folders.

4. Protocol Analysis
DNS Packets: Revealed domain name queries and their resolved IP addresses. For example, example.com resolved using a DNS query packet.

HTTP Packets: GET requests made to load websites, showing typical HTTP headers and responses over port 80.

TCP Packets: Showed connection establishment via 3-way handshake (SYN, SYN-ACK, ACK) and reliable data transfer.

ICMP Packets: No ICMP traffic was recorded in the capture, suggesting ICMP echo requests were either not sent or blocked.

5. Conclusion
Wireshark enables in-depth visibility into live network activity. Through this assignment, key network protocols were captured, filtered, and examined. The exercise improved understanding of how common internet services (web browsing, domain resolution) interact at the packet level. Wireshark’s filtering capability makes it an indispensable tool for learning and diagnosing network issues.

6. Interview Questions and Answers
Q1. What is Wireshark used for?
Wireshark is a network protocol analyzer used to capture and analyze network traffic.

Q2. What is a packet?
A packet is a small unit of data transmitted over a network that includes headers and payload.

Q3. How to filter packets in Wireshark?
Use display filters like tcp, http, dns in the filter bar.

Q4. What is the difference between TCP and UDP?
TCP is connection-based and reliable; UDP is connectionless and faster but less reliable.

Q5. What is a DNS query packet?
It’s a request to resolve a domain name (like google.com) into its IP address.

Q6. How can packet capture help in troubleshooting?
It can reveal dropped packets, misrouted traffic, and performance issues.

Q7. What is a protocol?
A protocol is a set of rules for communication between network devices (e.g., TCP, HTTP).

Q8. Can Wireshark decrypt encrypted traffic?
Only if encryption keys or SSL handshake logs are available; otherwise, encrypted traffic remains unreadable.
