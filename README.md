# Wearable Stress and Exercise Analysis

This repository contains an internship project focused on analyzing wearable physiological data collected using the Empatica E4 device.

## Project Objective
To analyze stress, aerobic, and anaerobic physiological responses using Electrodermal Activity (EDA) signals and build a complete data analysis pipeline.

## Dataset
- Wearable data collected using Empatica E4
- Conditions analyzed:
  - Stress
  - Aerobic exercise
  - Anaerobic exercise
- Raw data is not included due to size and privacy constraints

## Project Structure
- `01_explore.ipynb` – Exploratory data analysis and visualization  
- `02_labels.ipynb` – Stress and rest label generation using event tags  
- `03_features.ipynb` – Feature extraction from EDA signals  
- `04_model.ipynb` – Machine learning models for stress detection  
- `05_overall_user_summary.ipynb` – Overall per-user analysis across all conditions  

## Conclusion
The project demonstrates that wearable EDA signals can be effectively used to study stress and physical activity. The pipeline can be extended with additional signals and advanced models in future work.
