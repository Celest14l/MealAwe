# 🍱 Mealawe AI — Automated Quantity and Quality Verification of Food

Mealawe AI is an AI-powered food inspection system designed for cloud kitchens, restaurant chains, catering services, and industrial food production units. The platform automatically verifies food quantity and quality using Computer Vision and Vision Language Models (VLMs), ensuring compliance with Standard Operating Procedures (SOPs) while reducing manual auditing efforts.

---

## 🚀 Problem Statement

Manual food quality and quantity audits are time-consuming, inconsistent, and difficult to scale across large kitchen operations.

Mealawe AI automates this process by analyzing meal trays in real time and determining whether food portions meet predefined quantity and quality standards.

---

## ✨ Key Features

* Real-time AI-powered food inspection
* Automated quantity verification using fill-ratio analysis
* Food quality assessment using Vision Language Models
* Hybrid AI architecture (YOLO + VLM)
* Two-stage validation pipeline for improved reliability
* Self-correcting feedback loop for instant re-evaluation
* AI-assisted auto-annotation workflow
* API-based deployment architecture
* Pass/Fail verdict generation with detailed feedback

---

## 🏗️ System Architecture

```text
Image Upload (API/UI)
          │
          ▼
   YOLO Segmentation
          │
          ▼
 Mask Extraction & Mapping
          │
          ▼
 Fill Ratio Calculation
          │
          ▼
 Quantity Validation Gate
          │
          ▼
  VLM Quality Assessment
          │
          ▼
  Final JSON Verdict
      Pass / Fail
```

---

## ⚙️ Methodology

### Stage 1: Food Detection & Segmentation

* Meal images are uploaded through an API or web interface.
* YOLOv8/YOLOv26 instance segmentation identifies food items and tray compartments.
* Segmentation masks are extracted for further analysis.

### Stage 2: Quantity Verification

* Fill ratios are calculated for each compartment.
* Measured values are compared against predefined thresholds.
* Quantity compliance is validated automatically.

### Stage 3: Quality Assessment

* Images passing quantity checks are evaluated using Vision Language Models.
* Models assess food appearance, presentation, and quality.
* AI-generated reasoning improves decision reliability.

### Stage 4: Final Decision

The system generates a structured JSON response containing:

* Pass / Fail status
* Quantity validation results
* Quality assessment results
* Actionable feedback

---

## 🧠 AI Pipeline

### Computer Vision

* YOLOv26
* YOLOv8
* OpenCV
* NumPy

### Vision Language Models

* Qwen 2.5
* Qwen 3.5
* Gemini

### Training & Annotation

* PyTorch
* Ultralytics
* Roboflow
* Segment Anything Model (SAM)

---

## 💻 Tech Stack

### Backend

* FastAPI

### Frontend

* Vercel

### AI & Machine Learning

* YOLOv8 / YOLOv26
* Qwen 2.5 / 3.5
* Gemini
* PyTorch

### Image Processing

* OpenCV
* NumPy

### Annotation Tools

* Roboflow
* SAM (Segment Anything Model)

---

## 📈 Project Highlights

* Hybrid architecture combining Computer Vision and Vision Language Models
* Fill ratio-based quantity verification for SOP compliance
* Two-stage validation pipeline (Rule-Based + AI Reasoning)
* Self-correcting feedback mechanism for continuous improvement
* AI-assisted processing of 4000+ annotated images
* Achieves approximately 90% automation of food auditing workflows
* Designed for real-time deployment using API-driven architecture

---

## 🎯 Target Users

* Cloud Kitchens
* Restaurant Chains
* Food Quality Auditors
* Catering Services
* Hostel & Canteen Management
* Food Delivery Platforms
* Industrial Food Production Units

---

## 🔮 Future Scope

* Multi-food cuisine support
* Real-time video stream analysis
* Kitchen dashboard analytics
* Inventory integration
* Automated compliance reporting
* Mobile application deployment

---

## 👥 Team

* Priyanshu Singh
* Ranveer Singh
* Nidhi Pandit
* Pratyush Sinha

### Mentor

Dr. Shrikrishna Kolhar

---

## 📌 Impact

Mealawe AI significantly reduces manual food auditing effort by automating quantity and quality verification, improving operational efficiency, ensuring SOP compliance, and enabling scalable deployment across modern food service operations.
