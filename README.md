# Driving Behavior Classification

Time-series classification of driving behavior (aggressive, normal, slow) using smartphone accelerometer and gyroscope data. 

## Overview
Understanding driving behavior is important for applications such as ride-sharing safety, insurance risk modeling, and fleet monitoring. This project uses time-series sensor data from smartphones to classify driving styles. 

## Data Sources
- Driving Behavior Dataset (Kaggle): https://www.kaggle.com/datasets/outofskills/driving-behavior

## Methodology

### Feature Engineering
- Acceleration magnitude
- Gyroscope magnitude
- Sliding window segmentation
- Majority label assignment per window

### Models
- Random Forest (baseline)
- CNN
- CNN + GRU
- CNN + LSTM

### Evaluation:
- Accuracy and macro F1-score
- Averaged performance across multiple random seeds
- Per-class precision/recall analysis
 
## Results
- CNN-based models outperform Random Forest baseline, achieving up to 6% higher accuracy than in prior work (https://rochi.utcluj.ro/articole/10/RoCHI2022-Cojocaru-I-2.pdf)
- Aggressive and slow driving are well-classified due to distinct signal patterns
- "Normal" driving is consistently underpredicted

## Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- TensorFlow, Keras

