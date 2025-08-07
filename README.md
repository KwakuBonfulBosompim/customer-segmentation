# 🛍 Customer Segmentation Using RFM Analysis & K-Means Clustering

## 📌 Project Overview
This project analyzes retail transaction data from an online store to segment customers based on purchasing behavior.  
Using **RFM Analysis** (Recency, Frequency, Monetary) and **K-Means Clustering**, we group customers into meaningful segments for targeted marketing, customer retention, and sales optimization.

---

## 📂 Table of Contents
- [Overview](#-project-overview)
- [Dataset](#-about-the-dataset)
- [Tools & Techniques](#-tools--techniques)
- [Methodology](#-methodology)
- [Business Impact](#-business-impact)
- [Results](#-results)
- [Next Steps](#-next-steps)

---

## 📊 About the Dataset
**Source:** UK-based online retail dataset containing transactions from `01/12/2010` to `09/12/2011`.

- **Columns:** InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country  
- **Details:** Company sells unique all-occasion gifts. Many customers are wholesalers.  
- **Rows:** 541,909 transactions.

---

## 🛠 Tools & Techniques
- **Language:** Python  
- **IDE:** Google Colab  
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `scipy`  
- **Methods:**
  - RFM Feature Engineering
  - Data Cleaning & Outlier Removal
  - StandardScaler for normalization
  - K-Means Clustering
  - Silhouette Score & Elbow Method for cluster evaluation
  - Alternative models (DBSCAN, Agglomerative Clustering, GMM)

---

## 🔍 Methodology
1. **Data Cleaning**
   - Removed missing `CustomerID` values.
   - Removed returns & invalid transactions (negative Quantity/UnitPrice).
2. **Feature Engineering**
   - Created Monetary (`Amount`), Frequency, and Recency features.
3. **Outlier Removal**
   - Applied Z-score filtering to remove extreme values.
4. **Scaling**
   - Standardized features using `StandardScaler`.
5. **Clustering**
   - Applied **K-Means** and determined optimal `k` using Elbow & Silhouette methods.
   - Compared results with DBSCAN & Agglomerative clustering.
6. **Interpretation**
   - Segmented customers into groups: High-value frequent buyers, one-time buyers, low-spenders, etc.

---

## 📈 Business Impact
Customer segmentation allows for:
- 🎯 **Personalized marketing campaigns**  
- 🎁 **Loyalty program targeting** for frequent/high-spending customers  
- 🔄 **Retargeting inactive customers**  
- 📊 **Customer Lifetime Value (CLV) estimation**  
- 🧠 **Better promotion & inventory planning**

---

## 🏆 Results
- Optimal clusters identified using **K-Means**.  
- Clear behavioral patterns across customer groups.
- Exported segmentation results to CSV for business use.

---

## 🚀 Next Steps
- Integrate Recency feature for complete RFM analysis.
- Implement real-time clustering with streaming transaction data.
- Build dashboards for business teams to monitor segments.
- Test supervised models to predict customer movement between segments.

---

## 📬 Author
**Kwaku Bonful Bosompim**  
📍 Berlin, Germany  
🔗 [GitHub Profile](https://github.com/KwakuBonfulBosompim) | [LinkedIn](#)

