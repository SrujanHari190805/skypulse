# 🌦️ SkyPulse – Distributed Weather Monitoring Network

> **IEEE EPICS Funded Project | Rs. 7.13 Lakh Grant**

A 16-node distributed atmospheric sensing network deployed across Bengaluru, providing hyperlocal weather intelligence using LoRa mesh communication.

---

## 📌 Problem Statement

Existing weather monitoring infrastructure relies on sparse, centralized stations that fail to capture hyperlocal atmospheric variations across large urban areas. City-scale microclimate differences — critical for agriculture, disaster management, and urban planning — go unmeasured.

---

## 💡 Solution

SkyPulse is a scalable, low-power distributed sensor network of 16 nodes spread across Bengaluru. Each node independently captures atmospheric parameters and relays data via LoRa mesh to a central aggregation server, forming a city-scale hyperlocal weather intelligence platform.

---

## 🏗️ System Architecture

```
[Sensor Node x16]
   ├── Wind Speed Sensor
   ├── Rain Gauge
   ├── UV Index Sensor
   └── Particulate Matter (PM2.5/PM10)
         │
    [LoRa Module]
         │  (Long-range, low-power mesh)
         ▼
[Central Gateway / Aggregation Server]
         │
    [Cloud Dashboard]
         └── Real-time Visualization
         └── Historical Trend Analysis
         └── Alert System
```

---

## ⚙️ Hardware Stack

| Component | Purpose |
|---|---|
| ESP32 | Node microcontroller |
| LoRa SX1276 | Long-range mesh communication |
| Anemometer | Wind speed measurement |
| Tipping Bucket Rain Gauge | Rainfall measurement |
| ML8511 UV Sensor | UV index measurement |
| PMS5003 | PM2.5 / PM10 particulate matter |
| Custom PCB (Altium) | Node integration board |
| Solar Panel + LiPo | Low-power autonomous operation |

---

## 📡 Communication Protocol

- **Technology:** LoRa (Long Range)
- **Topology:** Mesh network
- **Range:** Up to 10 km line-of-sight per node
- **Power:** Ultra-low-power sleep/wake cycles
- **Data Rate:** Optimized for periodic telemetry bursts

---

## 🛠️ PCB Design

- Designed in **Altium Designer**
- Compact form factor for weatherproof enclosure
- Integrated LoRa antenna footprint
- Low-power voltage regulation circuitry
- Certification: Altium Designer Essentials

---

## 📊 Data Pipeline

```
Node Sensors → ESP32 ADC/GPIO → LoRa Transmission
    → Gateway Receiver → MQTT Broker
    → Cloud Storage → Dashboard Visualization
```

---

## 🚧 Current Status

- [x] Project funded (IEEE EPICS Grant – Rs. 7.13 Lakh)
- [x] Hardware prototyping underway
- [x] PCB design completed in Altium
- [x] LoRa communication protocol validated
- [ ] Full 16-node deployment (in progress)
- [ ] City-scale data aggregation dashboard (in progress)

---

## 🏆 Recognition

- **IEEE EPICS Grant** – Rs. 7.13 Lakh for city-scale deployment

---

## 👤 Author

**Sri Srujan Hari T**
B.E – Electronics & Communication Engineering, BMSIT&M
[LinkedIn](https://www.linkedin.com/in/srujan-hari-undefined-1a7364399) | thammineedisrujanhari@gmail.com
