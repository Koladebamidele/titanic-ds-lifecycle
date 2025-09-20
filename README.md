# Titanic Dataset - Data Science Lifecycle Project

This project walks through the **entire Data Science lifecycle** using the classic [Titanic dataset](https://www.kaggle.com/c/titanic). The goal is to apply the major stages of a data science project:

1. **Data Analysis (EDA)**
2. **Feature Engineering**
3. **Feature Selection**
4. **Model Building**

---

## 📊 1. Data Analysis (EDA)

The first step is to **explore and understand the dataset**.

* Performed **statistical analysis** of numerical and categorical variables.
* Created **visualizations** (histograms, scatter plots, heatmaps, bar charts).
* Identified **patterns, correlations, missing values, and outliers**.
* Summarized key insights that guide further preprocessing.

---

## 🛠 2. Feature Engineering

Based on the findings from EDA, preprocessing was applied:

1. **Handling missing values** (e.g., imputing with mean/median/mode).
2. **Encoding categorical columns** (e.g., one-hot encoding, label encoding).
3. **Scaling/normalizing** numerical features.

---

## 🛠 2.1 Feature Engineering (Train/Test Split)

As a best practice, preprocessing was repeated after splitting the dataset to avoid data leakage:

1. Split into **train** and **test** sets.
2. Applied the same preprocessing pipeline:

   * Filling missing values
   * Encoding categorical features
   * Standardizing numerical features

---

## 🎯 3. Feature Selection

To improve model performance and reduce complexity:

* Performed **correlation analysis**.
* Applied **statistical methods** and **algorithmic approaches** such as:

  * Dropping Constant Features (VarianceThreshold)
  * Information Gain (mutual_info_classif)
  * Chi-square
* Removed irrelevant/redundant features.

---

## 🤖 4. Model Building

Different machine learning models were trained and evaluated:

* Algorithms used:

  * Logistic Regression
  * Naive Bayes
  * K-Nearest Neighbors (KNN)
  * Decision Tree
  * Random Forest

* **Steps followed:**

  1. Split dataset into training, validation, and testing sets.
  2. Trained models with hyperparameter tuning.
  3. Evaluated using metrics:

     * Accuracy
     * Precision & Recall
     * F1-score
     * AUC (for classification)

---

## 📈 Results

* The models were compared to determine which algorithm performed best.
* Key insights from evaluation:

  * Which features had the most predictive power.
  * Trade-offs between model interpretability and accuracy.

---

## 📂 Project Structure

```
├── data/                 # Titanic dataset (CSV)
├── notebooks/            # Jupyter notebooks for EDA, preprocessing, modeling
├── README.md             # Project documentation
└── requirements.txt      # Dependencies
```

---

## 🚀 How to Run

1. Clone this repository

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebooks in the `notebooks/` folder to reproduce analysis and results.

---

## 🔮 Future Improvements

* Experiment with deep learning models.
* Implement cross-validation for more robust evaluation.
* Deploy the best model with a simple API or web app.

---

## 📌 References

* [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic)
* [Scikit-learn Documentation](https://scikit-learn.org/stable/)
* [Pandas Documentation](https://pandas.pydata.org/)

---

👨‍💻 Author: *Kolade Bamidele*