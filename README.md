A practical customer segmentation project using Recency, Frequency, Monetary (RFM) analysis and unsupervised machine learning (K-Means) to help e-commerce businesses understand their customer base and design better marketing strategies.

# Motivation
Businesses often struggle to differentiate between loyal, high-value customers and one-time buyers. A generic marketing approach results in wasted budget and lost opportunities. The goal of this project was to:
* Segment customers based on purchase behavior
* Identify high-value and lapsed customer groups
* Enable personalized marketing and retention campaigns

# Dataset
The dataset contains:
* Customer ID
* Order ID
* Quantity
* Unit Price
* Total
* City
* State
Time period: Dec 2023 – May 2025
Source: Google Analytics API (Client's Website) to Excel/CSV

# Methodology (RFM Analysis)
Step 1: RFM Feature Engineering
  * Recency: Days since last purchase
  * Frequency: Total number of orders
  * Monetary: Total spend
Used quantiles to assign RFM scores and rank customer value.

![](/Images_Cust_Seg/RFM_Main.png)

Step 2: Clustering
  * Standardized RFM values using StandardScaler
  * Applied K-Means Clustering
  * Chose optimal k using Elbow Method and Silhouette Score
  * 
![](/Images_Cust_Seg/K-Means.png)

Step 3: Visualization
  * Cluster distribution using Seaborn
  * Bar charts to interpret segments
  * Labeled clusters ("Top Customers", "Average Customers", "Lapsed Customers")
    
![](/Images_Cust_Seg/Clusters.png) ![](/Images_Cust_Seg/RFM.png)
![](/Images_Cust_Seg/Status.png)

# Tools & Technologies
  * Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
  * Jupyter Notebook for development
  * RFM scoring, K-Means clustering, and visual storytelling

# Key Outcomes
  * Identified 4 key customer segments:
    Top Customers: High recency, frequency, and spend
    Average Customers: Frequent buyers with mid spend
    Lapsed Customers: Low frequency, old purchases
    
![](/Images_Cust_Seg/Chart.png)

<a href="https://github.com/ShaguftaPathan/Python/blob/main/Cust_Seg_CCTV.ipynb">View Complete Jupyter Notebook</a>

# Business can now:
  * Launch SEO strategy for at-risk Average and lapsed customers
  * Reward loyal customers with personalized discounts
