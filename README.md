# Calories Burned Prediction Model

A Machine Learning project focused on predicting energy expenditure (**Calories_Burned**) based on workout data.

## Preproccesing Phase

### 1. Cleaning & Quality Control
* **Outlier Removal**: Used the **IQR (Interquartile Range)** method to eliminate extreme physiological anomalies.
* **Duplicate Management**: Cleaned the dataset to ensure unique observations.
* **Integrity Check**: Confirmed a 100% complete dataset with no missing values.

### 2. Feature Engineering & Selection
* **Target Variable**: `Calories_Burned`

### 3. Advanced Transformations
* **OneHotEncoding**: Transformed categorical data (`Gender`, `Workout_Type`) into numerical format.
* **StandardScaler**: Normalized numerical features to a mean of 0 and standard deviation of 1.
* **Safe Split**: Applied a strict 80/20 train-test split *before* scaling to prevent any information leakage from the test set.
