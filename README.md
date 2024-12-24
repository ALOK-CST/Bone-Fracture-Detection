# Bone Fracture Detection

This repository contains a bone fracture detection project implemented using **CNN**, **ResNet**, and **YOLO** models. The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/pkdarabi/bone-fracture-detection-computer-vision-project).

---

## Table of Contents 📋

- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Results](#results)
- [File Structure](#file-structure)
- [How to Use](#how-to-use)
- [Visualization](#visualization)
- [Contributing](#contributing)
- [License](#license)
- [References](#references)

---

## Overview 

Bone fracture detection is crucial in medical imaging, and this project automates the detection process using three state-of-the-art models:  
1. **Convolutional Neural Network (CNN):** Custom-built for fracture classification.  
2. **ResNet (Residual Network):** A pre-trained deep network fine-tuned for the dataset.  
3. **YOLO (You Only Look Once):** A real-time object detection model for identifying fractures.  

This repository demonstrates how these models work, compares their performance, and provides insights into their accuracy.  

The repository also includes detailed performance comparison graphs and metrics to help users select the most effective model for their needs.

---

## Dataset 

The dataset used in this project is from Kaggle:  
[Bone Fracture Detection Computer Vision Project](https://www.kaggle.com/datasets/pkdarabi/bone-fracture-detection-computer-vision-project).  

### Dataset Instructions:  
1. Download the dataset from the above link.  
2. Extract it and place the files in the `dataset/` directory.  

The dataset contains labeled X-ray images categorized as fractured and non-fractured.

---

## Features 

This project is packed with exciting features:

### 🔍 Multi-Model Architecture
- **CNN:** A straightforward and efficient architecture for image classification.  
- **ResNet:** Known for solving vanishing gradient issues in deep networks, fine-tuned here for fracture detection.  
- **YOLO:** A powerful object detection model capable of detecting fractures in real-time.

### 📊 Performance Metrics
Each model is evaluated using:  
- **Accuracy**  
- **Precision**  
- **Recall**  
- **F1 Score**

### 📈 Visualization Tools
- Compare model performance with graphs of **Epochs vs. Accuracy**.  
- Visualize predictions and detections for better interpretability.

---

## Results 

Key results of the models:
1. **CNN:**  
   - Accuracy: 88%  
   - F1 Score: 0.85  

2. **ResNet:**  
   - Accuracy: 92%  
   - F1 Score: 0.91  

3. **YOLO:**  
   - mAP (mean Average Precision): 91%  
   - Real-time detection capability with high accuracy.  

Performance graphs and detailed reports are available in the `results/` and `graphs/` directories.

---

## File Structure 

```plaintext
Bone-Fracture-Detection/
├── dataset/
│   └── [X-ray images dataset]
├── models/
│   ├── cnn_model.py
│   ├── resnet_model.py
│   ├── yolo_model.py
├── results/
│   ├── cnn_results.csv
│   ├── resnet_results.csv
│   ├── yolo_results.json
├── graphs/
│   ├── epochs_vs_accuracy.png
│   └── confusion_matrices/
├── main.py
├── requirements.txt
├── README.md
└── LICENSE
```
---

## How to Use

### Prerequisites

- Install Python 3.7 or higher.
- Install the required dependencies:

```bash
pip install -r requirements.txt
```
### Steps to Run
1. **Clone this repository:**
```bash
git clone https://github.com/ALOK-CST/Bone-Fracture-Detection.git
```
2. **Navigate into the project directory:**
```bash
cd Bone-Fracture-Detection
```
3. **Place the dataset in the dataset/ directory.**
4. **Run the script to train a model (e.g., ResNet):**
```bash
python models/resnet_model.py
```
5. **View the results and graphs in the results/ and graphs/ folders.**

---

## Visualization

### Sample visualization tools provided in this repository:

1. **Predicted vs. Actual Labels (Confusion Matrix).**
2. **Detection Boxes on X-ray Images (for YOLO).**
3. **Graphs of Epochs vs. Accuracy.**

---

## Contributing

### Contributions are welcome!

1. **Fork the repository.**
2. **Create a new branch.**
3. **Commit your changes and create a pull request.**

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## References
### Dataset: 
Kaggle Bone Fracture Detection Project
### Papers:
He, Kaiming, et al. "Deep Residual Learning for Image Recognition."
Redmon, Joseph, et al. "You Only Look Once: Unified, Real-Time Object Detection."

---
