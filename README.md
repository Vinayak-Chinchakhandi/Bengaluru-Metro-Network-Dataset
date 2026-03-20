# 🚇 Bengaluru Metro Network & Stations Dataset

A structured and graph-ready dataset representing the **Bengaluru (Bangalore) Namma Metro network**, including station metadata, geospatial coordinates, and network connectivity.

This dataset is designed to support developers, researchers, and students working on **transportation systems, smart city solutions, and data-driven metro applications**.

---

## 📂 Dataset Contents

### 1. bengaluru_metro_stations.csv

Contains metadata for all metro stations.

**Columns:**

- `station_name` — Name of the metro station  
- `station_code` — Unique short code for each station  
- `line` — Metro line (Purple Line, Green Line, Yellow Line)

---

### 2. bengaluru_metro_network.csv

Represents the metro system as a **graph structure** with connectivity and geospatial data.

**Columns:**

- `station_code` — Unique station identifier  
- `station_name` — Name of the station  
- `line` — Metro line  
- `sequence` — Order of station within the line  
- `is_interchange` — Interchange flag (1 = Yes, 0 = No)  
- `next_station_code` — Next station in route (`NULL` for terminal stations)  
- `latitude` — Geographic latitude  
- `longitude` — Geographic longitude  
- `distance_to_next_km` — Distance to next station (in km)  
- `line_color` — Hex color representing metro line  

---

## 🌐 Key Features

- Complete **graph-based metro network structure**
- Accurate **geospatial coordinates** for mapping
- Distance between stations using **Haversine formula**
- Interchange station modeling
- Multi-line coverage (Purple, Green, Yellow)
- Ready for **graph algorithms and routing systems**

---

## 💡 Use Cases

This dataset can be used for:

- 🚇 Route optimization (Dijkstra / shortest path)
- 🗺 Metro network visualization (Leaflet, Mapbox, GIS)
- 📊 Transportation analytics & simulations
- 🧠 Smart city and urban mobility research
- 📈 Demand prediction (with external ridership data)
- 🎫 Building metro ticketing or navigation systems

---

## 🔗 Integration

This dataset can be combined with metro ridership datasets (available on Kaggle) for:

- Passenger demand prediction  
- Peak hour analysis  
- Congestion modeling  

👉 Kaggle Dataset: [View on Kaggle](https://www.kaggle.com/datasets/vinayakchinchakhandi/bengaluru-metro-network-dataset)
---

## ⚠️ Notes

- Terminal stations have `next_station_code = NULL`
- Distances are calculated between consecutive stations
- Coordinates are manually curated and verified for accuracy
- Dataset will be updated as new metro lines/stations are added

---

## 📜 License

This dataset is released under **CC0 (Public Domain)**.  
You are free to use, modify, and distribute it without restrictions.

---

## 🙌 Contribution

This dataset was created to address the lack of structured metro datasets publicly available and to help developers and researchers build **real-world transportation solutions**.

If you use this dataset, consider giving credit or sharing your work 🙌