# 🌸 Iris Classification using Machine Learning

## 📌 Project Overview

This project focuses on classifying Iris flowers into three species:

- Iris-setosa
- Iris-versicolor
- Iris-virginica

using Machine Learning classification algorithms based on flower measurements such as sepal length, sepal width, petal length, and petal width.

This project was completed as part of the **Alfido Tech Machine Learning Internship**.

---

## 🎯 Objective

Build a classification model capable of predicting the species of an Iris flower using its physical characteristics.

---

## 📊 Dataset Information

**Dataset Name:** Iris Classification Dataset

### Features

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

### Target Variable

- Species

### Dataset Statistics

- Total Records: 150
- Iris-setosa: 50
- Iris-versicolor: 50
- Iris-virginica: 50

The dataset is balanced and contains no missing values.

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Joblib
- Google Colab

---

## 📈 Exploratory Data Analysis (EDA)

The following analyses were performed:

- Dataset Shape Analysis
- Dataset Information Analysis
- Statistical Summary
- Missing Value Analysis
- Class Distribution Analysis
- Scatter Plot Visualization
- Pair Plot Visualization

### Key Observations

- No missing values were found.
- Dataset is balanced across all species.
- Petal Length and Petal Width are the most informative features.
- Iris-setosa is clearly separable from other species.
- Iris-versicolor and Iris-virginica show slight overlap.

---

## 🤖 Machine Learning Models Used

### 1. Logistic Regression

Used as the baseline classification model.

### 2. K-Nearest Neighbors (KNN)

Implemented using:

```python
KNeighborsClassifier(n_neighbors=5)
```

### 3. Decision Tree Classifier

Implemented using:

```python
DecisionTreeClassifier(random_state=42)
```

---

## 📊 Model Performance

| Model | Accuracy |
|---------|---------|
| Logistic Regression | 100% |
| KNN | 100% |
| Decision Tree | 100% |

---

## 📋 Evaluation Metrics

The following metrics were evaluated:

- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-Score
- Classification Report

### Logistic Regression Results

| Metric | Score |
|----------|----------|
| Accuracy | 1.00 |
| Precision | 1.00 |
| Recall | 1.00 |
| F1 Score | 1.00 |

---

## 💾 Model Saving

The final model was saved using Joblib.

```python
import joblib

joblib.dump(lr_model, "iris_model.pkl")
```

Saved Model:

```text
iris_model.pkl
```

---

## 🚀 Example Inference

```python
import joblib
import numpy as np

model = joblib.load("iris_model.pkl")

new_flower = np.array([[5.1, 3.5, 1.4, 0.2]])

prediction = model.predict(new_flower)

print("Predicted Species:", prediction[0])
```

### Sample Output

```text
Predicted Species: Iris-setosa
```

---

## 📁 Repository Structure

```text
iris-classification-ml
│
├── README.md
├── Iris_Classification_ML.ipynb
├── iris_model.pkl
└── IRIS.csv
```

---

## 🎯 Conclusion

- Successfully performed EDA and visualization.
- Built and compared multiple machine learning models.
- Achieved 100% accuracy using Logistic Regression, KNN, and Decision Tree.
- Selected Logistic Regression as the final model due to simplicity and efficiency.
- Saved the trained model using Joblib.
- Demonstrated prediction using example inference code.

---

## 👨‍💻 Author

**Tushar Patel**

B.Tech CSE (AI & ML)

Machine Learning Intern – Alfido Tech

---

⭐ If you found this project useful, consider giving this repository a star.
