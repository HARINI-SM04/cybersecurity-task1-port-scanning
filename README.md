# cybersecurity-task1-port-scanning
Cyber Security Internship Task 1 - Network Port Scanning using Nmap
# Cyber Security Internship – Task 1

## Scan Your Local Network for Open Ports

### Objective

The objective of this task is to learn how to discover open ports and services running on devices within a local network using Nmap. This helps in understanding network exposure and basic network reconnaissance techniques.

---

## Tools Used

* Nmap
* Command Prompt
* Wireshark (Optional)
* GitHub

---

## Steps Performed

### 1. Installed Nmap

Downloaded and installed Nmap from the official website.

### 2. Identified Local IP Range

Used the following command in Command Prompt:

```bash
ipconfig
```

Identified the local network range as:

```bash
192.168.1.0/24
```

---

### 3. Performed TCP SYN Scan

Executed the following Nmap command:

```bash
nmap -sS 192.168.1.0/24
```

This command performs a TCP SYN scan to identify active hosts and open ports on the local network.

---

### 4. Recorded Open Ports and Services

Observed the scan results and noted the IP addresses, open ports, and associated services.

Example:

| IP Address  | Open Port | Service |
| ----------- | --------- | ------- |
| 192.168.1.1 | 80        | HTTP    |
| 192.168.1.1 | 443       | HTTPS   |

---

### 5. Identified Security Risks

Analyzed potential risks associated with open ports such as:

* Unauthorized access
* Exposure of vulnerable services
* Weak network configurations
* Possibility of brute-force attacks

---

### 6. Saved Scan Results

Saved the scan results using:

```bash
nmap -sS 192.168.1.0/24 -oN scan_results.txt
```

---

## Key Concepts Learned

* Port Scanning
* TCP SYN Scan
* Network Reconnaissance
* Open Ports
* Service Detection
* Basic Network Security

---

## Interview Questions and Answers

### 1. What is an open port?

An open port is a communication endpoint that accepts incoming network connections on a device.

### 2. How does Nmap perform a TCP SYN scan?

Nmap sends SYN packets to target ports and analyzes the responses without completing the full TCP handshake.

### 3. What risks are associated with open ports?

Open ports may expose services that attackers can exploit to gain unauthorized access.

### 4. Difference between TCP and UDP scanning?

TCP scanning checks connection-oriented ports, while UDP scanning checks connectionless ports and is generally slower and less reliable.

### 5. How can open ports be secured?

Unused ports should be closed, firewalls should be configured properly, and secure authentication should be enabled.

### 6. What is the role of a firewall regarding ports?

A firewall monitors and controls incoming and outgoing traffic by allowing or blocking ports.

### 7. What is port scanning?

Port scanning is the process of identifying open ports and services running on a device or network.

### 8. How does Wireshark complement port scanning?

Wireshark captures and analyzes network packets, helping users understand the traffic generated during scans.

---

## Outcome

Successfully learned how to scan a local network for open ports using Nmap and understood the importance of securing exposed network services.
