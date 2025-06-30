 ❤️ Heart Disease Prediction using Decision Tree & Random Forest

 📌 Task Objective

To build and evaluate classification models using Decision Tree and Random Forest algorithms to predict whether a person has heart disease based on clinical data.

 🗂 Dataset Used

- Source: [Heart Disease UCI Dataset – Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
- Total Records: 1025
- Target Variable: `target` (1 = disease, 0 = no disease)

 🛠 Tools & Libraries

- Python
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`

 ✅ Steps Performed

 1. Data Exploration
- Checked for null values and data types (none missing ✅)
- Target distribution is binary: 0 or 1

 2. Data Splitting
- Used `train_test_split` (80% training / 20% testing)

 3. Model 1: Decision Tree Classifier
- Trained a full decision tree (no depth limit)
- Achieved high training accuracy but prone to **overfitting**
- Visualized full tree and simplified tree (`max_depth=3`)
- Accuracy with `max_depth=3`: ~78%

 4. Model 2: Random Forest Classifier
- Trained with 100 estimators
- Achieved **accuracy: 98.5%**
- Excellent classification report:
  - Precision (Class 1): 1.00
  - Recall (Class 1): 0.97
- Robust to overfitting and highly accurate

 5. Feature Importance
- Top features: `cp`, `ca`, `thalach`, `oldpeak`
- Less important: `fbs`, `restecg`

 6. Cross-Validation
- Performed 10-fold CV on Random Forest
- Ensured consistent performance across folds

 📊 Results Summary

| Model           | Accuracy |
|------------------|----------|
| Decision Tree (`max_depth=3`) | ~78.0% |
| Random Forest               | 98.5% |
| 10-Fold CV (RF)             | ~95–98% |


 📁 Files Included

- `heart.csv` — Dataset  
- `random-forest.ipynb` — Code  
- `README.md` — Project overview 


✅ Internship Task

AI & ML Internship – Task 5: Tree-Based Models  

