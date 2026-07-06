# Diabetes Prediction using Machine Learning 🩺

A machine learning project that predicts the likelihood of diabetes in patients based on diagnostic medical features, using a Gradient Boosting classifier.

## 📌 Project Description

This project applies supervised machine learning to the classic **Pima Indians Diabetes** dataset to classify patients as diabetic or non-diabetic. The pipeline includes data cleaning, feature scaling, and model training with a Gradient Boosting classifier, along with visual evaluation through confusion matrix and related plots.

## 📊 Dataset

The dataset contains the following features:

| Feature | Description |
|---|---|
| Pregnancies | Number of times pregnant |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure (mm Hg) |
| SkinThickness | Triceps skin fold thickness (mm) |
| Insulin | 2-Hour serum insulin (mu U/ml) |
| BMI | Body mass index |
| DiabetesPedigreeFunction | Diabetes pedigree function score |
| Age | Age (years) |

**Target:** Outcome (1 = diabetic, 0 = non-diabetic)

## 🧹 Data Preprocessing

- Rows containing missing or invalid values were **removed** from the dataset.
- Features were **scaled/normalized** (StandardScaler / MinMaxScaler) prior to model training.
- Note: no explicit technique was applied to address potential class imbalance in this version.

## Result 

| Metric | Score |
|--------|-------|
| Recall  | 0.68 |
| Accuracy | 0.75 |
| Precision | 0.62 |

## 🤖 Model

- **Algorithm:** Gradient Boosting Classifier
- **Train/Test Split:** Standard train_test_split (e.g., 80/20)

## 📈 Evaluation & Results

Model performance was evaluated and visualized using plots such as:
- Confusion Matrix
- (add ROC Curve / Feature Importance here if applicable)

> 📌 See the `images/` or `results/` folder for sample output plots.

## 🛠️ Tools & Libraries

- Python (Jupyter Notebook)
- pandas, numpy
- scikit-learn
- matplotlib / seaborn

## 📁 Project Structure

```
diabetes-prediction/
│
├── notebook.ipynb          # Main analysis & modeling notebook
├── data/                    # Dataset files
├── images/
        Confusion Matrix , Precision-Recall Curve , Receiver Operating Characteristic (ROC) Curve   # Output plots (confusion Precision, ROC.)
├── requirements.txt          # Project dependencies
└── README.md
```

## 🚀 How to Run

```bash
pip install -r requirements.txt
jupyter notebook notebook.ipynb
```

## 📄 License

This project is open-source and available under the MIT License.

---### Short GitHub "About" Description (one-liner)
> Machine learning model to predict diabetes in patients using the Pima Indians Diabetes dataset and Gradient Boosting.
