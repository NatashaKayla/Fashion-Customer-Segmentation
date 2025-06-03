# 👗 Fashion Customer Segmentation - EDA & Clustering Modeling

This project focuses on analyzing fashion customer behavior and purchasing patterns to segment customers based on their preferences and transaction characteristics. It includes detailed exploratory data analysis and applies clustering techniques to uncover actionable customer groups for targeted marketing and personalization strategies.

---

## 🎯 Main Objectives

* Explore customer demographics and purchase behaviors
* Analyze patterns in product categories, payment preferences, and seasonality
* Visualize the distribution of customer features and purchasing metrics
* Apply clustering to group customers based on behavioral traits
* Identify insights that inform marketing and recommendation systems

---

## 🧾 Dataset Description

The dataset includes detailed customer and transactional information relevant to fashion retail. Key features include:

### 🧍 Demographic Information

* **Customer ID** – Unique identifier (not used in modeling)
* **Birth Date** – Used to derive age
* **Gender** – Customer gender
* **Location** – Region/city of residence

### 🛍️ Product & Purchase Details

* **Item Purchased**, **Category**, **Size**, **Color**, **Season** – Product-specific attributes
* **Purchase Amount (USD)** – Total transaction value
* **Review Rating** – Customer satisfaction score

### 💳 Customer Behavior & Preferences

* **Previous Purchases** – Number of past purchases
* **Frequency of Purchases** – Indicates shopping regularity
* **Subscription Status** – Whether subscribed to marketing/newsletter
* **Preferred Payment Method** – Typical method used by the customer

### 💸 Payment & Promotions

* **Payment Method** – Payment used in a given transaction
* **Discount Applied** – Boolean indicating if a discount was used
* **Promo Code Used** – Whether a promotional code was applied

### 🚚 Logistics

* **Shipping Type** – Indicates delivery method (e.g., standard, express)

---

## 📊 Key Analysis & Visualizations

To understand customer profiles and spot trends, the following analyses were performed:

* **Histograms and boxplots** – Distribution of numeric data (e.g., age, purchase amount, review rating)
* **Count plots and pie charts** – For categorical data like gender, category, season
* **Correlation matrix** – To observe relationships between numeric features
* **Bar plots** – Comparison of customer segments across category, color, and payment methods
* **Pairplots & scatterplots** – To observe cluster separation

---

## 🧠 Clustering Process

The clustering methodology focused on **K-Means**, with the following steps:

### 🔧 Preprocessing

* Conversion of categorical features using encoding
* Age derived from birth date
* Scaling of numerical features with StandardScaler
* Dimensionality reduction using PCA for visualization

### 📈 Elbow & Silhouette Method

* The optimal number of clusters was determined using:

  * **Elbow Method**: Plotted inertia vs number of clusters
  * **Silhouette Score**: Measured compactness and separation

### 🧩 Final Clustering Model

* **K-Means** was selected based on its performance and visual interpretability
* Clusters were visualized using 2D PCA plots with color-coded labels
* Characteristics of each cluster were profiled using bar plots

> ❗ Note: HAC (Hierarchical Agglomerative Clustering) and DBSCAN were not used in this project to keep the modeling focused and interpretable.

---

## 📈 Cluster Insights

Each customer group showed distinct patterns based on features like:

* **Spending power** (high vs low purchase amount)
* **Product preferences** (seasonal trends, color/size)
* **Engagement level** (frequency of purchases, use of promos)
* **Satisfaction** (review rating)

These clusters can support:

* Targeted marketing strategies
* Personalized recommendations
* Retention campaigns for high-frequency buyers

---

## 📌 Conclusion

* Exploratory analysis reveals meaningful trends in customer behavior
* K-Means successfully segmented customers into actionable groups
* Elbow and Silhouette methods helped determine an optimal number of clusters
* The insights support data-driven marketing decisions in fashion retail
