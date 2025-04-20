# HelixMesh-VPS-Defese
Proof-of-concept code for detecting VPS-hosted nodes via network latency profiling, GeoIP analysis, and challenge-response proof of locality.
# HelixMesh-VPS-Defense

HelixMesh-VPS-Defense is a proof-of-concept implementation designed to detect and flag potentially farmed nodes hosted on VPS infrastructure. This tool mimics real-world defenses used in the HelixMesh DePIN network to ensure only physically distributed, legitimate nodes are rewarded.

---

## Overview

DePIN networks are vulnerable to exploits where users deploy multiple nodes via VPS and automation scripts to unfairly farm rewards. This project implements three basic detection layers:

- **GeoIP-based VPS Detection** using public IP-to-location APIs.
- **Latency Profiling** to differentiate between residential and cloud-hosted nodes.
- **Challenge-Response Clock Drift Tests** to simulate physical hardware verification.

These combined methods improve Sybil resistance and reward fairness in decentralized infrastructure networks.

---

## Features

- GeoIP lookup to determine whether IP belongs to known data centers or hosting providers.
- Simulated latency profiling to detect non-residential or virtual environments.
- Clock drift challenge-response to mimic proof-of-local-presence.
- Simple output log to flag suspicious nodes.
- Fully extensible prototype for future integration with real DePIN validator systems.

---

## Requirements

- Python 3.7+
- Packages:
  - `requests`
  - `geopy`

Install dependencies using:

```bash
pip install -r requirements.txt
