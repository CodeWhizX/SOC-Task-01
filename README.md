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

### Key Concepts
- Network Reconnaissance
- Port Scanning
- TCP SYN Scan
- Open Ports
- Service Identification
- Network Security

### Learning Outcomes
- Understand local network scanning.
- Identify active hosts and open ports.
- Recognize services running on network devices.
- Understand potential security risks.

### Conclusion
This practical provided hands-on experience with Nmap and network reconnaissance using Kali Linux.

**Author:** Md Rizwan

**Internship Task:** Task 1
