# Red Wine Quality Prediction 🍷

## Overview
This project analyzes the "Red Wine Quality" dataset to determine if physicochemical properties (such as alcohol level, acidity, and pH) can effectively predict the quality of wine. The notebook explores data correlations, visualizes trends, and implements machine learning models to classify and predict wine quality scores.

## 📊 Dataset
The dataset contains various physicochemical tests for red variants of the Portuguese "Vinho Verde" wine.
* **Input variables:** fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulphates, alcohol.
* **Target variable:** quality (score between 0 and 10).

## 🚀 Key Features & Methodology

### 1. Exploratory Data Analysis (EDA)
* **Data Inspection:** Reviewing dataset structure, checking for missing values, and statistical summary.
* **Correlation Analysis:** Generating correlation matrices to identify relationships between variables (e.g., *Alcohol* vs. *Quality*).
* **Visualization:** Scatter plots to visualize the spread of quality scores against alcohol content.

### 2. Data Preprocessing
* **Filtering:** Focused analysis on wines with a quality rating greater than 4 (excluding table wines).
* **Splitting:** Division of data into training (80%) and testing (20%) sets.

### 3. Machine Learning Models
* **Linear Regression:**
    * **Focus:** Investigated the specific relationship between **Alcohol level** and **Quality**.
    * **Result:** The model showed a weak direct linear relationship, suggesting alcohol content alone is not a definitive predictor of quality.
* **Decision Tree Classifier:**
    * **Focus:** Utilized **all 11 physicochemical features** to predict quality.
    * **Result:** Achieved significantly higher accuracy on the training set compared to the linear model, capturing non-linear relationships between the features.

### 4. Prediction Interface
* Includes an interactive section allowing users to input a specific **Alcohol level**.
* The model predicts the wine quality by combining the user input with average values for the other physicochemical characteristics.

## 🛠️ Technologies Used
* **Python 3**
* **Pandas** (Data Manipulation)
* **NumPy** (Numerical Operations)
* **Matplotlib** (Data Visualization)
* **Scikit-Learn** (Machine Learning Models)

## 📉 Results Summary
The analysis highlights that while alcohol content has some correlation with quality, it is not the sole driver. A Decision Tree model incorporating all chemical properties yields better predictive power than a simple Linear Regression based on alcohol alone.

## 💻 How to Run
1.  Clone the repository.
2.  Ensure the `winequality-red.csv` dataset is available.
3.  Install dependencies:
    ```bash
    pip install pandas numpy matplotlib scikit-learn
    ```
4.  Run the Jupyter Notebook:
    ```bash
    jupyter notebook 20251106_Exercise_2_Redwine.ipynb
    ```
