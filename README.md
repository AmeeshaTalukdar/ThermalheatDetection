# 🌡️ Thermal Human Detection Using YOLO & Thermal Imaging

<div align="center">

# Detecting Humans Beyond Visible Light

### Leveraging Thermal Imaging, Computer Vision, and YOLO for Reliable Human Detection in Challenging Environments

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)
![YOLO](https://img.shields.io/badge/YOLO-Object%20Detection-green?style=for-the-badge)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-red?style=for-the-badge&logo=opencv)
![Roboflow](https://img.shields.io/badge/Roboflow-Dataset%20Management-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Research%20Project-success?style=for-the-badge)

</div>

---

## 📖 Overview

Traditional human detection systems rely heavily on RGB cameras and visible-light imagery. While effective in well-lit environments, these systems often fail under conditions such as:

- 🌑 Complete darkness
- 🌫️ Smoke-filled environments
- 🌧️ Poor weather conditions
- 🚨 Emergency and rescue situations
- 🏭 Industrial safety applications

This project addresses these limitations by leveraging **thermal imaging** and **YOLO-based object detection** to identify humans through their heat signatures rather than visible appearance.

By combining advanced image preprocessing, dataset balancing, augmentation techniques, and thermal computer vision, the system provides a robust solution for detecting human presence in low-visibility environments.

---

## 🎯 Project Goals

- Detect humans using thermal imagery.
- Improve detection performance in low-visibility conditions.
- Build a balanced thermal imaging dataset.
- Enhance thermal image quality using contrast enhancement.
- Apply augmentation techniques to improve model generalization.
- Prepare datasets for YOLO training and deployment.

---

## 🔬 Methodology

The complete workflow follows a structured computer vision pipeline:

```text
Raw Thermal Images
        │
        ▼
 Dataset Collection
        │
        ▼
 Annotation Processing
        │
        ▼
 Dataset Balancing
        │
        ▼
 CLAHE Enhancement
        │
        ▼
 Data Augmentation
        │
        ▼
 Roboflow Integration
        │
        ▼
 COCO Conversion
        │
        ▼
 YOLO Training
        │
        ▼
 Human Detection
```

---

## ✨ Key Features

### 📦 Dataset Processing

- Automatic extraction of thermal image datasets
- Label management and verification
- Organized image-label pairing
- Dataset preparation for training

---

### ⚖️ Intelligent Dataset Balancing

Thermal datasets often contain highly uneven distributions of human instances.

This project implements balancing strategies to:

- Reduce dataset bias
- Improve model generalization
- Ensure representative training samples
- Optimize learning across varying crowd densities

---

### 🌈 Thermal Image Enhancement

#### CLAHE (Contrast Limited Adaptive Histogram Equalization)

Thermal images often suffer from poor contrast.

CLAHE is applied to:

- Improve local contrast
- Highlight thermal signatures
- Enhance object boundaries
- Improve feature extraction for YOLO

---

### 🔄 Data Augmentation

To increase dataset diversity, augmentation techniques are applied using Albumentations.

Examples include:

- Geometric transformations
- Scaling
- Rotation
- Distortion
- Random image variations

Benefits:

✅ Improved robustness

✅ Reduced overfitting

✅ Better real-world performance

---

## 🤖 Human Detection Using YOLO

The processed thermal dataset is used to train a YOLO object detection model capable of identifying human presence directly from thermal signatures.

### Detection Class

| Class ID | Object |
|----------|---------|
| 0 | Human |

Unlike traditional RGB-based systems, the model learns thermal patterns that remain visible regardless of ambient lighting conditions.

---

## ☁️ Roboflow Integration

The project utilizes Roboflow for efficient dataset management.

### Features

- Dataset versioning
- Annotation management
- Dataset visualization
- COCO export support
- YOLO-ready dataset generation

### Workflow

```text
Enhanced Dataset
       │
       ▼
 Roboflow Upload
       │
       ▼
 Dataset Versioning
       │
       ▼
 COCO Export
       │
       ▼
 YOLO Training
```

---

## 📊 Dataset Analysis

The notebook includes extensive statistical analysis of the thermal dataset:

- Human count distribution
- Mean occupancy statistics
- Median occupancy analysis
- Standard deviation measurements
- Percentile-based analysis
- Visualization of dataset characteristics

These insights help improve dataset quality and model performance.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Core Development |
| OpenCV | Image Processing |
| YOLO | Object Detection |
| Roboflow | Dataset Management |
| Albumentations | Data Augmentation |
| NumPy | Numerical Computing |
| Matplotlib | Visualization |
| Google Colab | Training Environment |

---

## 📁 Project Structure

```bash
Thermal-Human-Detection/
│
├── dataset/
│   ├── images/
│   ├── labels/
│   └── enhanced_dataset/
│
├── balanced_dataset/
│
├── images_clahe/
│
├── images_augmented/
│
├── coco_dataset/
│
├── main.ipynb
│
└── README.md
```

---

## 🚀 Applications

### 🔥 Fire & Rescue Operations
Locate individuals through smoke and fire-affected environments.

### 🌙 Night Surveillance
Detect human activity in complete darkness.

### 🚁 Search & Rescue Missions
Support thermal drone-based victim detection.

### 🏭 Industrial Safety Monitoring
Monitor worker presence in hazardous zones.

### 🚨 Security Systems
Enhance perimeter monitoring under poor visibility conditions.

---

## 📈 Why Thermal Imaging?

Traditional cameras depend on reflected visible light.

Thermal cameras detect emitted infrared radiation:

| RGB Cameras | Thermal Cameras |
|------------|----------------|
| Require lighting | Work in darkness |
| Sensitive to shadows | Independent of lighting |
| Visibility-dependent | Heat-dependent |
| Performance drops in smoke | Better penetration in low visibility |

This makes thermal imaging particularly effective for human detection applications.

---

## 🔮 Future Improvements

- [ ] YOLOv8 / YOLOv11 training and benchmarking
- [ ] Real-time thermal video inference
- [ ] Multi-object tracking
- [ ] Edge-device deployment
- [ ] Thermal-RGB sensor fusion
- [ ] Performance comparison with RGB-based detectors
- [ ] Live drone integration

---

## 📌 Conclusion

This project demonstrates how thermal imaging combined with modern object detection techniques can overcome many limitations of traditional human detection systems.

By integrating:

- Thermal Vision
- Image Enhancement
- Dataset Balancing
- Data Augmentation
- YOLO Object Detection

the system provides a powerful framework for reliable human detection in environments where conventional vision systems struggle.

> **Humans emit heat regardless of lighting conditions. Thermal imaging allows us to see what traditional cameras cannot.**

---



Computer Vision • Deep Learning • Thermal Imaging • Object Detection

---

### ⭐ If you found this project useful, consider starring the repository and contributing to future improvements.
