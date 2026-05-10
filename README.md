# Acoustic-Based Machine Health Monitoring

This project focuses on developing an **acoustic-based machine health monitoring system** for detecting abnormal machine behavior using sound signals. Instead of relying on physical contact sensors, the system analyzes machine audio to identify potential faults, enabling a **non-invasive and cost-effective** approach to predictive maintenance.

## Overview

Machine sounds are recorded and converted into **Mel-spectrograms**, which provide a time–frequency representation of the audio signal. These spectrograms capture important acoustic patterns that help distinguish between normal and faulty machine conditions.

A **Convolutional Autoencoder (CAE)** is trained exclusively on normal operating sounds so that it learns the standard acoustic behavior of the machine. During testing, the model attempts to reconstruct the input spectrogram, and the **reconstruction error** is used as an anomaly indicator.

* **Low reconstruction error** → Normal machine behavior
* **High reconstruction error** → Potential abnormality or fault

The system also incorporates spectral feature extraction and machine-specific analysis to improve detection performance and robustness.

## Features

* Acoustic-based fault detection
* Non-invasive machine monitoring
* Mel-spectrogram generation
* Spectral feature extraction
* Anomaly detection using Convolutional Autoencoder (CAE)
* Reconstruction error-based abnormality detection
* Machine-specific analysis using classification techniques
* Suitable for predictive maintenance applications

## Technologies Used

* Python
* Google Colab
* Librosa
* NumPy
* Scikit-learn
* TensorFlow / Keras
* Matplotlib

## Workflow

1. Audio Acquisition
   Machine sound signals are collected and digitized.

2. Preprocessing
   The audio is cleaned and converted into Mel-spectrogram representations.

3. Feature Extraction
   Spectral features such as centroid, bandwidth, energy, and dominant frequency are extracted.

4. Machine Identification
   A classifier is used for machine-specific analysis.

5. CAE-Based Anomaly Detection
   The Convolutional Autoencoder reconstructs normal patterns and calculates reconstruction error.

6. Fault Classification
   Reconstruction error and extracted features are combined for final fault prediction.

## Applications

* Predictive Maintenance
* Industrial Machine Monitoring
* Early Fault Detection
* Smart Manufacturing Systems
* Condition Monitoring

## Dataset

The project uses the **MIMII Dataset** (Malfunctioning Industrial Machine Investigation and Inspection Dataset) for training and evaluation.

## Future Improvements

* Real-time deployment on embedded systems
* Edge AI integration
* Noise-robust anomaly detection
* Multi-machine monitoring support
* Live dashboard visualization

## Authors

* Rohith A
* Sidharth M Pillai
* PS Shabarinaath
* Kishore V

