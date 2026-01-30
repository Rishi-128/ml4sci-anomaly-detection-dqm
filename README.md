# Anomaly Detection for Data Quality Monitoring (DQM)

This project demonstrates an end-to-end machine learning pipeline for **anomaly detection in detector data quality monitoring (DQM)** using reconstruction-based methods and continuous learning.

The work is motivated by challenges in **high-energy physics experiments**, where detector conditions evolve over time, causing data drift and degradation in model performance. The project explores how **continuous learning** can mitigate these effects.

---

## 📌 Project Overview

In many scientific experiments, especially in high-energy physics, it is crucial to monitor detector data in real time to detect abnormal behavior. Traditional machine learning models trained once on historical data often fail when detector conditions change.

This project addresses that problem by:
- Detecting anomalies using an **autoencoder trained on normal data**
- Simulating **data drift** to reflect changing detector conditions
- Applying **continuous learning** to adapt the model over time

---

## 🧪 Methodology

### 1. Synthetic Detector Data Generation
- Normal samples represent stable detector behavior
- Anomalous samples simulate detector faults or abnormal conditions

### 2. Autoencoder-Based Anomaly Detection
- An autoencoder is trained **only on normal data**
- Anomalies are identified using **reconstruction error**

### 3. Data Drift Simulation
- Gradual changes are introduced into the data distribution
- Model performance degradation is analyzed over time

### 4. Continuous Learning
- The model is incrementally updated as new data arrives
- Continuous learning reduces reconstruction error under drift

---

## 📂 Repository Structure
```
├── 01_data_generation.ipynb # Synthetic detector data simulation
├── 02_autoencoder_training.ipynb # Training autoencoder on normal data
├── 03_anomaly_detection.ipynb # Anomaly detection via reconstruction error
├── 04_data_drift_simulation.ipynb # Performance degradation under data drift
├── 05_continuous_learning.ipynb # Online adaptation using continuous learning
└── README.md
```

---

## 📊 Key Results

- Clear separation between normal and anomalous data using reconstruction error
- Observable performance degradation under simulated data drift
- Continuous learning successfully mitigates degradation and restores performance

---

## 🛠️ Technologies Used

- Python
- NumPy
- PyTorch
- Matplotlib
- Jupyter / Google Colab

---

## 🎯 Relevance to ML4DQM (GSoC 2026)

This project aligns closely with the **ML4DQM** initiative by:
- Addressing detector data quality monitoring
- Using unsupervised anomaly detection
- Handling evolving detector conditions
- Exploring continuous learning strategies

---

## 🚀 Future Work

- Apply the pipeline to real detector datasets
- Explore advanced continual learning techniques
- Benchmark against alternative anomaly detection models

