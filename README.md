# nmap-local-discovery
To discover open TCP ports on a device in your local network, understand which services are running, identify potential security risks, and optionally capture packets to analyze the network traffic during the scan.

# Nmap Subnet Scanning Project

## Overview
This project involves scanning a local subnet (`192.168.--.0/24`) using `nmap` to identify live hosts and open ports. The scans were conducted on Kali Linux.

## Tools Used
- OS: Kali Linux
- Tool: Nmap v7.98SVN
- Network Interface: eth0 (IP: 192.168.------)


## Steps Performed

### 1. Setup Scan Directory
```bash
mkdir -p ~/scans
cd ~/scans



Identify IP Address

=>ifconfig

Subnet Scan
=>sudo nmap -sS 192.168.------/24 -oA ~/scans/scan_subnet

. Targeted Full Scan on Host (192.168.----)
=>sudo nmap -sS -sV -p- -T4 192.168.---- -oA ~/scans/192.168.------_full

then use wireshark to analyze 


