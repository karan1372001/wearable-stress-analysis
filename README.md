# Wearable Stress Detection using Empatica E4

This project focuses on detecting stress using physiological signals collected from wearable devices (Empatica E4) using machine learning techniques.


# Objective

The aim of this project is to:

1 Analyse physiological signals such as EDA, heart rate, temperature, and movement  
2 Detect stress vs non-stress using machine learning models  
3 Build a complete data pipeline from raw signals to prediction  
4 Evaluate model performance on unseen real-world data  
5 Understand why models fail to generalise across different datasets  


# Datasets

# 1. Empatica E4 Dataset (Main Dataset)
- Collected in a controlled environment  
- Signals: EDA, HR, TEMP, ACC  
- Labels generated using event tags (stress / rest)    


# 2. Nurse Dataset (External Dataset)
- Real-world data collected from nurses  
- Used to test model generalisation  
- Contains different conditions compared to lab data    


# Project Pipeline

The project was developed step-by-step:

1. # Data Exploration**  
   - Understanding structure of physiological signals  

2. # Preprocessing & Label Creation**  
   - Time alignment, cleaning, and stress label generation  

3. # Feature Extraction**  
   - Sliding window approach (10s, 30s, 60s)  
   - Statistical features: mean, standard deviation  

4. # Model Development**  
   - Logistic Regression  
   - Random Forest  

5. # External Validation**  
   - Tested model on nurse dataset  

6. # Feature Distribution Analysis**  
   - Compared EDA, HR, and Temperature distributions  
   - Identified why model failed  


# Project Files

- `01_explore.ipynb` – Data exploration  
- `02_labels.ipynb` – Label generation  
- `03_features.ipynb` – Feature extraction  
- `04_model.ipynb` – Model training and evaluation  
- `05_overall_user_summary.ipynb` – Summary analysis  
- `06_external_validation.ipynb` – Testing on nurse dataset
  

# Results

- Random Forest achieved **~80% accuracy** on the original dataset  
- Model performance dropped to **0 accuracy on the nurse dataset**  


# Key Insight

The model failed because:

- The nurse dataset has **different feature distributions**  
- EDA, heart rate, and temperature patterns are not similar  
- Data was collected in **real-world conditions**, unlike controlled lab data  

This shows that the model **could not generalise to new data**


# Key Learning

- Wearable signals can be used for stress detection  
- Feature engineering is critical for time-series data  
- Models trained on one dataset may fail on another  
- External validation is essential in machine learning  
- Data distribution plays a major role in model performance  


# Conclusion

This project successfully built a stress detection system using wearable data. However, testing on a real-world dataset revealed a complete failure in performance, highlighting the importance of generalisation and dataset differences.
  
- Handling class imbalance  
- Training on multiple datasets  
