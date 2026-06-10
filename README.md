# Network Scanning and Information Gathering using Nmap

## Objective

The objective of this project was to perform network reconnaissance and information gathering using Nmap. The project demonstrates the process of identifying active hosts, discovering open ports, detecting running services, and performing operating system fingerprinting within a controlled local network environment.

## Tools Used

* Kali Linux 2025.1
* Nmap 7.95

## Methodology

### 1. IP Address Identification

The local IP address of the scanning machine was identified using:

ip addr

### 2. Host Discovery

A ping sweep was performed to identify active hosts on the network.

nmap -sn 192.168.x.x/24

### 3. Service Version Detection

A detailed scan was conducted on the target host.

nmap -sV 192.168.x.xxx

### 4. Operating System Detection

OS fingerprinting was performed using:

sudo nmap -O 192.168.x.xxx

## Findings

### Active Hosts

* 192.168.0.xxx (TP-Link Router)
* 192.168.0.xxx (Windows Host)
* 192.168.0.xxx (Kali Linux Scanner)

### Open Ports and Services

| Port   | State | Service | Version            |
| ------ | ----- | ------- | ------------------ |
| 80/tcp | Open  | HTTP    | Microsoft IIS 10.0 |

### Operating System Detection

Nmap identified the target host as likely running Microsoft Windows 11.

## Conclusion

This project successfully demonstrated network reconnaissance techniques using Nmap. Host discovery, service identification, and operating system detection were performed in a controlled environment. The exercise provided practical experience in information gathering, which is the first stage of a cybersecurity assessment.
