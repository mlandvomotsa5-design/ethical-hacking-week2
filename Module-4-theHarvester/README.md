# Module 4: Footprinting & Reconnaissance with theHarvester

## Overview
This module utilizes `theHarvester`, a Python-based OSINT tool, to gather emails, subdomains, hostnames, and open ports across multiple public search engines and database APIs.

---

## Tasks & Executed Commands

### Task 1: Search via Baidu Source
Querying target domain `microsoft.com` using the Baidu engine with a result limit of 1000.
```bash
theHarvester -d microsoft.com -l 1000 -b baidu
