# Comparing Congestion Control Schemes in Datacenter Networks

## Project Overview

A network simulation and performance analysis project comparing NDP and SMaRTT congestion control schemes in high-speed datacenter networks.

The project investigates congestion management, network latency, queue occupancy, load balancing, and transport protocol performance under different traffic patterns and network conditions.

This project was developed for ECE-GY 6383 at NYU Tandon School of Engineering.

## Research Objectives

- Compare NDP and SMaRTT congestion control mechanisms.
- Investigate congestion caused by many-to-one incast traffic.
- Evaluate flow completion time and network latency.
- Analyze switch queue occupancy and congestion behavior.
- Investigate load balancing and network link failures.
- Evaluate transport protocols for high-speed AI datacenter networks.

## Technologies and Tools

| Technology | Purpose |
|---|---|
| htsim | Datacenter network simulation |
| NDP | Receiver-driven datacenter transport |
| SMaRTT | RTT-based congestion control |
| UEC | High-performance Ethernet transport research |
| ECN | Explicit Congestion Notification |
| Python | Performance data analysis |
| Linux | Simulation environment |
| Fat-Tree | Datacenter network topology |

## Network Architecture

The experimental environment uses a three-tier fat-tree topology to model a high-speed datacenter network.

| Parameter | Configuration |
|---|---|
| Network Topology | Three-tier Fat-Tree |
| Number of Servers | 128 |
| Number of Pods | 8 |
| Core Switches | 16 |
| Link Speed | 400 Gbps experimental configuration |
| Packet Size | 2048 bytes |
| Traffic Patterns | Incast and Many-to-Many |

## Congestion Control Schemes

### NDP

NDP is a receiver-driven datacenter transport protocol designed to reduce congestion and provide low-latency communication through packet trimming, receiver feedback, and multipath forwarding.

### SMaRTT

SMaRTT uses round-trip time measurements and congestion feedback to dynamically adjust transmission behavior and manage congestion in high-speed datacenter networks.

## Experimental Scenarios

### Incast Traffic

Multiple servers simultaneously transmit data to a single destination, creating congestion at the receiving side.

Evaluated flow sizes include:

- 2 MB
- 10 MB
- 50 MB
- 100 MB

### Many-to-Many Traffic

Multiple source and destination servers communicate concurrently to evaluate congestion behavior under distributed workloads.

### Hotspot Traffic

Traffic is concentrated on selected destination servers to investigate localized network congestion.

### Link Failure Analysis

Network link failures are introduced to investigate transport performance and congestion behavior under degraded network conditions.

### Load Balancing

Different traffic distribution strategies are investigated to evaluate their effects on network utilization and switch queue occupancy.

## Performance Metrics

| Metric | Description |
|---|---|
| Flow Completion Time | Time required to complete a network flow |
| Average FCT | Mean flow completion time |
| Tail Latency | High-percentile flow completion latency |
| Queue Occupancy | Amount of buffered traffic at network switches |
| Queue Variance | Variation in switch queue utilization |
| Throughput | Data transmission rate |
| ECN | Explicit congestion feedback |
| Fairness | Distribution of network resources among flows |

## Performance Analysis

The experiments investigate how congestion control mechanisms respond to bursty traffic, competing flows, queue buildup, load balancing, and network failures.

The comparison highlights the importance of transport protocol design, congestion feedback, and traffic distribution in high-speed datacenter networks.

Detailed experimental results, performance graphs, and discussion are provided in the final technical report and presentation.

## Technical Skills Demonstrated

- High-Speed Datacenter Networking
- Network Architecture and Fat-Tree Topology
- Congestion Control
- Network Transport Protocols
- NDP and SMaRTT
- Explicit Congestion Notification (ECN)
- Network Load Balancing
- Network Performance Benchmarking
- Flow Completion Time Analysis
- Queue Occupancy Analysis
- Network Failure Analysis
- Python Data Analysis
- Linux Network Simulation
- AI Datacenter Networking

## Academic Project

- Institution: NYU Tandon School of Engineering
- Course: ECE-GY 6383
- Semester: Fall 2025
- Program: M.S. Computer Engineering

## Project Report and Presentation

- [Final Technical Report](./ECE6383_FinalProject%20%20%287%29.pdf)
- [Project Presentation Slides](./final_hSpeed_d.pptx)

## Final Video Presentation

[Watch the Final Project Presentation on Google Drive](https://drive.google.com/file/d/18OQ4Y0zCCY_MW-ESFtU0nY1BNnsWx2OF/view?usp=sharing)
