# Wearable Stress Detection using Empatica E4

This project focuses on detecting stress using wearable sensor data collected from the Empatica E4 device.


##  Objective

The aim of this project is to:
- Analyse physiological signals (EDA, heart rate, temperature, movement)  
- Detect stress using machine learning  
- Build a complete pipeline from raw data to prediction  
- Test the model on an external dataset  
  

## Datasets

### 1. Empatica E4 Dataset
- Signals: EDA, HR, TEMP, ACC  
- Labels created using event tags (stress / rest)  

### 2. External Dataset
- Nurse Stress Prediction Wearable Sensors Dataset (Kaggle)  
- Real-world data from nurses  
- Used to test model generalisation  

Datasets are not included. Download and place them in the `data/` folder.


## Project Steps

1. Data exploration  
2. Preprocessing and label creation  
3. Feature extraction using sliding windows (10s, 30s, 60s)  
4. Statistical analysis (boxplots, t-tests)  
5. Machine learning (Logistic Regression & Random Forest)  
6. External validation on nurse dataset  


##  Files

- `01_explore.ipynb` – Data exploration  
- `02_labels.ipynb` – Label creation  
- `03_features.ipynb` – Feature extraction  
- `04_model.ipynb` – Model training  
- `05_overall_user_summary.ipynb` – Summary analysis  
- `06_external_validation.ipynb` – External dataset testing  


## Results

- Random Forest achieved ~80% accuracy on the original dataset  
- Accuracy dropped on external dataset  

 This shows the model does not generalise well to real-world data  


## Key Learning

- Wearable signals can be used to detect stress  
- Feature engineering is important  
- Models trained on one dataset may not generalise well  
- External validation is essential  


## Conclusion

This project successfully built a stress detection system using wearable data. However, testing on a real-world dataset showed a drop in performance, highlighting the importance of model generalisation.
