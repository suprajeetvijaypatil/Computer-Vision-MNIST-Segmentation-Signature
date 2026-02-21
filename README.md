# Computer Vision & Machine Learning Portfolio

This repository contains three major tasks focused on image classification, structural image analysis, and biometric verification.These projects were developed as part of the Computer Vision curriculum at **SRH Hochschule Heidelberg**

## 📁 Projects Overview

### 1. Handwritten Digit Classification (MNIST)
* **Objective**: Automatically recognize handwritten digits (0–9) using the MNIST dataset.
* **Methodology**: Implemented a **Convolutional Neural Network (CNN)** using TensorFlow and Keras.
* **Architecture**: 
    * Two convolutional layers (32 and 64 filters) with ReLU activation to detect spatial patterns like edges and curves.
    * MaxPooling layers to reduce dimensionality while focusing on the most important features.
    * Dense layers with a Softmax output for 10-digit classification.
* **Performance**: Achieved a test accuracy of approximately **98.7%**.

### 2. Graph-Based Image Segmentation
* **Objective**: Segment an image into meaningful regions by grouping pixels that share similar properties.
* **Methodology**:
    * Treated the image as a graph where each pixel is a node.
    * Calculated edge weights based on the absolute difference in grayscale intensity between neighboring pixels.
    * Merged segments iteratively if the edge weight was below a defined threshold .
* **Results**: Demonstrated that a lower $\theta$ is sensitive to pixel differences, while a higher $\theta$ provides more tolerance for intensity changes and results in fewer segments.

### 3. Dynamic Signature Verification
* **Objective**: Verify identity using the writing process (pen position and timing) rather than just a static image[cite: 467].
* **Methodology**:
    * Decomposed trajectories into individual strokes based on pen-down/pen-up states.
    * Converted strokes into symbolic strings based on local $x$ and $y$ extrema tokens.
    * Compared signatures using an **Adapted Levenshtein (Minimum Edit Distance)** algorithm that operates at the stroke level.
* [cite_start]**Evaluation**: Successfully differentiated between genuine and forged signatures using a fixed threshold of 0.35.

---

## 🛠️ Tools & Technologies
* **Languages**: Python 
* **Libraries**: TensorFlow, Keras, OpenCV, NumPy, Matplotlib 
* **Environment**: Google Colab 

---

## 🎓 Academic Info
* **Student**: SUPRAJEET VIJAY PATIL 
* **Matriculation Number**: 100004941 
* **Institution**: Hochschule Heidelberg 
* **References**: Lecture notes by Professor Gnjatovic 

---

## 🚀 Getting Started
1. **Upload Notebooks**: Open the `.ipynb` files in Google Colab.
2. **Data Preparation**: Upload the required datasets (MNIST CSVs or Signature TXT files) as specified in the notebook instructions.
