# 🩺 Chronic Kidney Disease Prediction

This project uses machine learning to predict the likelihood of chronic kidney disease based on clinical parameters. The final ensemble model achieves **up to 100% accuracy**.

## 📂 Project Structure

- `Kidney_disease_prediction.ipynb` — Complete end-to-end notebook
- `evc_kidney_disease.pkl` — Final saved VotingClassifier model
- `requirements.txt` — Python dependencies

## 📊 Dataset

- **Source**: [Kaggle Notebook](https://www.kaggle.com/code/niteshyadav3103/chronic-kidney-disease-prediction-98-accuracy)
- The dataset includes features such as blood pressure, albumin, blood glucose, etc.

## 🔧 Preprocessing Steps

- Missing values: `SimpleImputer`
- Encoding: Label Encoding
- Outlier removal: IQR capping
- Scaling: `MinMaxScaler` (range: -1 to 1)
- Dimensionality Reduction: `PCA`

## 🤖 Models Used

| Model                    | Accuracy Score |
|--------------------------|----------------|
| LogisticRegression       | 0.97           |
| DecisionTreeClassifier   | 1.00           |
| RandomForestClassifier   | 1.00           |
| BaggingClassifier        | 0.99           |
| GradientBoostingClassifier | 1.00         |
| KNeighborsClassifier     | 0.96           |
| SVC                      | 0.98           |
| BernoulliNB              | 0.93           |
| GaussianNB               | 1.00           |
| XGBClassifier            | 0.99           |
| VotingClassifier         | 1.00           |


## 🚀 Deployment

Final model saved as: evc_kidney_disease.pkl
