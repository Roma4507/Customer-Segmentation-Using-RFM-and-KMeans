
🛍️ Customer Segmentation via Clustering
This project uses unsupervised machine learning techniques to cluster customer transactions based on behavioral purchase patterns. The goal is to segment customers for better targeting, marketing, and sales strategies.

🎯 Objective
To apply clustering (e.g., K-Means and Hierarchical Clustering) to transaction-level data in order to:

Identify distinct groups of customers based on purchasing behavior

Improve marketing efforts through segmentation

Detect anomalies or outlier behaviors

📁 Dataset Description
The dataset contains the following columns:

Column Name	Description
InvoiceNo : Unique identifier for each transaction
StockCode	: Product/item code
Description :	Description of the product
Quantity : Number of units purchased
InvoiceDate : Date and time of purchase
UnitPrice :	Price per unit
CustomerID :	Unique identifier for the customer
Country :	Country of the customer

🔧 Preprocessing
Removed missing or null CustomerID values

Converted InvoiceDate to datetime and extracted features (Month, Hour, etc.)

Calculated total price = Quantity × UnitPrice

Grouped data by CustomerID for behavior-based features:

Total number of orders

Total spend

Average quantity

Recency metrics

🧪 Techniques Used
Feature Engineering:

Aggregated features at customer level

Log transformation and scaling

Clustering:

K-Means Clustering

Elbow Method & Silhouette Score

Agglomerative (Hierarchical) Clustering

Dimensionality Reduction:

PCA for 2D visualization

📊 Visualizations
Histogram to visualize Recency,Frequency and Monetary distributions

Cluster scatterplots in 2D space

Elbow and silhouette method graphs


🛠️ Libraries Used
pandas, numpy

scikit-learn

matplotlib, seaborn

openpyxl (for Excel data loading)

🚀 How to Run
Place Data.xlsx and KYC_Clustering.ipynb in the same folder.

Install dependencies:

bash
Copy
Edit
pip install pandas numpy scikit-learn matplotlib seaborn openpyxl
Launch the notebook:

bash
Copy
Edit
jupyter notebook KYC_Clustering.ipynb

📌 Sample Insights
Some customers frequently place high-volume orders but from limited product categories.

Others purchase small quantities but spend more per unit.

Country-based patterns can distinguish clusters of domestic vs. international buyers.

🔮 Future Work
Incorporate RFM (Recency, Frequency, Monetary) analysis

Integrate DBSCAN for outlier-aware clustering

Build an interactive dashboard using Streamlit

