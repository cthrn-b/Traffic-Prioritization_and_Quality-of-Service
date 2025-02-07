# Traffic Prioritization and Quality of Service (QoS)

## Overview
This introduces the concepts of traffic prioritization using Quality of Service (QoS). It guides through configuring QoS policies to optimize network performance for different types of traffic and analyzing the results.

## Objectives
- Understand the importance of QoS in network performance.
- Configure QoS policies to prioritize different types of network traffic.
- Measure network performance before and after applying QoS.
- Analyze network traffic using tools like Wireshark.

## Requirements
### Software & Tools
- Network simulator (e.g., Cisco Packet Tracer, GNS3) or actual hardware with QoS capabilities.
- Wireshark for traffic analysis.
- iPerf for traffic generation and measurement.

### Devices
- Two routers
- Two switches
- At least four computers or virtual machines

## Network Topology
- Two routers connected via a WAN link.
- Switches connected to each router.
- Two computers per switch:
  - One generating high-priority traffic (e.g., VoIP, video streaming).
  - One generating low-priority traffic (e.g., file downloads, web browsing).

## Tasks
### Task 1: Baseline Performance Measurement
1. Use iPerf to generate network traffic without QoS policies.
2. Measure latency, bandwidth, and jitter for different types of traffic.
3. Capture network traffic using Wireshark to analyze packet flow.

### Task 2: Configure QoS Policies
1. Classify traffic:
   - Define traffic classes (e.g., real-time vs. background traffic).
   - Use ACLs or classifiers to identify different types of traffic.
2. Apply QoS techniques:
   - **Priority Queuing (PQ):** Prioritize real-time traffic.
   - **Weighted Fair Queuing (WFQ):** Ensure fair bandwidth allocation.
   - **Traffic Shaping:** Limit bandwidth for certain traffic types to prevent congestion.

### Task 3: Re-Test Network Performance with QoS
1. Repeat Task 1 tests after applying QoS policies.
2. Measure the impact of QoS on latency, bandwidth, and jitter.
3. Capture and analyze network traffic using Wireshark to verify prioritization.

---

## Author
This project was created by the repository owner.
