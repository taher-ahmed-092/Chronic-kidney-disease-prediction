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

                   Method used  Accuracy score
0           LogisticRegression            0.97
1       DecisionTreeClassifier            1.00
2       RandomForestClassifier            1.00
3            BaggingClassifier            0.99
4   GradientBoostingClassifier            1.00
5         KNeighborsClassifier            0.96
6                          SVC            0.98
7                  BernoulliNB            0.93
8                   GaussianNB            1.00
9                XGBClassifier            0.99
10            VotingClassifier            1.00

## 🚀 Deployment

Final model saved as: evc_kidney_disease.pkl
