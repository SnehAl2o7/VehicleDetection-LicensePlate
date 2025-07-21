# 🚘 Vehicle & Number Plate Detection System 🔍

![Build](https://img.shields.io/badge/Build-Passing-brightgreen)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-purple)
![OCR](https://img.shields.io/badge/OCR-EasyOCR-red)
![License](https://img.shields.io/badge/License-MIT-blue)
![Python](https://img.shields.io/badge/Python-3.8+-blue)

> 🎯 A real-time AI-powered system that detects vehicles and extracts number plates from images or video feeds. Ideal for smart surveillance, toll booths, and law enforcement use cases.

---

## ✨ Key Features

| 🚀 Feature                  | 💡 Description |
|----------------------------|----------------|
| 🚘 **Vehicle Detection**   | Detects cars, trucks, bikes using **YOLOv8** |
| 🔠 **Number Plate OCR**    | Extracts plate numbers using **EasyOCR** or **PaddleOCR** |
| 🖼 **Image/Video Input**    | Works with both static images and live video |
| 📍 **Bounding Boxes**       | Annotates frames with detected vehicles and plate text |
| 💾 **Log Exporting**        | Saves extracted info with timestamps to JSON/CSV |
| 🌐 **Optional Web App**     | View detections in-browser with **Flask** backend |

---

## 🧠 Tech Stack

| Category            | Technologies |
|---------------------|--------------|
| 🔍 Object Detection  | [YOLOv8](https://github.com/ultralytics/ultralytics) |
| 🔤 OCR Engine        | [EasyOCR](https://github.com/JaidedAI/EasyOCR), PaddleOCR |
| 📦 Libraries         | OpenCV, NumPy, Pillow, Flask, Ultralytics |
| 🗄️ Data Logging       | Pandas, CSV, JSON |
| 🌐 Web Framework     | Flask (optional dashboard) |

---

## 📊 Workflow Diagram

```mermaid
graph LR
    A[Input Image or Video Frame] --> B[YOLOv8: Detect Vehicles]
    B --> C[Crop Vehicle Regions]
    C --> D[Detect Number Plate Region]
    D --> E[Apply OCR on Plate]
    E --> F[Extracted Plate Number]
    F --> G[Save to Log File]
    G --> H[Display/Return Annotated Image]
