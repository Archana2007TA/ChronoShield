# 🌍 ChronoShield
### High-Rigor Urban Climate Intelligence & Microclimate Prediction Platform

---

## 🚀 Overview
**ChronoShield** is an advanced spatial-temporal urban climate intelligence system designed to model, simulate, and predict hyper-local microclimate anomalies (such as street-level heatwaves and toxic PM2.5 air pockets) **2 to 4 hours before they peak**. 

Standard macro-level weather stations fail to capture street-level thermal variations caused by traffic congestion, concrete heat retention, and urban density. ChronoShield bridges this knowledge gap by fusing moving mobile telemetry with static urban morphology on a directed spatial road graph.

---

## 🏗️ System Architecture & Decoupled Layers

1. **Layer 1: Edge & Telemetry Ingestion:** Uses `OSMnx` to build a directed road network graph, binding static morphology attributes (Tree Canopy Density Index, Surface Albedo/Heat Retention) and simulating opportunistic mobile sensor streams.
2. **Layer 2: Spatial-Temporal ML Engine:** Implements map-matching, non-linear physical interaction feature engineering (`SpikePotential`), and predictive forecasting (`LightGBM` + `Isolation Forest` + `ST-GNN`).
3. **Layer 3: Backend API & Streaming Pipeline:** Built with `FastAPI` and backed by `PostgreSQL` + `PostGIS` to serve high-performance GeoJSON spatial predictions and telemetry analytics.
4. **Layer 4: Geospatial Validation Dashboard:** An interactive command-center web interface featuring a multi-horizon predictive time-slider, vulnerable corridor alerts, and macro-vs-micro model explainability charts.

---

## 🛠️ Technology Stack

* **Core Intelligence & Backend:** Python 3, FastAPI, GeoPandas, Shapely, OSMnx, NetworkX, LightGBM, Scikit-learn, PyTorch.
* **Spatial Storage & Database:** PostgreSQL, PostGIS (spatial indexing & geometric queries).
* **Frontend Visualization:** HTML5, CSS3, Modern JavaScript (ES6+), Leaflet.js, Chart.js.
* **Edge Hardware (Optional):** C / C++ (ESP32 microcontrollers for physical sensor node prototyping).

---

## 📂 Repository Structure

```text
ChronoShield/
├── PRD.md                 # Official Product Requirements Document
├── README.md              # Project documentation & overview
├── index.html             # Interactive Geospatial Intelligence Dashboard (MVP)
