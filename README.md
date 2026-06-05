# Barcode Detection Using a Hybrid Digital Image Processing and CNN Framework

## Overview

This project presents a hybrid barcode detection system that combines Digital Image Processing (DIP) techniques with Convolutional Neural Networks (CNNs) to accurately detect and classify barcode regions in images.

The proposed approach utilizes image preprocessing, edge detection, morphological operations, and Region of Interest (ROI) extraction to localize potential barcode areas. These candidate regions are then validated using a lightweight CNN model, reducing computational cost while improving detection accuracy.

The system is designed to perform effectively in challenging environments involving noise, blur, rotation, varying illumination, and complex backgrounds.

---

## Objectives

* Detect barcode regions in real-world images.
* Reduce false positives through ROI-based classification.
* Improve barcode detection accuracy using a hybrid approach.
* Minimize computational complexity by processing only candidate regions.
* Compare full-image CNN classification with ROI-based CNN classification.

---

## Features

### Image Preprocessing

* RGB to Grayscale Conversion
* Gaussian Filtering
* Histogram Equalization

### Edge Detection

* Sobel Edge Detection
* Canny Edge Detection
* Vertical Gradient Analysis

### Morphological Processing

* Dilation
* Opening
* Closing

### ROI Extraction

* Contour Detection
* Connected Component Analysis
* Aspect Ratio Analysis
* Rectangularity Evaluation
* Edge Density Filtering

### CNN Classification

* Lightweight CNN Architecture
* Binary Classification (Barcode / Non-Barcode)
* Data Augmentation
* Dropout Regularization

---

## Proposed Workflow

1. Input Image
2. Image Preprocessing
3. Edge Detection
4. Morphological Operations
5. ROI Extraction
6. CNN-Based Classification
7. Barcode Detection Output

---

## Technologies Used

* Python
* OpenCV
* TensorFlow / Keras
* NumPy
* Matplotlib
* Digital Image Processing
* Convolutional Neural Networks (CNN)

---

## Dataset Preparation

The dataset consists of:

* Images containing barcodes
* Images without barcodes

Dataset preprocessing included:

* Image resizing
* Annotation and labeling
* Training, validation, and testing split
* Data augmentation for improved generalization

---

## Model Comparison

### Model A – Full Image CNN

* Validation Accuracy: 96.63%
* Validation Loss: 0.0888

### Model B – ROI-Based CNN

* Validation Accuracy: 99.52%
* Validation Loss: 0.0043

### Key Finding

The ROI-based CNN significantly outperformed the full-image CNN by reducing background interference and focusing only on candidate barcode regions.

---

## Results

* Improved barcode localization accuracy
* Reduced false detections
* Lower validation loss
* Enhanced performance in noisy and complex environments
* Efficient computational processing through ROI extraction

---

## Future Improvements

* Real-time barcode detection
* Multi-barcode detection support
* Barcode decoding integration
* Mobile deployment
* Support for QR codes and additional barcode formats
* Optimized inference speed for embedded systems

---

## Research Contribution

This project demonstrates that combining traditional Digital Image Processing techniques with CNN-based classification can significantly improve barcode detection performance while reducing computational requirements compared to full-image deep learning approaches.

---
