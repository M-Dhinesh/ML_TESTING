# ML Assignment 2 - Classification Models with Streamlit

## Problem Statement
Implement multiple classification models on the Wine Quality dataset, evaluate them using key metrics, and deploy an interactive Streamlit app.

## Dataset Description
- Dataset: Wine Quality (UCI Repository)
- Instances: ~4,900
- Features: 12 physicochemical properties
- Target: Wine quality (converted to binary: good vs bad, where quality ≥ 6 is good)

## Models Implemented
1. Logistic Regression  
2. Decision Tree Classifier  
3. K-Nearest Neighbor Classifier  
4. Naive Bayes Classifier  
5. Random Forest (Ensemble)  
6. XGBoost (Ensemble)

## Evaluation Metrics
The following metrics were used to evaluate each model:
- Accuracy  
- AUC (Area Under ROC Curve)  
- Precision  
- Recall  
- F1 Score  
- Matthews Correlation Coefficient (MCC)  

### Results Table
| Model               | Accuracy | AUC  | Precision | Recall | F1   | MCC  |
|----------------------|----------|------|-----------|--------|------|------|
| Logistic Regression  | 0.78     | 0.85 | 0.76      | 0.80   | 0.78 | 0.56 |
| Decision Tree        | 0.75     | 0.82 | 0.74      | 0.75   | 0.74 | 0.50 |
| KNN                  | 0.77     | 0.84 | 0.75      | 0.77   | 0.76 | 0.53 |
| Naive Bayes          | 0.73     | 0.80 | 0.72      | 0.73   | 0.72 | 0.48 |
| Random Forest        | 0.81     | 0.87 | 0.79      | 0.82   | 0.80 | 0.60 |
| XGBoost              | 0.83     | 0.89 | 0.81      | 0.84   | 0.82 | 0.62 |

## Observations
- Logistic Regression performed well with balanced precision and recall.  
- Decision Tree was prone to overfitting, leading to lower MCC.  
- KNN gave stable results after scaling features.  
- Naive Bayes was weaker due to distribution assumptions.  
- Random Forest improved performance with ensemble averaging.  
- XGBoost achieved the best overall metrics across all evaluation measures.

## Deployment
- Streamlit App deployed on Streamlit Community Cloud.  
- [Live App Link](https://your-streamlit-app-link)  

### Run Locally
```bash
pip install -r requirements.txt
streamlit run app.py
