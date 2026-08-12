# Customer Segmentation Analysis using RFM and K-Means

**Name:** Aparaajetha Suvarnam
**Internship:** Oasis Infobyte (OIBSIP)
**Track:** Data Analytics
**Task:** Task 2 – Customer Segmentation Analysis

---

## 📌 Project Overview

This project focuses on performing **Customer Segmentation Analysis** on an e-commerce retail dataset.

The objective is to group customers into meaningful segments based on their purchasing behaviour. **RFM (Recency, Frequency, Monetary) analysis** is used to identify important customer characteristics, followed by the **K-Means clustering algorithm** to create distinct customer segments.

The resulting segments can help businesses develop targeted marketing strategies, improve customer retention, and focus resources on high-value customers.

---

## 🎯 Objective

The main objectives of this project are:

* Analyze customer purchasing behaviour.
* Calculate Recency, Frequency, and Monetary (RFM) metrics.
* Identify important behavioural features for customer segmentation.
* Standardize the RFM features before clustering.
* Determine the optimal number of clusters using the Elbow Method.
* Apply K-Means clustering.
* Visualize and profile the resulting customer segments.
* Develop actionable marketing recommendations for each segment.

---

## 📊 Dataset

**Dataset:** Online Retail Dataset

The dataset contains transaction-level information from an e-commerce retail business.

### Main Features

| Feature       | Description                       |
| ------------- | --------------------------------- |
| `InvoiceNo`   | Unique invoice/transaction number |
| `StockCode`   | Product code                      |
| `Description` | Product description               |
| `Quantity`    | Number of units purchased         |
| `InvoiceDate` | Date and time of transaction      |
| `UnitPrice`   | Price per unit                    |
| `CustomerID`  | Unique customer identifier        |
| `Country`     | Customer's country                |

A `TotalAmount` feature was created during the analysis:

**TotalAmount = Quantity × UnitPrice**

---

## 🛠️ Technologies Used

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Scikit-learn** – Standardization and K-Means clustering
* **Google Colab** – Development environment
* **Jupyter Notebook** – Project notebook format

---

## 🔄 Project Workflow

The analysis follows these steps:

1. Load the Online Retail dataset.
2. Inspect the dataset structure.
3. Check missing values and duplicate records.
4. Clean invalid and incomplete transactions.
5. Calculate total transaction value.
6. Perform customer-level descriptive analysis.
7. Perform RFM analysis.
8. Select Recency, Frequency, and Monetary as clustering features.
9. Standardize the RFM features using `StandardScaler`.
10. Use the Elbow Method to determine the suitable number of clusters.
11. Apply K-Means clustering.
12. Profile the resulting customer segments.
13. Visualize the customer clusters.
14. Analyze the number of customers in each segment.
15. Develop actionable marketing recommendations.

---

## 📐 RFM Analysis

RFM analysis was used to represent customer purchasing behaviour through three metrics.

### Recency

Measures how recently a customer made a purchase.

* Lower Recency → More recent purchase
* Higher Recency → Customer has not purchased recently

### Frequency

Measures how frequently a customer makes purchases.

* Higher Frequency → More frequent purchases
* Lower Frequency → Less frequent purchases

### Monetary

Measures the total amount spent by a customer.

* Higher Monetary → Higher customer value
* Lower Monetary → Lower customer value

The three RFM features were used as the input features for customer clustering.

---

## ⚙️ Data Standardization

Recency, Frequency, and Monetary values have different numerical scales.

Therefore, **StandardScaler** from Scikit-learn was applied before K-Means clustering so that the features could be compared on a common scale.

---

## 📈 Elbow Method

The **Elbow Method** was used to determine a suitable number of customer clusters.

Different values of K were evaluated using their inertia values. Based on the resulting elbow curve, **K = 4** was selected for the final K-Means model.

---

## 🤖 K-Means Clustering

The K-Means algorithm was applied to the standardized RFM features.

### Clustering Configuration

* **Number of clusters:** 4
* **Random state:** 42
* **Number of initializations:** 10

Each customer was assigned to one of the four clusters based on similarities in their purchasing behaviour.

---

## 👥 Customer Segments

The four clusters were interpreted using their RFM characteristics.

### Cluster 0 – Regular Customers

These customers show moderate purchasing activity and spending.

**Recommended strategies:**

* Encourage repeat purchases.
* Provide loyalty rewards.
* Use personalized product recommendations.
* Apply cross-selling strategies.

---

### Cluster 1 – At-Risk / Inactive Customers

These customers have relatively high Recency and comparatively lower purchasing activity.

**Recommended strategies:**

* Launch customer win-back campaigns.
* Send personalized offers.
* Provide limited-time promotions.
* Encourage customers to return.

---

### Cluster 2 – High-Value Loyal Customers

These customers have very recent purchases, extremely high purchase frequency, and very high monetary contribution.

**Recommended strategies:**

* Provide VIP loyalty benefits.
* Offer exclusive rewards.
* Give early access to new products.
* Focus strongly on customer retention.

---

### Cluster 3 – Loyal High-Spending Customers

These customers purchase frequently and recently and contribute substantial revenue.

**Recommended strategies:**

* Provide premium loyalty rewards.
* Offer personalized promotions.
* Encourage repeat purchases.
* Use upselling and cross-selling opportunities.

---

## 📊 Visualizations

The project includes the following visualizations:

### 1. Elbow Method

Used to determine the suitable number of clusters for K-Means.

### 2. Frequency vs Monetary Scatter Plot

Shows the relationship between purchase frequency and customer spending across the different clusters.

### 3. Recency vs Monetary Scatter Plot

Shows the relationship between how recently customers purchased and their monetary contribution.

### 4. Number of Customers per Cluster

A bar chart showing the distribution of customers across the four customer segments.

### 5. Monetary Value Distribution

A boxplot was used to analyze differences in monetary contribution across customer clusters and reveal variations that may not be apparent from average values alone.

---

## 💡 Business Insights

The analysis demonstrates that customers have significantly different purchasing behaviours.

High-value customers who purchase frequently and recently represent an important segment for customer retention.

At-risk customers with high Recency values should be targeted with re-engagement campaigns, while regular customers can be encouraged to increase their purchase frequency through loyalty programs and personalized recommendations.

---

## 🚀 Business Recommendations

Based on the customer segmentation analysis, the following actions are recommended:

### 1. Retain High-Value Customers

Use VIP programs, exclusive benefits, personalized experiences, and early access to products to improve retention.

### 2. Re-engage At-Risk Customers

Use targeted win-back campaigns, personalized offers, reminders, and limited-time promotions to encourage inactive customers to return.

### 3. Increase Customer Lifetime Value

Encourage regular customers to purchase more frequently through loyalty programs, personalized recommendations, cross-selling, and upselling.

### 4. Use Segment-Specific Marketing

Avoid using the same marketing strategy for every customer. Customize campaigns according to the characteristics of each customer segment.

### 5. Prioritize Valuable Customers

Focus retention efforts on customers with high purchasing frequency, recent activity, and high monetary contribution.

---

## 📁 Project Structure

```text
DataAnalytics-L1-CustomerSegmentation/
│
├── CustomerSegmentation_Task2.ipynb
├── README.md
└── screenshots/
```

---

## ▶️ How to Run the Project

### Using Google Colab

1. Open `CustomerSegmentation_Task2.ipynb` in Google Colab.
2. Upload the Online Retail dataset.
3. Make sure the dataset path matches the path used in the notebook.
4. Run the notebook cells sequentially from beginning to end.
5. Review the generated statistics, visualizations, customer segments, and recommendations.

### Using Jupyter Notebook

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

Then launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `CustomerSegmentation_Task2.ipynb` and run the cells sequentially.

---

## 📌 Conclusion

The Customer Segmentation Analysis successfully applies **RFM analysis and K-Means clustering** to identify distinct customer groups based on purchasing behaviour.

The analysis identified four customer segments with different levels of recency, purchase frequency, and monetary contribution.

These segments provide a practical foundation for targeted marketing, customer retention, and better allocation of marketing resources.

By understanding the differences between regular, at-risk, and high-value customers, businesses can develop more personalized and effective marketing strategies.

---

## 👩‍💻 Author

**Aparaajetha Suvarnam**

Data Analytics Intern – Oasis Infobyte (OIBSIP)

**Task:** Customer Segmentation Analysis
**Track:** Data Analytics
