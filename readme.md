**Multiomics Data Analysis README**

---

### Dataset:
The dataset used in this project is named `task1_multiomics_data`. It contains multiomics data for analysis.

### Exploratory Data Analysis (EDA):
The EDA file (`EDA_of_Multiomics.ipynb`) explores the dataset to gain insights and understand its characteristics.

### Regression Model Performance Summary:

#### Linear Regression:
- **Without Data Normalization:**
  - Mean Squared Error: 247.53
  - Mean Absolute Error: 10.81
  - R-squared: -1.44
- **With Data Normalization:**
  - Mean Squared Error: 113.82
  - Mean Absolute Error: 7.99
  - R-squared: -0.12

#### Support Vector Regression (SVR):
- **Best Hyperparameters:** {'C': 1, 'gamma': 'scale', 'kernel': 'linear'}
- **Without Data Normalization:**
  - Mean Squared Error: 193.92
  - Mean Absolute Error: 9.24
  - R-squared: -0.91
- **With Data Normalization:**
  - Mean Squared Error: 145.71
  - Mean Absolute Error: 8.85
  - R-squared: -0.43

#### Decision Tree:
- **Best Hyperparameters:** {'max_depth': 6, 'min_samples_leaf': 3, 'min_samples_split': 13}
- **Without Data Normalization:**
  - Mean Squared Error: 221.99
  - Mean Absolute Error: 12.18
  - R-squared: -1.18
- **With Data Normalization:**
  - Mean Squared Error: 221.99
  - Mean Absolute Error: 12.18
  - R-squared: -1.18

#### Random Forest:
- **Best Hyperparameters:** {'max_depth': 11, 'min_samples_leaf': 2, 'min_samples_split': 7, 'n_estimators': 101}
- **Without Data Normalization:**
  - Mean Squared Error: 124.49
  - Mean Absolute Error: 9.34
  - R-squared: -0.22
- **With Data Normalization:**
  - Mean Squared Error: 127.97
  - Mean Absolute Error: 9.56
  - R-squared: -0.26

### Observations (Regression):
- Linear Regression with data normalization performs the best.
- SVR and Linear Regression benefit from data normalization, while Decision Tree's performance remains consistent.
- Random Forest's performance is slightly impacted by normalization.

### Classification Models:
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- AdaBoost
- XGBoost

### Observations (Classification):
- SVM achieved perfect accuracy (100%).
- Decision Tree and XGBoost showed competitive performance with accuracies around 82-83%.
- Random Forest performed well with an accuracy of 88.24%.

### Note:
- Data normalization has varying effects on regression models but didn't significantly impact classification models in this analysis.

---