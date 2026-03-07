<!DOCTYPE html>
<html lang="en">
<head>

</head>

<body>

<div class="container">

<h1>Heart Disease Prediction using Machine Learning</h1>

<p>
This project builds a machine learning model to predict the risk of heart disease
using healthcare data. The goal is to analyze key health indicators and apply
machine learning techniques to assist in early risk detection.
</p>

<h2>Project Objectives</h2>

<ul>
<li>Analyze healthcare indicators related to heart disease</li>
<li>Build a machine learning model for risk prediction</li>
<li>Visualize health patterns in the dataset</li>
<li>Evaluate model performance using classification metrics</li>
</ul>

<h2>Dataset</h2>

<p>
The dataset used in this project is the <b>CDC Heart Disease Indicators Dataset (2022)</b>.
It contains multiple health indicators related to lifestyle and medical conditions.
</p>

<h3>Target Variable</h3>

<pre>HadHeartAttack</pre>

<p>This variable indicates whether the patient has experienced a heart attack.</p>

<h2>Machine Learning Workflow</h2>

<pre>
1. Data Loading
2. Data Cleaning
3. Exploratory Data Analysis
4. Feature Encoding
5. Feature Scaling
6. Dimensionality Reduction (PCA)
7. Data Visualization (t-SNE)
8. Model Training (SVM)
9. Hyperparameter Optimization
10. Model Evaluation
</pre>

<h2>Data Preprocessing</h2>

<p>
The dataset was filtered to include only female patients to analyze
heart disease risk specifically for women.
</p>

<p>
Several features were removed to reduce redundancy and potential bias.
</p>

<table>
<tr>
<th>Feature</th>
<th>Reason for Removal</th>
</tr>

<tr>
<td>State</td>
<td>Not relevant for prediction</td>
</tr>

<tr>
<td>Sex</td>
<td>Dataset already filtered</td>
</tr>

<tr>
<td>HeightInMeters</td>
<td>Redundant due to BMI</td>
</tr>

<tr>
<td>WeightInKilograms</td>
<td>Redundant due to BMI</td>
</tr>

<tr>
<td>RaceEthnicityCategory</td>
<td>Removed to avoid bias</td>
</tr>

</table>

<h2>Feature Encoding</h2>

<p>
Categorical variables were converted into numerical values using
One-Hot Encoding.
</p>

<pre>
pd.get_dummies()
</pre>

<h2>Feature Scaling</h2>

<p>
Feature values were standardized using StandardScaler to ensure all variables
have similar ranges.
</p>

<pre>
StandardScaler()
</pre>

<h2>Dimensionality Reduction</h2>

<h3>Principal Component Analysis (PCA)</h3>

<p>
PCA was applied to reduce the number of features while preserving
important information in the dataset.
</p>

<p>Benefits include:</p>

<ul>
<li>Reducing noise</li>
<li>Improving model performance</li>
<li>Reducing overfitting</li>
</ul>

<h2>Visualization</h2>

<h3>t-SNE</h3>

<p>
t-SNE was used to visualize high-dimensional healthcare data
in two dimensions. This helps identify clusters and patterns
within the dataset.
</p>

<h2>Machine Learning Model</h2>

<p>
The primary model used in this project is the
<b>Support Vector Machine (SVM)</b>.
</p>

<p>
SVM identifies the optimal boundary that separates
patients with heart disease risk from those without risk.
</p>

<h2>Hyperparameter Optimization</h2>

<p>
Model parameters were optimized using:
</p>

<pre>
HalvingGridSearchCV
</pre>

<p>
This method efficiently searches for the best parameter combinations
to improve prediction accuracy.
</p>

<h2>Model Evaluation</h2>

<p>The model performance was evaluated using:</p>

<ul>
<li>Confusion Matrix</li>
<li>Classification Report</li>
</ul>

<table>

<tr>
<th>Metric</th>
<th>Description</th>
</tr>

<tr>
<td>Precision</td>
<td>Correct positive predictions</td>
</tr>

<tr>
<td>Recall</td>
<td>Ability to detect heart disease cases</td>
</tr>

<tr>
<td>F1 Score</td>
<td>Balance between precision and recall</td>
</tr>

<tr>
<td>Accuracy</td>
<td>Overall prediction correctness</td>
</tr>

</table>

<h2>Technologies Used</h2>

<ul>
<li>Python</li>
<li>Pandas</li>
<li>NumPy</li>
<li>Scikit-learn</li>
<li>Matplotlib</li>
<li>Seaborn</li>
<li>Jupyter Notebook</li>
</ul>


<div class="footer">

<p>
Muhammed Raihan<br>
Computer Science Graduate – Artificial Intelligence & Big Data
</p>

</div>

</div>

</body>
</html>
