# 🧠 Multi-Modal Deep Learning for Cancer Detection Across Imaging Techniques

This project implements a **multi-modal deep learning framework** that integrates three imaging sources — **X-Ray**, **Histopathology**, and **Ultrasound** — to improve cancer detection accuracy.  
By combining features from diverse modalities using **ResNet50 feature extraction** and a **custom MLP classifier**, this approach provides a more holistic understanding of medical imaging data for early disease diagnosis.

---

## 📌 Overview

| Stage | Description |
|-------|--------------|
| **1. Data Collection** | Loads and organizes X-Ray, Histopathology, and Ultrasound image datasets. |
| **2. Label Standardization** | Cleans and aligns label classes across modalities. |
| **3. Image Preprocessing** | Normalization, resizing, and augmentation for better generalization. |
| **4. Feature Extraction** | Uses **ResNet50** to generate 2048-dimensional embeddings for each modality. |
| **5. Feature Fusion** | Concatenates embeddings (6144-dim vector) into a unified feature representation. |
| **6. Model Training** | Trains a **Multi-Layer Perceptron (MLP)** with class weighting to handle imbalance. |
| **7. Evaluation** | Generates metrics such as accuracy, confusion matrix, ROC curves, and classification reports. |

---

## 🧩 Key Features

- **Multi-Modal Integration:** Combines multiple imaging types for robust detection.
- **Transfer Learning:** Leverages pretrained **ResNet50** for efficient feature extraction.
- **Class Imbalance Handling:** Uses augmentation and weighted losses.
- **Comprehensive Evaluation:** Includes confusion matrices, ROC curves, and precision-recall analysis.
- **Extensible Framework:** Easily adaptable to other medical imaging modalities.

---

## ⚙️ Tech Stack

- **Languages:** Python  
- **Frameworks:** PyTorch, FastAI, TensorFlow (for preprocessing)  
- **Libraries:** OpenCV, NumPy, Pandas, Matplotlib, Scikit-learn  
- **Model Architectures:** ResNet50, Multi-Layer Perceptron (custom)  
