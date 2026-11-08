# 🐄 Lumpy Skin Disease Detection with YOLOv11

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/YOLOv11-Object%20Detection-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Roboflow-Dataset-red?style=for-the-badge" />
</p>

<p align="center">
  <b>AI-powered cattle disease detection using YOLOv11 deep learning technology.</b>
</p>

---

## 🌟 Overview

This project uses **YOLOv11n** to detect and localize visible Lumpy Skin Disease (LSD) symptoms in cattle images.

The model identifies suspicious skin nodules using bounding boxes, helping demonstrate how AI can support early livestock disease screening.

## ✨ Key Features

- 🐄 Detects visible Lumpy Skin Disease symptoms.
- 🎯 Localizes skin nodules with bounding boxes.
- 🧠 Uses pretrained YOLOv11 Nano.
- 📦 Downloads an annotated dataset from Roboflow.
- 📊 Evaluates model performance.
- 🖼️ Visualizes detection results.

## 🛠️ Technology Stack

- Python
- YOLOv11n
- Ultralytics
- Roboflow
- OpenCV
- NumPy
- Matplotlib
- Jupyter Notebook

## 📊 Dataset & Model

| Property | Details |
|---|---|
| Model | YOLOv11n |
| Dataset | Lumpy Skin Disease |
| Platform | Roboflow |
| Training Images | 201 |
| Validation Images | 68 |
| Epochs | 50 |
| Image Size | 640 × 640 |
| Batch Size | 8 |
| Device | CPU |

## 🏆 Training Results

| Evaluation Metric | Score |
|---|---:|
| Precision | **96.8%** |
| Recall | **61.5%** |
| mAP@50 | **72.1%** |
| mAP@50-95 | **56.3%** |

## 🚀 Installation & Usage

**1. Clone the repository**

```bash
git clone https://github.com/your-username/lumpy-skin-disease-detection.git
cd lumpy-skin-disease-detection
```

**2. Install dependencies**

```bash
pip install ultralytics roboflow opencv-python matplotlib numpy jupyter
```

**3. Run Jupyter Notebook**

```bash
jupyter notebook
```

Open `Lumpy Skin Disease Prediction.ipynb` and execute the cells in order.

## 📁 Project Structure

```text
Lumpy Skin Disease Prediction/
│
├── Lumpy Skin Disease Prediction.ipynb
├── lumpy-skin-diesease--1/
│   ├── data.yaml
│   ├── train/
│   └── valid/
│
├── runs/
│   └── detect/
│       └── train/
│           └── weights/
│               ├── best.pt
│               └── last.pt
│
└── README.md
```

## ⚠️ Disclaimer

This project is an experimental AI-based detection system. Predictions are not a confirmed veterinary diagnosis. Always consult a qualified veterinarian for disease confirmation and treatment.

## 👨‍💻 Developer

**Zabir Hasan**

🌐 Website: [www.zabirhasan.com](https://www.zabirhasan.com)

---

<p align="center">
  <b>🐄 LumpyGuard AI</b>
  <br/>
  <i>Empowering Livestock Health Through Artificial Intelligence.</i>
  <br/><br/>
  Made with ❤️ using Python & YOLOv11
</p>
