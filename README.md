#  E-commerce Analysis

This project applies the RFM (Recency, Frequency, Monetary) framework to segment customers of a UK-based online retailer, based on transaction data from December 1, 2010, to December 9, 2011. By engineering key features and leveraging clustering algorithms, raw data is transformed into actionable customer profiles.

The objective is to enhance marketing effectiveness and boost sales by identifying key customer segments and understanding their purchasing behavior. This segmentation uncovers distinct profiles that provide valuable insights for targeted strategies and improved customer retention.

---

##  Project Workflow

### 1. Data Cleaning & Preprocessing
- Removed missing values and duplicates.
- Corrected stock codes and handled cancelled transactions.
- Filtered out transactions with zero unit prices.
- Created a new `TotalPrice` column.

### 2. Feature Engineering
Classic RFM metrics were combined with additional features to capture customer behavior in depth:

- **Recency**: Days since last purchase.
- **Total_Transactions**: Number of purchases made.
- **Total_Products_Purchased**: Quantity of items bought.
- **Total_Spend**: Total amount spent.
- **Average_Transaction_Value**
- **Unique_Products_Purchased**
- **Cancellation_Frequency** and **Cancellation_Rate**
- **Monthly_Spending_Mean** and **Monthly_Spending_Std**

### 3. Exploratory Data Analysis
- Visualized distributions and correlations.
- Analyzed purchasing and cancellation patterns.

### 4. Clustering & Segmentation
- Scaled features.
- Determined optimal cluster count using Elbow method and Silhouette score.
- Applied KMeans on RFM features.
- Incorporated churn analysis by flagging customers inactive for over 180 days.

---


The cleaned and enriched datasets are prepared for further applications, such as building dashboards or developing churn prediction models.


---

## Dashboard

![Image](https://github.com/user-attachments/assets/5934fbc3-1191-49da-8153-8d8aeaed0ae3)

---

##  Dataset

- Source: [Kaggle – E-commerce Data by Carrie1](https://www.kaggle.com/datasets/carrie1/ecommerce-data)
