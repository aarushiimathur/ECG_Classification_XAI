# ECG Anomaly Detection using Explainable AI (XAI)

This project integrates **Deep Learning** and **Explainable AI (XAI)** to classify ECG signals as *Normal* or *Abnormal* and provide interpretability for the model’s predictions. It enhances medical AI transparency by visualizing which ECG components (P, QRS, T waves) influenced the outcome.

---

## Overview

Traditional deep learning models achieve high accuracy in ECG classification but act as “black boxes.” This project combines a **Convolutional Neural Network (CNN)** for classification with **SHAP**, **Saliency Maps**, and **Autoencoders** for explainability.
The system allows clinicians and researchers to understand *why* an ECG was classified as abnormal.

---

## Features

* Classifies ECG signals using a 1D CNN architecture.
* Applies SHAP and Saliency Maps to highlight influential regions of the ECG.
* Uses Autoencoders for counterfactual reconstruction (normal vs abnormal comparison).
* Visualizes model reasoning via an interactive Streamlit dashboard.
* Enables transparent and trustworthy AI decision-making in cardiac analysis.

---

## Dataset

**MIT-BIH Arrhythmia Database (PhysioNet)**

* ECG signals segmented into 200-sample windows.
* SMOTE applied for class balance.
* Data preprocessed using the `wfdb` library for signal extraction and annotation.

---

## Methodology

1. **Data Preprocessing** – Load, segment, and normalize ECG signals.
2. **Model Training** – Train a 1D CNN for normal vs abnormal classification.
3. **Explainability Integration** –

   * **SHAP**: Identifies the contribution of each time point to the model’s prediction.
   * **Saliency Map**: Highlights regions of maximum gradient influence.
   * **Autoencoder**: Reconstructs ECG signals to show deviation from normal patterns.
4. **Visualization** – Interactive exploration through Streamlit.

---

## Technologies Used

* Python
* TensorFlow / Keras
* Scikit-learn
* NumPy, Matplotlib
* SHAP, wfdb, Streamlit

---

## Results

* CNN model achieved approximately **96.7% accuracy**.
* SHAP identified the **QRS region** as the most influential ECG segment.
* Autoencoder reconstructions effectively differentiated normal and abnormal signals.
* Balanced classification performance obtained using SMOTE.

---

## Real-World Impact

This project demonstrates how integrating **Explainable AI** techniques with deep learning can enhance the reliability of AI-assisted medical diagnosis. By providing transparency, it bridges the gap between machine predictions and clinical trust.

---

## Authors

* **Aarushi Mathur**
* **Anusri Kadam**
* **Alabhya Sharma**



