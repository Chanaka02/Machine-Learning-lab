# Machine Learning Practicals

A collection of hands-on machine learning notebooks covering **supervised learning** (regression and classification) and **unsupervised learning** (K-Means and hierarchical clustering). Each notebook walks through a complete workflow: loading data, checking for missing values, preprocessing, training a model, evaluating it, and visualising the results.

All notebooks were built in **Google Colab** using Python and scikit-learn.

---

## 📂 Projects

| # | Notebook | Topic | Algorithm | Dataset |
|---|----------|-------|-----------|---------|
| 1 | `Practical_5_task_1.ipynb` | Salary Prediction | Simple Linear Regression | `Salary_dataset.xlsx` |
| 2 | `Practical_6.ipynb` | Heart Disease Prediction | Random Forest Classifier | `heart.csv` |
| 3 | `Practical_8_1.ipynb` | Income-Based Customer Clustering | K-Means Clustering | `income.csv` |
| 4 | `Customer_Segmentation__1_.ipynb` | Mall Customer Segmentation | Hierarchical (Agglomerative) Clustering | `Mall_Customers.csv` |
| 5 | `Iris_Flower_Classification__1_.ipynb` | Iris Flower Grouping | Hierarchical (Agglomerative) Clustering | `Iris.csv` |

---

## 📝 Project Details

### 1. Salary Prediction — Linear Regression
Predicts salary from years of experience.
- Scatter plot of experience vs. salary
- 80/20 train-test split
- Extracts the slope (`m`) and intercept (`b`) of the fitted line
- Plots the best-fit line against test data
- Evaluated with **MAE, MSE, RMSE and R² score**

### 2. Heart Disease Prediction — Random Forest
Classifies whether a patient has heart disease based on clinical features.
- Checks class distribution of the target column
- 80/20 train-test split
- Trains a Random Forest with 100 trees
- Evaluated with **accuracy, confusion matrix and classification report**
- Compares accuracy across different numbers of trees (10, 50, 100, 200)

### 3. Customer Clustering by Age & Income — K-Means
Groups customers based on age and income.
- Feature scaling with `StandardScaler`
- Uses the **Elbow Method (WCSS)** to choose the number of clusters
- Trains K-Means with K = 3 (`k-means++` initialisation)
- Visualises clusters with a coloured scatter plot

### 4. Mall Customer Segmentation — Hierarchical Clustering
Segments mall customers by annual income and spending score.
- Feature scaling with `StandardScaler`
- Builds a **dendrogram** using Ward linkage to decide the cluster count
- Agglomerative clustering into 5 segments
- Shows cluster sizes and mean income/spending per cluster

### 5. Iris Flower Grouping — Hierarchical Clustering
Groups iris flowers using sepal and petal measurements without using labels.
- Feature scaling with `StandardScaler`
- Truncated **dendrogram** with Ward linkage
- Agglomerative clustering into 3 groups
- Compares discovered clusters with the actual species using a **crosstab**

---

## 🛠️ Tech Stack

- **Python 3**
- **pandas**, **NumPy** — data handling
- **Matplotlib**, **Seaborn** — visualisation
- **scikit-learn** — models, preprocessing and metrics
- **SciPy** — dendrograms and linkage
- **Google Colab** — development environment

---

## 🚀 How to Run

### Option 1: Google Colab (recommended)
1. Open any notebook in [Google Colab](https://colab.research.google.com/).
2. Run the cells in order.
3. When prompted by `files.upload()`, upload the matching dataset from the table above.

### Option 2: Run locally
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/machine-learning-practicals.git
   cd machine-learning-practicals
   ```
2. Install the dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn scipy openpyxl jupyter
   ```
3. Remove or skip the `google.colab` upload cell, place the dataset in the same folder as the notebook, and run:
   ```bash
   jupyter notebook
   ```

---

## 📊 Datasets

The datasets are not included in this repository. They are publicly available on platforms such as [Kaggle](https://www.kaggle.com/):
- Salary Dataset (Years of Experience vs Salary)
- Heart Disease Dataset
- Income Dataset (Age and Income)
- Mall Customers Dataset
- Iris Dataset

---

## 📚 Concepts Covered

- Supervised vs. unsupervised learning
- Train-test splitting
- Feature scaling
- Regression metrics (MAE, MSE, RMSE, R²)
- Classification metrics (accuracy, precision, recall, F1-score, confusion matrix)
- Ensemble learning (Random Forest)
- Choosing K with the Elbow Method
- Dendrograms and Ward linkage

---

## 👤 Author

**Your Name**
- GitHub: [@your-username](https://github.com/your-username)

---

⭐ If you found this helpful, feel free to star the repository!
