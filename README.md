# HelixMesh-VPS-Defense

HelixMesh-VPS-Defense is a proof-of-concept tool to detect and flag potentially farmed nodes running on cloud/VPS infrastructure. It's designed to help DePIN networks improve Sybil resistance by identifying setups that may be automated or non-residential.

---

## 🧠 Overview

In decentralized physical infrastructure networks (DePIN), users may deploy multiple virtual nodes on VPS or data centers to farm rewards unfairly. This tool simulates real-world defense strategies like:

- 🌐 GeoIP-based hosting provider detection
- 🛰️ Latency profiling
- ⏱️ Clock drift tests (challenge-response)

These mechanisms help networks identify suspicious behavior and promote fair, distributed node participation.

---

## ⚙️ Configuration

You can configure the tool by editing the list of IPs you want to test:

```python
nodes = [
    my_ip,             # Automatically fetches your public IP
    "45.13.12.3",      # Example VPS IP
    "192.168.1.20",    # Example local IP
    "23.94.107.1"      # Another VPS example
]
