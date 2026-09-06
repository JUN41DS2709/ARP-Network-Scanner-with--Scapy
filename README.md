# ARP Network Scanner
A simple Python-based network scanner that uses **ARP requests** and **Scapy** to discover active devices on a local network. It displays their IP address, MAC address, and MAC vendor.

## Features

* Discover active hosts on a local network
* Uses ARP requests with Scapy
* Displays IP and MAC addresses
* Identifies MAC address vendors
* Clean table-based output

## Requirements

```bash
pip install scapy prettytable mac-vendor-lookup
```

## Usage

```bash
python scanner.py --h 192.168.1.0/24
```

Multiple targets can also be provided:

```bash
python scanner.py --h 192.168.1.1 192.168.1.10
```

> Run with appropriate administrator/root privileges when required.

## How It Works

The scanner sends ARP broadcast requests, collects responses from active devices, extracts their IP and MAC addresses, and performs a MAC vendor lookup.

**Use this tool only on networks you own or have permission to scan.**
**Thanks and all credits to @hellsender01 for teaching me this code** 
