# decisional-statistic
[link presentation] {https://gamma.app/docs/Analyse-des-Ventes-en-Ligne-wxkhw0jkhjhqens}

# 📊 Customer Segmentation & Sales Analysis Project

This project focuses on exploratory data analysis, statistical modeling, and customer segmentation using a retail sales dataset. The objective is to better understand customer purchasing behavior and support business decision-making through data-driven insights.

---

## 🎯 Objectives

* Clean and prepare transactional sales data
* Analyze sales trends and customer behavior
* Apply statistical methods (ANOVA, regression analysis)
* Perform customer segmentation using the RFM model and K-Means clustering
* Generate business recommendations to improve marketing performance and customer retention

---

## 📂 Dataset Description

The dataset contains retail transaction data with variables such as:

* CustomerID
* InvoiceNo
* Quantity
* UnitPrice
* Country
* InvoiceDate
* Product information

Additional variables were created during preprocessing:

* `TotalPrice = Quantity × UnitPrice`
* RFM indicators:

  * **Recency**
  * **Frequency**
  * **Monetary (MontantTotal)**

---

## 🧹 Data Cleaning

Main preprocessing steps included:

* Removing canceled transactions
* Handling missing values
* Keeping missing `CustomerID` values for global revenue analysis
* Removing missing `CustomerID` rows for clustering and customer-level analysis
* Creating derived variables such as `TotalPrice`

---

## 📊 Exploratory Data Analysis (EDA)

The analysis included:

* Sales distribution analysis
* Time-series visualization of sales trends
* Boxplots and histograms
* Analysis of categorical variables with pie charts
* Weekly and seasonal sales behavior

Key findings:

* Sales patterns show biweekly peaks
* December has the highest sales activity
* Sundays and holidays correspond to lower sales volumes

---

## 📈 Statistical Analysis

### ANOVA

Used to compare average order amounts across countries.

Result:

* Significant differences between countries
* Very low p-value (< 0.05)

### Regression Analysis

A regression model was built to identify variables influencing sales.

Main insights:

* `Quantity` and `UnitPrice` strongly impact sales
* `DayOfWeek` has no significant effect

---

## 🤖 Customer Segmentation (RFM + K-Means)

### RFM Model

Customers were segmented using:

* **Recency**
* **Frequency**
* **Monetary Value**

### Standardization

Variables were standardized using **Z-score normalization** before clustering.

### K-Means Clustering

The optimal number of clusters was selected using the **Elbow Method**.

Identified segments:

* VIP customers
* Active high-value customers
* Regular customers
* Inactive customers

---

## 💡 Business Recommendations

* Retain VIP customers with loyalty programs
* Convert active high-value customers into VIPs
* Launch targeted campaigns around payday periods
* Reactivate inactive customers with personalized promotions

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

## 📌 Conclusion

This project demonstrates how statistical analysis and machine learning techniques can support customer understanding and business strategy. The combination of RFM segmentation and clustering provides actionable insights for marketing and sales optimization.
