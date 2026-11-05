# Cyber Security Internship – Task 1

## Local Network Open Port Scanning Using Nmap

### Objective
To identify active devices and open ports on a local network using Nma


### Tools Used
- Kali Linux
- Nmap
- Wireshark (Optional)

### Practical Implementation

**1. Check IP Address**
```bash
ip -4 addr
```

**2. Check Network Configuration**
```bash
ip route
```

**3. Discover Active Devices**
```bash
sudo nmap -sn 192.168.50.0/24
```

**4. Perform TCP SYN Scan**
```bash
sudo nmap -sS 192.168.50.0/24
```

**5. Save Scan Results**
```bash
sudo nmap -sS -oN scan-results.txt 192.168.50.0/24
```

## Key Concepts

1. **Port Scanning:** Identifying open ports on network devices to understand available services.

2. **TCP SYN Scan:** A scanning technique used by Nmap (`-sS`) to identify open TCP ports by sending SYN packets.

3. **IP Ranges:** A range of IP addresses belonging to a network, such as `192.168.50.0/24`.

4. **Network Reconnaissance:** Gathering information about network devices, services, and potential entry points.

5. **Open Ports:** Network communication endpoints that accept incoming connections from other devices.

6. **Network Security Basics:** Understanding firewalls, securing unused ports, monitoring network traffic, and protecting exposed services.

### Learning Outcomes
- Understand local network scanning.
- Identify active hosts and open ports.
- Recognize services running on network devices.
- Understand potential security risks.


## Interview Questions & Answers

### 1. What is an open port?
An open port is a communication endpoint on a device that accepts incoming network connections. It allows applications and services to communicate over a network.

### 2. How does Nmap perform a TCP SYN scan?
Nmap uses the `-sS` option to send TCP SYN packets to target ports. If a SYN-ACK response is received, the port is considered open. If RST is received, the port is closed.

### 3. What risks are associated with open ports?
Open ports can expose services to attackers. Vulnerable services, weak authentication, and outdated software may lead to unauthorized access, data theft, or system compromise.

### 4. Explain the difference between TCP and UDP scanning.
TCP scanning checks connection-oriented ports using TCP packets. UDP scanning checks connectionless services using UDP packets. UDP scanning can be slower because responses are not always received.

### 5. How can open ports be secured?
- Close unnecessary ports.
- Disable unused services.
- Configure firewalls.
- Keep software updated.
- Use strong authentication.
- Monitor network traffic regularly.

### 6. What is a firewall's role regarding ports?
A firewall monitors and filters network traffic based on security rules. It allows authorized connections and blocks unwanted or suspicious traffic through specific ports.

### 7. What is a port scan and why do attackers perform it?
A port scan is a technique used to identify open ports and services on a target system. Attackers use it to discover potential entry points and vulnerabilities.

### 8. How does Wireshark complement port scanning?
Wireshark captures and analyzes network packets. It helps understand communication between devices, inspect TCP SYN, SYN-ACK, and RST packets, and observe network scanning activity.

---

## Conclusion
This task helped me understand network reconnaissance, open ports, TCP SYN scanning, and basic network security concepts using Nmap and Kali Linux.


**Author:** Md Rizwan

**Internship Task:** Task 1
