# cybersec-portfolio
A collection of cybersecurity projects showcasing my learning and hands-on experience.
# Wireshark Packet Analysis — Network Traffic Inspection

##  Overview
This project demonstrates how to capture and analyze network packets using **Wireshark**, one of the most powerful tools for network analysis.  
The goal was to observe how data travels across the network and understand the structure of HTTP traffic between a computer and a web server.

---

##  Objective
To use Wireshark to capture real-time internet traffic, identify protocols, and interpret what happens when a web page is requested or loaded.

---

##  Tools Used
- **Wireshark v4.6.0**
- **Windows 10 x64**
- **Web Browser (for generating traffic)**

---

##  Steps Taken
1. Installed Wireshark on the system.  
2. Selected the **Wi-Fi** network interface for packet capture.  
3. Started the capture while visiting a website.  
4. Stopped the capture after several seconds of activity.  
5. Applied the filter `http` to focus on HTTP communication packets.  
6. Inspected the details of one packet to view its source, destination, and content.  
7. Documented findings and observations.

---

##  Findings
The captured packet (Frame 7602) showed:
- **Protocol:** HTTP  
- **Source IP:** Local device (e.g. `2600:1408:...`)  
- **Destination IP:** Web server (e.g. `2001:818:e3cd:...`)  
- **Content Type:** `text/html`  
- **Summary:** The packet contained HTML data transferred between a browser and a server, part of a web page request/response.

This confirms that network traffic contains readable information (in cleartext) if the protocol isn’t encrypted — which is a key cybersecurity concept.

---

##  Explanation
When you browse the internet, your computer sends small units of data called **packets** to websites.  
Wireshark allows us to capture and view these packets to see what’s being transmitted in real time.

In this project:
- The captured packet shows a **HTTP request and response** between the local system and a remote web server.  
- It contains information like **headers**, **content type**, and **data length**, which define how data is sent.  
- This helps cybersecurity professionals identify unusual traffic, detect attacks, or troubleshoot network issues.

---

## 📊 Screenshot Evidence
<img width="1365" height="714" alt="Screenshot 2025-11-10 165711" src="https://github.com/user-attachments/assets/aa2d1f84-dbe5-4cc9-8613-31fb565596ac" />
<img width="1365" height="714" alt="Screenshot 2025-11-10 165358" src="https://github.com/user-attachments/assets/adec131a-5e66-4ee9-91a9-5549fe40474a" />
<img width="1365" height="700" alt="Screenshot 2025-11-10 165335" src="https://github.com/user-attachments/assets/0d13906e-a179-494f-adda-6ae092df2e53" />
<img width="1362" height="707" alt="Http findings" src="https://github.com/user-attachments/assets/33148b20-96c1-4e71-a6e7-e86c436855cd" />

##  Conclusion
This project demonstrates how Wireshark can capture, analyze, and interpret network packets.  
Understanding how traffic flows is an essential cybersecurity skill for:
- Network monitoring  
- Incident response  
- Detecting suspicious activity

---

## 🧑🏽‍💻 Author
**Ruth Campbell**  
Cybersecurity Student | Network Enthusiast  
📍 Lisbon, Portugal
