# Red Wine Quality Prediction 🍷📈

## 📌 Overview
This project explores the relationship between the chemical properties of red wine—specifically alcohol content—and its quality rating. Using the **Red Wine Quality** dataset, the goal is to build a linear regression model that predicts a wine's quality score, focusing on wines that are rated above "Table Wine" standards (quality > 4).

## 🚀 Key Steps & Methodology
1. **Data Loading & Inspection:**
   - Loaded the dataset and examined its structure using `describe()` and `info()`.
   - Checked for missing data to ensure data integrity.
2. **Exploratory Data Analysis (EDA):**
   - Analyzed correlations between different features.
   - Visualized the relationship between `alcohol` and `quality` using scatter plots.
3. **Data Filtering:**
   - Filtered out lower-quality wines (`quality <= 4`) to focus the model on higher-grade wines where quality variance is more significant for selling purposes.
4. **Modeling:**
   - **Simple Linear Regression:** Built a model using `alcohol` as the primary predictor.
   - **Multiple Linear Regression:** Expanded the model to include all available chemical features (e.g., acidity, sugar, chlorides) for a more robust prediction.
5. **Prediction:**
   - Created an interactive script to predict wine quality based on a user-inputted alcohol level while keeping other chemical properties at their average values.

## 📊 Results
- The initial analysis showed a correlation between alcohol content and quality.
- Filtering the dataset to exclude low-quality wines refined the correlation analysis.
- The final model allows for predicting the quality score of a wine given specific chemical inputs.

## 🛠️ Technologies Used
- **Python**
- **Pandas** (Data Manipulation)
- **Matplotlib** (Data Visualization)
- **Scikit-Learn** (Machine Learning: `LinearRegression`, `train_test_split`)

## 💻 How to Run
1. Open the notebook in a Jupyter environment or Google Colab.
2. Ensure the red wine dataset is available in the expected path (or update the load path).
3. Run the cells sequentially to process the data, train the model, and see the predictions.
4. (Optional) Use the interactive cell at the end to input an alcohol level and get a predicted quality score.
