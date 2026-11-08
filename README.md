# 🐄 Lumpy Skin Disease Detection with YOLOv11

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/YOLOv11-Object%20Detection-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Ultralytics-Framework-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Roboflow-Dataset-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" />
</p>

<p align="center">
  An AI-powered cattle health monitoring system that detects Lumpy Skin Disease (LSD) using YOLOv11 deep learning technology.
</p>

---

## 🌟 Overview

**Lumpy Skin Disease Detection** is a deep learning-based object detection project designed to identify visible signs of **Lumpy Skin Disease (LSD)** in cattle through image analysis.

Powered by **YOLOv11n (You Only Look Once)**, the system detects and localizes suspicious skin nodules on cattle images using bounding boxes.

Lumpy Skin Disease is a serious viral infection that affects cattle health, milk production, and livestock productivity. Early identification of visible symptoms can help farmers and livestock professionals take timely action.

This project demonstrates an end-to-end AI workflow, from dataset preparation and model training to evaluation and image-based inference.

### 🎯 Key Objectives

- 🐄 Detect visible Lumpy Skin Disease symptoms in cattle.
- 🎯 Localize suspicious skin nodules using bounding boxes.
- ⚡ Build a lightweight and efficient object detection model.
- 🧠 Apply YOLOv11 deep learning for automated image analysis.
- 📊 Evaluate model performance using standard detection metrics.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 🧠 YOLOv11 Detection | Uses YOLOv11 Nano for object detection. |
| 🐄 Skin Nodule Detection | Identifies visible suspicious skin nodules. |
| 🎯 Bounding Box Localization | Highlights detected regions in images. |
| 📦 Roboflow Dataset | Uses an annotated cattle disease dataset. |
| 🔥 Model Training | Fine-tunes a pretrained YOLOv11 model. |
| 📊 Performance Evaluation | Measures Precision, Recall, and mAP. |
| 🖼️ Prediction Visualization | Displays detection results on images. |
| ⚡ Lightweight Architecture | Nano model suitable for resource-constrained environments. |

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| YOLOv11n | Object detection model |
| Ultralytics | Model training and inference |
| Roboflow | Dataset management and downloading |
| OpenCV | Image processing |
| Matplotlib | Training visualization |
| NumPy | Numerical operations |
| Jupyter Notebook | Development environment |

---

## 🧠 Model & Dataset

### Model Architecture

**YOLOv11n (Nano)**

YOLOv11n is a lightweight object detection architecture designed for fast inference and relatively low computational requirements.

It was selected because it offers a practical balance between detection performance, speed, and model size.

### Dataset Information

The project uses a labeled cattle skin disease dataset obtained from Roboflow.

**Dataset Details:**

| Property | Information |
|---|---|
| Dataset Name | Lumpy Skin Disease |
| Workspace | end-game |
| Platform | Roboflow |
| Annotation Format | YOLOv11 |
| Training Images | 201 |
| Validation Images | 68 |
| Total Images | 269 |

The dataset contains cattle skin images annotated with bounding boxes around visible skin nodules.

---

## 📊 Training Results

The YOLOv11n model was trained for **50 epochs** using CPU processing.

### Model Performance

| Evaluation Metric | Score |
|---|---:|
| 🎯 Precision | **96.8%** |
| 🔍 Recall | **61.5%** |
| 📈 mAP@50 | **72.1%** |
| 🏆 mAP@50-95 | **56.3%** |

### Performance Visualization

<details>
<summary><b>📈 Understanding the Evaluation Metrics</b></summary>

- **Precision (96.8%)** — Of the model's positive detections, approximately 96.8% were correct according to the evaluation criteria.
- **Recall (61.5%)** — The model detected approximately 61.5% of the ground-truth objects.
- **mAP@50 (72.1%)** — Measures average precision at an IoU threshold of 0.50.
- **mAP@50-95 (56.3%)** — Measures average precision across IoU thresholds from 0.50 to 0.95.

</details>

> 💡 **Note:** These are the reported validation results from this training run. Performance may vary on new cattle images, different lighting conditions, and unseen environments.

### 📸 Training & Validation Samples

The notebook includes visualizations of training and validation batches, allowing you to inspect the annotated images and bounding boxes used during model development.

---

## 📁 Project Structure

```text
Lumpy Skin Disease Prediction/
│
├── 📓 Lumpy Skin Disease Prediction.ipynb
│
├── 📂 lumpy-skin-diesease--1/
│   │
│   ├── 📄 data.yaml
│   │
│   ├── 📂 train/
│   │   ├── images/
│   │   └── labels/
│   │
│   └── 📂 valid/
│       ├── images/
│       └── labels/
│
├── 📂 runs/
│   └── 📂 detect/
│       └── 📂 train/
│           │
│           ├── 📂 weights/
│           │   ├── best.pt
│           │   └── last.pt
│           │
│           ├── results.png
│           ├── confusion_matrix.png
│           ├── train_batch0.jpg
│           └── val_batch0_pred.jpg
│
└── 📄 README.md
```

*Note: The actual generated files and folder names may vary depending on your training environment.*

---

## 🐄 About Lumpy Skin Disease

**Lumpy Skin Disease (LSD)** is an infectious viral disease of cattle caused by the Lumpy Skin Disease Virus, which belongs to the *Capripoxvirus* genus.

### Common Symptoms

- 🌡️ Fever
- 🔴 Firm skin nodules
- 🐄 Swelling of superficial lymph nodes
- 🥛 Reduced milk production
- 🍽️ Loss of appetite
- 💧 Skin lesions and associated discomfort

### Transmission

The disease is primarily transmitted through blood-feeding insects, including mosquitoes and biting flies.

### Why Early Detection Matters

Early recognition of suspicious symptoms can help livestock owners seek veterinary assistance, reduce potential disease spread, and protect cattle health.

> ⚠️ **Medical Disclaimer:** This project is an experimental AI-based visual detection system. Its predictions are not a confirmed veterinary diagnosis. A qualified veterinarian should examine suspected cases and determine appropriate treatment and control measures.

---

## 🔮 Future Improvements

Potential improvements for future versions include:

- 📷 Real-time cattle disease detection using a camera.
- 📱 Mobile application for farmers.
- 🌐 Web-based disease detection dashboard.
- 📊 Detection history and report generation.
- 🔔 Alerts for suspected infected cattle.
- 🧠 Improved model training with a larger and more diverse dataset.
- 🐄 Multi-disease detection for different cattle diseases.
- 🌦️ Robust detection under different lighting and environmental conditions.

---

## 👨‍💻 Developer

**Developed as an AI and Machine Learning project focused on intelligent livestock health monitoring.**

🌐 Website: [www.zabirhasan.com](https://www.zabirhasan.com)

---


<p align="center">
  **🐄 LumpyGuard AI**
  <br/>
  *Empowering Livestock Health Through Artificial Intelligence.*
  <br/><br/>
  Made with ❤️ using Python, Deep Learning & YOLOv11
</p>
