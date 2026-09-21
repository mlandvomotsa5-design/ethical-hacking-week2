# Module 5: Network Scanning with Zenmap

## Overview

This module focuses on active local network scanning, host discovery, and network topology mapping using **Zenmap** (the official graphical user interface for Nmap). The primary objective of this exercise is to identify live assets across a designated IP range, document active hardware MAC addresses, and establish a baseline for internal network auditing.

## Lab Setup & Execution

* **Target Subnet:** `10.0.0.0/24`
* **Scan Profile Used:** `Ping Scan`
* **Tooling:** Zenmap / Nmap

## Host Discovery Summary

A **Ping Scan** was executed across the `10.0.0.0/24` subnet. A total of **4 active hosts** were identified on the local network segment.

### Active Hosts Table

| IP Address | MAC Address | Device / Interface | Status |
| --- | --- | --- | --- |
| `10.0.0.1` | `00:50:56:E3:B3:2C` | Active Host | Up |
| `10.0.0.4` | `00:0C:29:C0:94:8F` | Active Host | Up |
| `10.0.0.19` | `00:50:56:E9:64:82` | Active Host | Up |
| `10.0.0.50` | `00:0C:29:40:C0:93` | Local Workstation | Up |

## Key Takeaways & Security Insights

1. **Asset Discovery & Baseline:** Ping scanning provides a fast and efficient method for security analysts to enumerate live systems on an IP subnet without generating heavy port-scanning noise.
2. **Hardware Auditing:** Capturing hardware MAC addresses along with IP bindings helps trace network interface vendors (e.g., VMware OUI prefixes like `00:50:56` and `00:0C:29`) and detect unauthorized hardware or rogue devices connected to the internal network.
3. **Internal Security Monitoring:** Regular host discovery scans form the foundation for attack surface management, asset inventory tracking, and vulnerability management workflows.
