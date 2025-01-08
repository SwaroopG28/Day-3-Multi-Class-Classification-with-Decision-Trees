## **Day 3: Multi-Class Classification with Decision Trees**

### 📄 **Project Overview**
This project focuses on building a **Decision Tree Classifier** to segment customers into distinct categories based on their shopping behavior. The dataset used is the **Mall Customer Segmentation Dataset** available on Kaggle.

**Dataset Link:** [Mall Customer Segmentation](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

---

### 🎯 **Objective**
- Understand customer segments using **Decision Tree Classifier**.
- Perform **feature preprocessing** and **exploratory data analysis (EDA)**.
- Optimize model performance using **GridSearchCV**.
- Evaluate the model with key metrics such as **Accuracy**, **Precision**, **Recall**, and **F1-Score**.
- Visualize the **Decision Tree** and feature importances.

---

### 📊 **Dataset Description**
- **CustomerID:** Unique identifier for each customer (removed during preprocessing).
- **Gender:** Categorical feature (encoded numerically).
- **Age:** Age of the customer.
- **Annual Income (k$):** Customer's annual income.
- **Spending Score (1-100):** Customer's spending behavior score.

**Target Variable (Generated):**
- Categories derived using **K-Means Clustering:**
   - Low Spend
   - Medium Spend
   - High Spend

---

### ⚙️ **Technologies Used**
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- K-Means Clustering
- Decision Tree Classifier
- GridSearchCV
- Pickle (Model Saving)

---

### 🛠️ **Steps Performed**

#### **1. Data Preprocessing**
- Removed `CustomerID` (non-informative feature).
- Encoded `Gender` using **LabelEncoder**.
- Standardized numerical features (`Age`, `Annual Income`, `Spending Score`) using **StandardScaler**.
- Created target variable using **K-Means Clustering** with 3 segments.

#### **2. Exploratory Data Analysis (EDA)**
- Visualized class distribution.
- Plotted correlation heatmaps.
- Scatter plot for `Annual Income` vs `Spending Score` to observe clusters.

#### **3. Model Training**
- Split data into **80% training** and **20% testing**.
- Initialized **Decision Tree Classifier**.
- Performed **GridSearchCV** for hyperparameter tuning (`max_depth`, `min_samples_split`, `criterion`).
- Selected the best model.

#### **4. Model Evaluation**
- Evaluated the model using:
   - **Accuracy**
   - **Precision**
   - **Recall**
   - **F1-Score**
- Displayed **Confusion Matrix**.
- Plotted the **Decision Tree Visualization**.

