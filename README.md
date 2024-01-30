# Anomaly Detection
![blogimage-450476-](https://github.com/quant-dot-ai/predictive-maintenance-using-autoencoders/assets/146693417/35ec0a18-bb01-4d7f-9517-627db3d5c20b)
_![image source:](https://www.google.com/url?sa=i&url=https%3A%2F%2Ftracked.ai%2Fblog-desc.aspx%3Fu%3Danomaly-detection-as-a-data-analytics-professional&psig=AOvVaw17vACJrQjgemp_KrBwLi5q&ust=1706668451352000&source=images&cd=vfe&opi=89978449&ved=0CBUQjhxqFwoTCLj6iciJhIQDFQAAAAAdAAAAABAE)_


## Introduction

This project aims to implement predictive maintenance in the Metro do Porto's Air Production Unit (APU) using deep learning techniques. The motivation is to identify machinery failures early, using autoencoder networks to detect anomalies in sensor data and reduce false alarms. The project's goal is to improve safety and efficiency in metro rail systems by preemptively identifying and addressing potential failures.

## Data Description

The MetroPT-3 dataset, collected from February to August 2020, forms the basis of this study. It comprises 15,169,480 data points with 15 features from 7 analog and 8 digital sensors. These sensors include pressure measurements (TP2, TP3, H1, DV pressure, Reservoirs), Motor Current, Oil Temperature, and various digital signals like COMP, DV electric, TOWERS, MPG, LPS, Pressure Switch, Oil Level, and Caudal Impulse.

## Tools and Technologies Used

- **Deep Learning**: For constructing predictive models using autoencoder networks.
- **Sparse Autoencoders**: Employed for their ability to represent data sparsely, enhancing anomaly detection.
- **Variational Autoencoders**: Used for their probabilistic approach in representing data.
- **Performance Metrics**: F1 Score, Recall, and Precision for assessing model performance.

## Analysis

Two types of autoencoders, sparse and variational, were tested with both analog and digital sensor data. The analysis involved examining the sensor data trends during normal operation and failure, using binary classification techniques and time to failure prediction methods initially. However, these methods were not effective for preemptive failure detection, leading to the adoption of autoencoder networks.

## Results

The study found that digital sensor data, especially with sparse autoencoders, was more effective in anomaly detection. The sparse autoencoder model demonstrated nearly 100% accuracy in F1 Score, Recall, and Precision for anomalies flagged 24 hours before failure. This contrasts with variational autoencoders and models using analog signals, which showed lower performance metrics.

## Scope for Further Development

Future work involves integrating advanced techniques like LSTM, Transformers, Causal Forest, and Survival Analysis for improved prediction and understanding of the factors leading to system failures. The focus will be on not just detecting anomalies but also proactively monitoring and maintaining system integrity through advanced, data-driven methodologies.

### Formal Report
You can read a blog post on this project [here](https://medium.com/@vgupta701/metro-rail-predictive-maintenance-based-on-anomaly-detection-0008ffa7a5b7)

