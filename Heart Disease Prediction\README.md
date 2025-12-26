# Heart Disease Prediction using Logistic Regression
## Problem Statement
Heart disease is one of the leading causes of death worldwide.  
Early prediction can help doctors and patients take preventive measures.  
This project aims to predict whether a person is likely to have heart disease based on medical attributes using a **Logistic Regression** machine learning model.
## Dataset
- **Source:** Kaggle  
- **Total Rows:** 1025  
- **Total Features:** 14  
- **Target Variable:** Heart Disease (0 = No, 1 = Yes)  
## Tools & Technologies
- Python  
- Google Colab  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Scikit-learn
## Project Workflow
### Data Collection
The dataset was downloaded from Kaggle and uploaded to Google Colab.  
It contains patient medical records with multiple health-related attributes.
### Data Exploration
- Checked dataset shape and data types  
- Verified missing values  
- Analyzed feature distributions  
### Data Preprocessing
- Selected relevant features  
- Split data into **features (X)** and **target (y)**  
- Performed **train-test split (80% training, 20% testing)**  
- Applied feature scaling using **StandardScaler**
### Model Selection
**Logistic Regression** was chosen because:
- It is suitable for binary classification problems  
- Easy to interpret  
- Performs well on medical datasets  
### Model Training
- Model trained on the training dataset  
- Learned relationships between medical attributes and heart disease outcome  
### Model Evaluation
Model performance evaluated using:
- Accuracy Score  
- Confusion Matrix  
- Classification Report (Precision, Recall, F1-score)  
## Results
- Logistic Regression achieved good prediction accuracy  
- Model successfully classified patients with and without heart disease  
- Balanced performance on both positive and negative classes  
## Future Improvements
- Apply advanced models (Random Forest, XGBoost, Neural Networks)  
- Perform hyperparameter tuning  
- Add feature importance analysis  
- Use cross-validation for better generalization  
## How to Run
1. Open Google Colab  
2. Upload the dataset  
3. Install required libraries  
4. Run the notebook cells sequentially  
5. Train and evaluate the model  

---
