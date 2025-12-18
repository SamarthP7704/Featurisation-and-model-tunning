# **Featurisation and Model Tuning for Semiconductor Yield Prediction**

## **Overview**

This project focuses on predicting Pass or Fail yield outcomes in a semiconductor manufacturing process using high-dimensional sensor data. Fabrication lines typically collect hundreds of signals per production entity, and only a subset of these signals contributes meaningfully to final yield.

The purpose of this project is to build a classification model and determine whether all available features are required, or if a reduced feature set provides more efficient and accurate predictions.

---

## **Dataset**

**File:** `sensor-data.csv`
**Shape:** 1567 rows × 592 columns

* 591 columns represent sensor-derived features
* 1 column represents the target yield label
* Target values:

  * `-1` = Pass
  * `1` = Fail

Each row corresponds to a single production entity at a specific test point in the manufacturing process.

---

## **Objectives**

1. Predict Pass/Fail yield for semiconductor production entities.
2. Evaluate the relevance of all features and determine whether dimensionality reduction improves performance.
3. Apply data cleansing, exploratory analysis, feature selection, and model tuning techniques.

---

## **Project Steps**

### **1. Data Import and Exploration**

* Loaded the dataset and inspected its structure, shape, types, and summary statistics.
* Examined target distribution and identified potential data quality issues.

### **2. Data Cleansing**

* Handled missing values using appropriate strategies based on feature characteristics.
* Removed irrelevant or constant features.
* Performed necessary transformations such as scaling or outlier adjustments.

### **3. Feature Engineering and Selection**

* Identified informative features using statistical, filter-based, and model-based selection methods.
* Evaluated multicollinearity and redundancy.
* Assessed dimensionality reduction impact on model performance.

### **4. Model Development**

* Trained classification models on both full and reduced feature sets.
* Optimised hyperparameters to improve predictive performance.
* Compared models to determine the most reliable approach.

### **5. Evaluation**

* Measured accuracy, precision, recall, F1-score, and confusion matrix metrics.
* Analysed whether reduced feature subsets provided comparable or improved results.
* Documented key insights from model tuning and feature relevance.

---

## **Technologies Used**

* Python
* NumPy
* Pandas
* Scikit-learn
* Matplotlib / Seaborn
* Jupyter Notebook

---

## **Conclusion**

This project demonstrates how feature selection and model tuning can significantly improve predictive accuracy and efficiency in semiconductor manufacturing environments. The results highlight the importance of identifying the most informative sensor signals and reducing unnecessary dimensionality in high-volume industrial datasets.

---
