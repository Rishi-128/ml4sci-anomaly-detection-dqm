# Anomaly Detection for Data Quality Monitoring (DQM)

This project demonstrates reconstruction-based anomaly detection for
detector data quality monitoring using an autoencoder.

## Project Structure
- 01_data_generation.ipynb – Synthetic detector data simulation
- 02_autoencoder_training.ipynb – Train autoencoder on normal data
- 03_anomaly_detection.ipynb – Detect anomalies via reconstruction error

## Motivation
In high-energy physics experiments, detector conditions evolve over time.
Machine learning models can be used to identify abnormal behavior and
assist human operators in maintaining data quality.

## Tools Used
- Python
- NumPy
- PyTorch
- Matplotlib
