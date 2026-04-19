🚦 Smart Traffic Control & Surveillance System
📌 Overview

An AI-powered real-time intelligent traffic monitoring system designed for automated traffic management, violation detection, and emergency vehicle prioritization.

The system uses a custom-trained YOLO-based object detection model, OpenCV, and edge computing (Raspberry Pi) to analyze live traffic feeds. It performs vehicle detection, classification, speed estimation, helmet detection, and automatic number plate recognition (ANPR).

All detected events are streamed in real time to a cloud-based backend and visualized through a web dashboard designed for government-level traffic monitoring and enforcement.

🎯 Objectives
Enable real-time intelligent traffic monitoring using computer vision
Detect and classify vehicles (car, bike, bus, truck, etc.)
Identify traffic violations (helmet, overspeeding, red-light violation)
Perform automatic number plate recognition (ANPR)
Prioritize emergency vehicles dynamically
Provide centralized analytics for traffic authorities
⚙️ System Architecture
Edge Layer: Raspberry Pi + Camera modules
AI Layer: YOLO-based object detection + OpenCV processing
Backend Layer: REST APIs + WebSocket streaming
Cloud Layer: Storage + analytics database
Frontend Layer: Real-time dashboard for monitoring and alerts
🧠 Core Features
🚗 Vehicle Intelligence
Real-time detection of vehicles (bike, car, bus, truck)
Vehicle classification using custom-trained YOLO model
🪖 Violation Detection
Helmet detection for riders
Red-light violation detection
Overspeeding estimation
🚨 Emergency Handling
Automatic detection of ambulances and fire brigades
Dynamic green signal prioritization for emergency vehicles
🔢 ANPR System
License plate detection using OCR (EasyOCR / Google Vision API)
Vehicle identity mapping and tracking
📡 Real-Time Data Pipeline
Streaming detection results via WebSockets
REST API-based cloud synchronization
Secure storage of images, logs, and metadata
📊 Analytics Dashboard
Live traffic visualization
Violation logs with evidence images
Vehicle history search (plate-based lookup)
Automated challan generation system
🧠 AI / ML Approach
Object Detection: Custom YOLO model (YOLOv8/YOLOv11-based)
Computer Vision: OpenCV for preprocessing and frame analysis
OCR: EasyOCR + Google Cloud Vision API
Edge Processing: Raspberry Pi inference for low-latency detection
🛠 Tech Stack
🖥 Frontend
React.js
Next.js
Google Maps API
⚙️ Backend
Node.js
Express.js
Socket.IO
REST APIs
🤖 AI / ML
YOLO (custom-trained)
OpenCV
EasyOCR
Google Cloud Vision API
🧩 Hardware
Raspberry Pi
Camera modules
I2C LCD display
☁️ Cloud & DevOps
Google Cloud Platform (GCP)
MongoDB
Docker (optional deployment layer)
OAuth 2.0 authentication
🌍 Applications
Smart city traffic management
Automated traffic violation enforcement
Emergency vehicle prioritization systems
Real-time traffic analytics for government agencies
Urban traffic planning and congestion analysis
⚠️ Challenges Addressed
Low-latency inference on edge devices → optimized YOLO inference
Multi-stream data synchronization → WebSocket + REST hybrid pipeline
High traffic density scenarios → dynamic signal optimization logic
Real-time scalability → cloud + edge hybrid architecture
📁 System Modules
client/ → Frontend dashboard
server/ → Backend APIs + data storage
traffic_signal_simulation/ → traffic logic + simulation engine
lcd/ → Raspberry Pi display module
yolo_detect.py → detection pipeline
custom_yolo11.pt → trained model weights
🚀 Key Highlights (Resume Version)
Built a real-time AI-based traffic surveillance system using YOLO and OpenCV
Implemented vehicle detection, classification, and violation tracking pipeline
Designed edge computing system using Raspberry Pi for low-latency inference
Developed REST + WebSocket-based real-time data streaming architecture
Integrated ANPR system using OCR and Google Vision API
Created government-level analytics dashboard with live traffic visualization
Automated traffic violation detection and challan generation system
📊 Impact
Improves traffic flow efficiency through dynamic signal control
Reduces manual enforcement workload
Enhances emergency vehicle response time
Enables data-driven urban traffic planning