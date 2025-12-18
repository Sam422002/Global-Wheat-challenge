# Global Wheat Detection 🌾

## 📌 Project Overview
This repository contains a computer vision solution for the **Global Wheat Detection** challenge. The goal is to accurately detect and localize wheat heads in high-resolution outdoor field images.

Accurate estimation of wheat head density is a critical metric for crop health and yield estimation. However, outdoor field images present significant challenges, including:
* **Overlapping plants** (dense populations)
* **Wind blur** and motion artifacts
* **Varied lighting conditions** and backgrounds across different global regions (Europe, North America, etc.)

This project utilizes deep learning object detection techniques to address these issues and generalize across different growing environments.

## 📊 Performance Metrics
The model was evaluated using Mean Average Precision (mAP) and Recall. Below are the performance metrics achieved on the validation set:

| Metric | Value | Description |
| :--- | :--- | :--- |
| **mAP@0.5** | **0.8915** | Precision when IoU threshold is 0.5 |
| **mAP@0.5:0.95** | **0.7721** | Average mAP over thresholds 0.5 to 0.95 |
| **Mean Recall** | **0.7395** | Recall calculated at 100 detections |

> **Note:** These results were achieved after training for **28 epochs**. The model demonstrates strong detection capabilities at the standard 0.5 IoU threshold (approx 89% accuracy).

## 🛠️ Methodology & Approach
* **Dataset:** [Global Wheat Head Dataset](https://kaggle.com/competitions/global-wheat-detection) containing thousands of images from diverse global regions.
* **Model Architecture:** [Insert Model Name here, e.g., YOLOv5 / Faster R-CNN / EfficientDet]
* **Training Configuration:**
    * **Epochs:** 28
    * **Optimizer:** [e.g., SGD / Adam]
    * **Loss Function:** [e.g., Focal Loss / GIoU Loss]

## 🚀 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone [https://github.com/your-username/Global-Wheat-Detection.git](https://github.com/your-username/Global-Wheat-Detection.git)
   cd Global-Wheat-Detection
