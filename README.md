# HerdGuard

# 🐄 HerdGuard AI

### Smart India Hackathon 2026

**AI/ML-Based Early Warning and Decision-Support System for Subclinical Mastitis**

> **Project Type: Mostly Software**

HerdGuard is a software-focused AI/ML system designed to identify increasing mastitis risk in dairy cattle by analysing longitudinal cow-level data.

The core of HerdGuard is a machine-learning pipeline that transforms sensor and farm data into:

**Individual Baseline → Anomaly Detection → Risk Prediction → Explainable AI → Decision Support**

IoT sensors are proposed as the data-acquisition layer that supplies the software platform with real-world cattle and farm measurements.

---

# 📌 Problem Statement

Mastitis is a major challenge in dairy farming. The subclinical stage can develop before obvious clinical symptoms appear, making early identification difficult.

Traditional observation may detect the problem only after changes in milk quality, production or animal behaviour become noticeable.

HerdGuard proposes a software-driven AI system that continuously analyses cow-level measurements and identifies deviations from an individual animal's normal behaviour.

The goal is to provide an early-warning signal that can support farmers and veterinary personnel in deciding when further inspection or clinical confirmation may be appropriate.

---

# 💡 Proposed Solution

HerdGuard combines longitudinal data processing, anomaly detection, machine learning and explainable AI.

The proposed software workflow is:

```text
Cow / Farm Data
      ↓
Data Ingestion
      ↓
Data Processing
      ↓
Individual Cow Baseline
      ↓
Sensor Deviation Detection
      ↓
Feature Normalization
      ↓
XGBoost Risk Prediction
      ↓
Risk Score
      ↓
Risk Classification
      ↓
SHAP Explanation
      ↓
Farmer / Veterinary Decision Support

## 🛠️ Tech Stack

### 💻 Software & Backend
- **Python** — Core AI/ML and data-processing language
- **FastAPI** — Backend/API layer
- **MQTT over TLS** — Secure IoT data communication
- **PostgreSQL** — Primary database
- **TimescaleDB** — Time-series sensor data storage
- **PostGIS** — Geospatial data and herd hotspot mapping

### 🤖 AI / Machine Learning
- **XGBoost** — Primary risk prediction model
- **LightGBM** — Alternative gradient-boosting model
- **Scikit-learn** — Data preprocessing and model evaluation
- **SHAP** — Explainable AI and feature contribution analysis
- **LSTM / GRU** — Planned Phase-2 sequence modelling
- **MLflow** — Model tracking and experiment management

### 📊 Data & Analytics
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computation
- **Matplotlib** — Data visualization
- **Longitudinal time-series analysis** — Individual cow behaviour and anomaly detection

### 🌐 Frontend & Applications
- **React** — Web dashboard
- **GIS Mapping** — Herd-level risk and hotspot visualization
- **Flutter** — Farmer, veterinarian and field-worker mobile application
- **Bhashini API** — Multilingual text and voice support
- **SMS Alerts** — Farmer and veterinary notifications

### 📡 IoT & Hardware Integration
- **ESP32** — Cow tag and farm gateway
- **DS18B20** — Temperature sensing
- **MPU-6050** — Motion/activity sensing
- **LoRa** — Long-range sensor communication
- **DHT22** — Environmental temperature and humidity
- **Milk Conductivity Probe** — Milk conductivity measurement
- **Load Cell** — Milk-yield / weight measurement
- **RFID / Barcode** — Cow identification
- **GPS** — Location tracking
- **SD Card + GSM** — Offline storage and communication backup

### 🔄 HerdGuard Pipeline

**Sense → Send → Store → Predict → Explain → Act**

IoT sensors collect cow and farm data → secure communication transmits the data → time-series storage maintains longitudinal records → AI/ML predicts risk → SHAP explains the prediction → dashboard, mobile app and SMS deliver decision-support alerts.
