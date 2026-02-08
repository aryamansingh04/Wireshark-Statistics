# Wireshark Statistics and Graph Analysis

A **Python-based network traffic analysis project** that processes Wireshark packet capture files and exported statistics to generate **network insights, performance metrics, and visualizations**.

---

# Overview

This project analyzes network traffic captured in **Wireshark (.pcapng)** format and processes exported **protocol and conversation statistics** to provide:

* Traffic pattern visualization over time
* Protocol hierarchy distribution analysis
* Network conversation statistics
* Communication performance metrics

The implementation is designed for **academic network analysis experiments** using **Python, Scapy, and data visualization libraries**.

---

# Files Description

* **exp7.pcapng** → Raw Wireshark packet capture containing network traffic
* **Stasitics.ipynb** → Jupyter Notebook with complete traffic analysis code
* **protocol.csv** → Protocol hierarchy statistics exported from Wireshark
* **conversation.csv** → Network conversation statistics exported from Wireshark
* **Staistics and Graphs.pdf** → Final documentation/report of the experiment

---

# Features

## 1. Traffic Visualization

The project generates **time-based traffic graphs** for:

* **Total Traffic (Frames)** → Overall packet count per second
* **TCP Traffic** → Transmission Control Protocol activity
* **UDP Traffic** → User Datagram Protocol communication
* **HTTP/HTTPS Traffic** → Web traffic on ports **80** and **443**
* **DNS Traffic** → Domain Name System queries and responses

These graphs help identify **traffic spikes, browsing behavior, and protocol usage trends**.

---

## 2. Protocol Analysis

From the exported **protocol hierarchy statistics**, the project computes:

* **Total packet count**
* **Data size vs header size estimation**
* **Protocol distribution within captured traffic**
* **Bits-per-second throughput metrics**

This provides insight into **how different protocols contribute to network load**.

---

## 3. Conversation Analysis

Using **Wireshark conversation statistics**, the project determines:

* **Address pairs with maximum data transfer**
* **Average inter-packet time between communicating hosts**
* **Packet counts exchanged between address pairs**
* **Bidirectional traffic behavior**

This reveals **communication intensity, active hosts, and session characteristics**.

---

# Requirements

Install the required Python libraries:

```bash
pip install scapy matplotlib numpy pandas
```

---


## 4. Run the Notebook Cells

Execute all cells sequentially to:

* Generate **traffic graphs**
* Compute **protocol statistics**
* Analyze **network conversations**
* Display **processed data tables**

---

# Key Metrics Calculated

* **Total Packets** → Number of captured packets
* **Data Size** → Payload data across application protocols
* **Header Size** → Difference between total bytes and payload size
* **Maximum Bytes Transferred** → Largest communication between two addresses
* **Average Inter-Packet Time** → Delay between consecutive packets in a conversation

---

# Output

The notebook produces:

* **Line graphs** showing packets-per-second for multiple protocols
* **Console summaries** of computed statistics
* **Cleaned Pandas DataFrames** for structured network data analysis

---

# Notes

* Supports both **IPv4 and IPv6** traffic
* Automatically cleans **CSV formatting issues** (quotes, whitespace, encoding)
* Uses **1-second time intervals** for graph generation
* Developed in **Google Colab**, compatible with any **Jupyter environment**

---

# Technologies Used

* **Scapy** → Packet parsing and manipulation
* **Matplotlib** → Graph plotting and visualization
* **NumPy** → Numerical computation
* **Pandas** → Data cleaning and statistical analysis

---

# License

This project is created for **educational and network analysis purposes only**.

---
