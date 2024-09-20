# E-commerce Customers Segmentation
## 📊 Dataset Overview:
This project involves analyzing and segmenting customers in an e-commerce environment using data from five interrelated tables. The goal is to understand customer behaviors, transactions, and merchant activity to create meaningful customer segments.

## Dataset Description:
The dataset includes the following tables:

### Customers Table:
**customer_id:** Unique identifier for each customer.

**join_date:** The date the customer joined the platform.
**city_id:** Identifier for the customer's city.
**gender_id:** Identifier for the customer's gender.

### Genders Table:
**gender_id:** Unique identifier for each gender.
**gender_name:** The gender (e.g., male, female).

### Cities Table:
**city_id:** Unique identifier for each city.
**city_name:** The name of the city.

### Transactions Table:
**transaction_id:** Unique identifier for each transaction.
**customer_id:** The customer who performed the transaction.
**transaction_date:** The date the transaction was recorded.
**transaction_status:** Status of the transaction (e.g., claimed, burnt).
**coupon_name:** Name of the coupon used in the transaction.
**burn_date:** The date the coupon was burnt.
**branch_id:** Identifier for the branch where the coupon was used.

### Branches Table:
**branch_id:** Unique identifier for each branch.
**merchant_id:** Identifier for the merchant who owns the branch.

### Merchants Table:
**merchant_id:** Unique identifier for each merchant.
**merchant_name:** Name of the merchant.

## 🏗️ Project Structure:
### 📥 Import Libraries and Load Dataset:

The dataset is loaded, and necessary libraries for data manipulation and visualization are imported, including:
pandas, numpy for data handling.
matplotlib, seaborn for visualization.
sklearn for machine learning models.

### 🛠️ Data Preprocessing:
Handling Missing Values: Missing data is handled using imputation techniques where necessary.
Feature Encoding: Categorical variables such as gender, city, and merchant names are encoded for model training.
Feature Scaling: Numerical features are normalized to ensure they are on a comparable scale.
Merging Tables: All five tables are merged to create a single unified dataset for analysis.

### 🔍 Exploratory Data Analysis (EDA):
**Histograms & Bar Plots:** To visualize customer and transaction distributions.
**Heatmaps:** Used to explore relationships between different features.
#### Questions Answered:
How are customer transactions distributed across cities and branches?
What is the distribution of transactions across merchants?
How do gender and city influence customer activity?

### 🧠 Clustering and Segmentation:
#### Several clustering algorithms are applied to segment customers, including:
**K-Means Clustering:** For customer segmentation based on transaction data.
**DBSCAN & Agglomerative Clustering:** Alternative methods for clustering, evaluated using silhouette scores.
Model Evaluation:
**Silhouette Scores:** Used to evaluate the quality of clustering for each model.
**Centroid Analysis:** Visualizations of cluster centroids in 2D and 3D PCA plots.

### 📊 Visualizing the Clusters:
PCA (Principal Component Analysis) is used to reduce dimensionality and visualize clusters in 2D and 3D.
Bar plots and scatter plots are used to interpret the segments and draw insights about customer behaviors.

### 🚀 Further Steps:
Cluster Profiling: Insights are drawn from the clusters to develop profiles of typical customer groups.
Recommendations: Suggested improvements for marketing and merchant strategies based on customer segments.
### 📝 Instructions for Running the Project:
**Clone the Repository:**
```bash
git clone [https://github.com/your-username/ecommerce-customer-segmentation.git](https://github.com/Mohammed-Mahmoud-Elsayed-Ahmed-MMES/Graduation-Project-Part-2-MLSC-Data-Science-Machine-Learning-Course.git)
```

**Install the Required Libraries:**
Run the following command to install dependencies:
```bash
pip install -r requirements.txt
```
Run the Jupyter Notebook:

**Start the notebook:**
```bash
jupyter notebook E-commerce_Graduation_Project_part2.ipynb
```

**Extract Dataset:** From the E-commerce_data.

### 🧠 Conclusion:
This project offers valuable insights into customer segmentation in an e-commerce context. By applying clustering algorithms such as K-Means, DBSCAN, and Agglomerative Clustering, we have segmented the customers into meaningful groups that could help drive personalized marketing strategies and optimize business decisions.
