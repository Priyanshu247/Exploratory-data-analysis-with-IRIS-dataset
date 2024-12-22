# Iris Dataset Classification with Logistic Regression

## Objective
The goal of this project is to classify the species of Iris flowers (setosa, versicolor, virginica) based on the following features:
- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)

## Dataset
- **Source**: The Iris dataset is a classic dataset in machine learning, available in the Scikit-learn library.
- **Size**: 150 samples, 4 features, and 1 target class.
- **Target Classes**:
  - 0: Setosa
  - 1: Versicolor
  - 2: Virginica

## Steps in the Project

### 1. Data Exploration
- Loaded the dataset using Scikit-learn's `load_iris()` function and converted it to a Pandas DataFrame.
- Explored the dataset for:
  - Shape and basic statistics.
  - Distribution of features and their relationships using visualizations (e.g., pair plots).

### 2. Data Preprocessing
- Checked and handled missing values (none found).
- Identified and removed duplicate entries (1 duplicate found and removed).
- Standardized the features using `StandardScaler` to improve model performance.

### 3. Visualizations
- Plotted distributions of features with density smoothing curves.
- Created pair plots to explore the relationships between features and their separation across species.

### 4. Model Building
- Chose Logistic Regression as the classification model due to its simplicity and effectiveness for linearly separable data.
- Split the dataset into 70% training and 30% testing subsets.
- Trained the Logistic Regression model on the scaled training data.

### 5. Model Evaluation
- Evaluated the model using precision, recall, F1-score, and accuracy metrics.
- Achieved perfect classification:

```
              precision    recall  f1-score   support

           0       1.00      1.00      1.00        19
           1       1.00      1.00      1.00        13
           2       1.00      1.00      1.00        13

    accuracy                           1.00        45
   macro avg       1.00      1.00      1.00        45
weighted avg       1.00      1.00      1.00        45
```

### 6. Conclusions
- The Logistic Regression model successfully classified the Iris species with 100% accuracy on the test set.
- The dataset's features (especially petal dimensions) provided clear separation between species, contributing to the model's excellent performance.

## Folder Structure
```
Project/
├── notebooks/
│   └── Iris_EDA_and_Model.ipynb
├── README.md
```

## Future Work
- Experiment with more advanced models such as:
  - **Support Vector Machines (SVM)**
  - **Random Forest**
  - **K-Nearest Neighbors (KNN)**
- Apply hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
- Test the model's generalizability on noisy or more complex datasets.

## How to Run
1. Clone this repository:
   ```bash
   git clone <repository_url>
   ```
2. Run the Jupyter Notebook for step-by-step analysis and model building:
   ```bash
   jupyter notebook notebooks/Iris_EDA_and_Model.ipynb
   ```

---
This project is part of my data science portfolio. Feel free to reach out with any feedback or suggestions!
