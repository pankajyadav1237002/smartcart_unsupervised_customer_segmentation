#  Smart Cart: Customer Segmentation & Behavioral Analytics

An end-to-end Machine Learning project focused on analyzing retail customer data to discover distinct behavioral segments using unsupervised clustering.

---

##  Project Overview
Understanding customer behavior is vital for targeted marketing, personalizing recommendations, and improving retention. This project processes a retail customer dataset, engineers insightful behavioral and demographic features, and implements an unsupervised machine learning pipeline to group customers into distinct segments.

---

##  Key Steps & Workflow

1. Data Loading & Inspection:
   - Loaded the customer dataset (2,240 rows and 22 columns).
   - Inspected data types, columns, and handled missing values (specifically utilizing median imputation for the `Income` column).

2. Feature Engineering:
   - `Age`: Derived from the customer's `Year_Birth`.
   - `Customer_Tenure_days`: Calculated length of relationship based on enrollment date (`Dt_Customer`).
   - `Total_Spending`: Aggregated expenditures across multiple product categories (Wines, Fruits, Meat, Fish, Sweets, and Gold products).
   - **`Total_Children`**: Combined `Kidhome` and `Teenhome` into a single family size metric.
   - **Categorical Mapping**: Simplified granular education levels and marital statuses into broader, cleaner categories (`Education` and `Living_With`).

3. Dimensionality Reduction & Preparation:
   - Dropped redundant raw features to prevent multicollinearity and clean up the feature space before modeling.

---

## 🛠️ Tech Stack & Libraries
* Python (Programming Language)
* Pandas & NumPy (Data Manipulation & Cleaning)
* Matplotlib & Seaborn (Exploratory Data Analysis & Visualization)
* Scikit-Learn (Clustering & Machine Learning Pipeline)
* Jupyter Notebook (Development Environment)

---

## 📂 Project Structure
```text
├── smartcart.ipynb       # Main Jupyter Notebook containing code, EDA, and preprocessing
└── README.md             # Project documentation
