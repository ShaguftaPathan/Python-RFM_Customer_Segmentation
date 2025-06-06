<a href="https://shaguftapathan.github.io/Python-RFM_Customer_Segmentation/">View Project</a>

A practical customer segmentation project using Recency, Frequency, Monetary (RFM) analysis and unsupervised machine learning (K-Means) to help e-commerce businesses understand their customer base and design better marketing strategies.

<span style="color:#4a89c2; font-size:22px;"><b>Motivation</b></span>  
Businesses often struggle to differentiate between loyal, high-value customers and one-time buyers. A generic marketing approach results in wasted budget and lost opportunities. The goal of this project was to:  
* Segment customers based on purchase behavior  
* Identify high-value and lapsed customer groups  
* Enable personalized marketing and retention campaigns  

<span style="color:#4a89c2; font-size:22px;"><b>Dataset</b></span>  
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

<span style="color:#4a89c2; font-size:22px;"><b>Methodology (RFM Analysis)</b></span>  
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

![](/Images_Cust_Seg/K-Means.png)  

Step 3: Visualization  
  * Cluster distribution using Seaborn  
  * Bar charts to interpret segments  
  * Labeled clusters ("Top Customers", "Average Customers", "Lapsed Customers")  
    
![](/Images_Cust_Seg/Clusters.png) ![](/Images_Cust_Seg/RFM.png)  
![](/Images_Cust_Seg/Status.png)  

<span style="color:#4a89c2; font-size:22px;"><b>Tools & Technologies</b></span>  
  * Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)  
  * Jupyter Notebook for development  
  * RFM scoring, K-Means clustering, and visual storytelling  

<span style="color:#4a89c2; font-size:22px;"><b>Key Outcomes</b></span>  
  * Identified 4 key customer segments:  
    Top Customers: High recency, frequency, and spend  
    Average Customers: Frequent buyers with mid spend  
    Lapsed Customers: Low frequency, old purchases  
    
![](/Images_Cust_Seg/Chart.png)  

<a href="https://github.com/ShaguftaPathan/Python/blob/main/Cust_Seg_CCTV.ipynb">View Complete Jupyter Notebook</a>  

<span style="color:#4a89c2; font-size:22px;"><b>Business can now:</b></span>  
  * Launch SEO strategy for at-risk Average and lapsed customers  
  * Reward loyal customers with personalized discounts  
