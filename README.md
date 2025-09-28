# AeroMed SafePass (Demo+) 🚑🚀

**Workspace:** [Rocket.new IDE](https://www.rocket.new/68d2a19fef839b0014a6079f?type=2&f=NLC_REACT#preview)  
**Live Demo:** [AeroMed SafePass Dashboard](https://aeromed-safepass-dashboard-h7rex30.public.builtwithrocket.new)

---

## 📅 Date
23rd September 2025

---

## 🛑 Problem Statement

Every second counts in emergencies, but ambulances face:

* 🚦 Traffic congestion without a guaranteed **green corridor**  
* 🚑 Delays at intersections due to uncoordinated traffic lights  
* 🏥 Hospitals unprepared because they receive patient data **only after arrival**

Traditional systems are **reactive**, costing precious lives.

---

## ✅ Solution — AeroMed SafePass

AeroMed SafePass is a **drone-assisted AI system** that enables:

* **Drone scouting 300–400m ahead** of ambulances to detect congestion and hazards.  
* **AI-driven green corridor automation** at intersections.  
* Real-time **vitals streaming** to hospitals (synthetic for demo).  
* Role-based dashboards for **dispatchers, pilots, hospitals, and analysts**.  
* Advanced **analytics, heatmaps, and reports** for mission insights.  

All data streams, telemetry, and vitals are **synthetic but realistic**, enabling production-like testing.

---

## ✨ Key Features

### Drone Simulation
* 3D **altitude slider**  
* Battery % circular progress  
* Drone route preview on map

### Traffic Light Automation
* Intersection markers with live color  
* **Force Green Corridor** button  
* Configurable cycle time per intersection

### Hospital Dashboard
* Timeline charts for HR, SPO2, BP  
* **Vitals report PDF export**  
* Critical alert banners (HR>150, SPO2<90)

### AI Assistant
* Dummy Q&A: ETA, battery, traffic summary  
* Preseeded responses, ready for integration

### Analytics & Insights
* Missions summary (total, avg response, congestion cleared)  
* Congestion heatmap overlay  
* Chart export (PNG/PDF)

### Logs & Activity
* Colored log levels (INFO / ALERT / EVENT)  
* Filter & CSV export

### Multi-Language Support
* Toggle: English / Tamil / Hindi  
* Seeded translation file for labels

---

## 🧑‍💻 High-Level Tech Stack

### 🖼️ Computer Vision & Perception
* YOLOv8 / YOLOv11 for vehicle/pedestrian detection  
* DeepSORT / ByteTrack for object tracking  
* OpenCV + Mediapipe for preprocessing & annotations  
* PointPillars / PointNet for LiDAR point clouds  
* ONNX + TensorRT for edge deployment

### 🛰️ Drone Autonomy & Simulation
* ArduPilot / PX4 autopilot stack  
* ROS2 for sensor fusion & middleware  
* Gazebo / AirSim for 3D SITL simulation  
* MAVSDK / MAVROS for mission control integration  
* RRT* / D* Lite path planning with obstacle avoidance

### 🧠 AI & ML Frameworks
* PyTorch / TensorFlow for model training  
* Scikit-learn / XGBoost for congestion prediction  
* ST-GCN for spatio-temporal traffic flow forecasting  
* RLlib / Stable-Baselines3 for green corridor optimization  
* Unity Perception & NVIDIA Omniverse for synthetic datasets

### 🏥 Healthcare Integration
* HL7 FHIR API for vitals streaming  
* FHIR Observation + Encounter resources  
* Local FHIR server simulation (FastAPI)

### 📡 Communication & Streaming
* MQTT (Eclipse Mosquitto) for telemetry  
* WebRTC (aiortc / Pion) for live drone video  
* RTSP fallback for synthetic feeds  
* Kafka for event streaming & logs

### 📊 Data & Analytics
* TimescaleDB / InfluxDB for telemetry  
* PostgreSQL / SQLite for mission state  
* ElasticSearch / OpenSearch for log analytics  
* Chart.js / Recharts / Grafana for dashboards & heatmaps  
* Synthetic geospatial congestion heatmaps

### ⚙️ DevOps & MLOps
* Docker + Docker Compose for deployment  
* Kubernetes (K3s / K8s)  
* MLflow / W&B for model tracking  
* DVC for dataset versioning  
* Prometheus + Grafana + Alertmanager for monitoring  
* Sentry for error tracking

### 🔧 Frontend & UI
* React.js / Tailwind CSS / Globules CSS  
* Responsive dashboard with cards, charts, maps, video panels  
* Sticky sidebar, modals, alerts, toast notifications

---

## 🌍 Impact
* 🚑 Faster ambulance arrival → lives saved  
* 🚦 AI green corridor automation reduces human dependency  
* 🏥 Hospitals prepared in advance with live vitals  
* 📊 Valuable insights for smart city mobility planning

---

## 🙏 Credits
* 💡 Idea inspiration: **Vimal**  
* 🤖 Build powered by: **Rocket.new AI Agent**  
* 👩‍💻 Team & community support

---

## 🚀 Future Work
* Real drone integration with live AI perception  
* Full hospital data pipeline (HL7/FHIR)  
* Advanced traffic & urban mobility AI predictions
