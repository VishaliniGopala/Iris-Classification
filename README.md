# Iris Classification Project

## Objective

Build a machine learning classification model to predict Iris flower species using classic flower measurements.

Target Variable:

Species

Features Used:

- SepalLengthCm
- SepalWidthCm
- PetalLengthCm
- PetalWidthCm

---

## Dataset

Iris Classification Dataset

---

## Project Workflow

1. Load Dataset
2. Exploratory Data Analysis (EDA)
3. Data Cleaning
4. Feature Encoding
5. Visualization & Class Separability
6. Train/Test Split
7. Model Training
8. Model Evaluation
9. Model Comparison
10. Model Saving
11. Prediction Example

---

## Algorithms Compared

- Logistic Regression
- k-Nearest Neighbors (k-NN)
- Decision Tree Classifier

---

## Exploratory Data Analysis

Performed:

- head()
- info()
- describe()
- missing value analysis

Visualizations:

- Scatter Plot
- Histogram
- Boxplot
- Pairplot

---

## Evaluation Metrics

- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-Score

---

## Package Versions

Python == 3.10

pandas == 2.2.3

numpy == 2.2.5

matplotlib == 3.10.1

seaborn == 0.13.2

scikit-learn == 1.6.1

joblib == 1.5.0

---

## Installation Commands

Create virtual environment (optional):

```bash
python -m venv venv
```

Activate environment.

Windows:

```bash
venv\Scripts\activate
```

Linux / Mac:

```bash
source venv/bin/activate
```

Install packages:

```bash
pip install pandas==2.2.3 numpy==2.2.5 matplotlib==3.10.1 seaborn==0.13.2 scikit-learn==1.6.1 joblib==1.5.0
```

Alternative:

```bash
pip install -r requirements.txt
```

---

## Exact Commands to Reproduce Results

Launch Jupyter:

```bash
jupyter notebook
```

OR

```bash
jupyter lab
```

Open:

```plaintext
Iris_Classification.ipynb
```

Run all notebook cells sequentially.

---

## Save Best Model

```python
joblib.dump(best_model,'iris_model.joblib')
```

---

## Example Prediction / Inference

```python
import joblib
import numpy as np

model=joblib.load('iris_model.joblib')

sample=np.array([[5.1,3.5,1.4,0.2]])

prediction=model.predict(sample)

print(prediction)
```

Decode prediction:

```python
species=encoder.inverse_transform(prediction)

print(species[0])
```

Example Output:

```plaintext
Iris-setosa
```

---

## Project Files

```plaintext
Iris_Classification.ipynb
iris_model.joblib
README.md
Iris.csv
requirements.txt
```

---

## Expected Result

The trained model predicts the Iris flower species from sepal and petal measurements.