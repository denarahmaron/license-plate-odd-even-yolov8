# 🚗 YOLOv8 Odd-Even License Plate Detection

## 📌 Overview

This project focuses on **optimization of a prediction model for detecting odd-even vehicle license plates** using the YOLOv8 algorithm.

The system is designed to support **traffic management policies**, especially the implementation of **odd-even vehicle restrictions**, by automatically detecting and classifying license plates in real-time.

---

## 🎯 Objectives

* Develop a **YOLOv8-based model** for license plate detection
* Classify license plates into:

  * 🔵 Odd
  * 🔴 Even
* Evaluate model performance using:

  * Precision
  * Recall
  * F1-Score
  * mAP (mean Average Precision)
* Compare detection performance between:

  * Static images
  * Video input

---

## 🧠 Methodology

### 1. Data Collection

* Dataset consists of vehicle license plate images
* Various conditions:

  * Lighting variations
  * Different angles
  * Multiple vehicle types

---

### 2. Preprocessing

* Cropping license plate region
* Resizing to **640x640 pixels**
* Data labeling:

  * `0` → Odd
  * `1` → Even

---

### 3. Data Split

* Train
* Validation
* Test

---

### 4. Model Training

* Algorithm: **YOLOv8**
* Training environment: Google Colab
* Epoch: 100

---

### 5. Evaluation Metrics

* Precision
* Recall
* F1-Score
* mAP50
* mAP50-95

---

## 📊 Results

| Metric    | Value |
| --------- | ----- |
| Precision | 0.93  |
| Recall    | 0.919 |
| mAP50     | 0.975 |
| mAP50-95  | 0.748 |

✅ The model shows **high accuracy and reliability** for real-time detection.

---

## 🚀 Features

* Real-time license plate detection
* Odd-even classification
* Works on both **images and video**
* Optimized for performance vs accuracy

---

## 🖥️ Tech Stack

* Python
* YOLOv8 (Ultralytics)
* OpenCV
* Google Colab

---

## 📂 Project Structure

```
.
├── notebooks/          # Jupyter notebooks
├── datasets/           # Dataset (excluded in repo)
├── runs/               # Training results (excluded)
├── models/             # Model weights
├── src/                # Source code
├── README.md
└── requirements.txt
```

---

## ⚙️ Installation

```bash
git clone https://github.com/denarahmaron/license-plate-odd-even-yolov8.git
cd license-plate-odd-even-yolov8
pip install -r requirements.txt
```

---

## ▶️ Usage

### Run Detection (Image)

```bash
python detect.py --source image.jpg
```

### Run Detection (Video)

```bash
python detect.py --source video.mp4
```

---

## ⚠️ Limitations

* Dataset does not cover all license plate variations
* Limited computational resources (Google Colab GPU)
* Focus only on YOLOv8 model

---

## 💡 Future Improvements

* Integrate OCR (plate number recognition)
* Deploy as web application (React + API)
* Improve dataset diversity
* Optimize for edge devices (CCTV / IoT)

---

## 📖 Research Background

This project is based on a final thesis:

**"Optimalisasi Model Prediksi Pada Plat Nomor Ganjil Genap Menggunakan Algoritma YOLOv8"**
STMIK IKMI Cirebon – 2025

---

## 🤝 Contribution

Feel free to fork, improve, and contribute to this project.

---

## 📬 Contact

**Denar Ahmaron Surya Gemilang**

* GitHub: https://github.com/denarahmaron

---

## ⭐ Acknowledgment

Thanks to all contributors, mentors, and researchers who inspired this work in the field of computer vision and traffic systems.
