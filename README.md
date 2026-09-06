# 🛡️ HostelGuard AI

## AI-Powered Smart Hostel Security and Surveillance System

HostelGuard AI is an AI-powered hostel security and surveillance system designed to monitor CCTV camera feeds in real time and detect potentially suspicious or unsafe activities.

The system uses computer vision and deep learning to detect people, monitor occupancy, identify restricted-area entry, detect intruders and loitering, and generate security alerts automatically.

---

## 🚀 Key Features

- 👤 Real-time person detection
- 👥 People counting
- 🚨 Intruder detection
- ⛔ Restricted-area monitoring
- 🕒 Loitering detection
- 👥 Overcrowding detection
- 🔔 Automated security alerts
- 📊 Real-time CCTV monitoring
- 📝 Alert logging in JSON format
- 🌐 Backend integration using Flask

---

## 🧠 AI & Computer Vision

The system uses **YOLOv8** for real-time object detection.

### Detection Pipeline

CCTV Camera Feed  
↓  
Video Frame Processing  
↓  
YOLOv8 Person Detection  
↓  
People Tracking & Analysis  
↓  
Security Rule Evaluation  
↓  
Alert Generation  
↓  
Alert Logging / Backend

---

## 🛠️ Technology Stack

### AI & Computer Vision
- Python
- OpenCV
- YOLOv8
- Ultralytics

### Backend
- Flask

### Database
- MongoDB / Firebase

### Data & Alerts
- JSON-based alert logging

---

## 🔍 Security Detection Modules

### 1. Person Detection
Detects people present in the CCTV camera feed using YOLOv8.

### 2. People Counting
Counts the number of people present in a monitored area.

### 3. Intruder Detection
Identifies unauthorized persons entering monitored areas.

### 4. Restricted Area Detection
Monitors predefined restricted zones and generates an alert when a person enters the area.

### 5. Loitering Detection
Detects when a person remains within a monitored area for longer than the defined threshold.

### 6. Overcrowding Detection
Monitors the number of people in an area and generates an alert when the configured occupancy limit is exceeded.

---

## 🚨 Alert System

When a security condition is detected, HostelGuard AI generates an alert containing relevant event information.

Alerts are stored in:

```text
alerts.json


HostelGuard-AI/
│
├── backend/
│   └── app.py
│
├── detection/
│   ├── person_detection.py
│   ├── intruder_detection.py
│   ├── restricted_area.py
│   ├── loitering_detection.py
│   └── overcrowding_detection.py
│
├── models/
│   └── yolov8n.pt
│
├── alerts/
│   └── alerts.json
│
├── frontend/
│
├── requirements.txt
├── README.md
└── .gitignore



📌 Project Vision
HostelGuard AI aims to transform conventional CCTV surveillance into an intelligent security system by combining real-time computer vision with automated event detection and alert generation.
Instead of relying entirely on manual CCTV monitoring, the system continuously analyzes camera feeds and helps security personnel identify important events more efficiently.
