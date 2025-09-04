# E-Commerce-Logistics-Analysis-and-Delivery-Time-Prediction
Exploratory analysis of the Olist Brazilian E-Commerce dataset to study customer reviews, delivery performance, and freight costs. Includes a baseline linear regression model (R² ≈ 0.11) to predict delivery times, highlighting logistics complexity and improvement opportunities.


**Dataset**

The dataset comes from Olist (publicly available on Kaggle/Dropbox links) and includes:

Customers, sellers, and product details

Orders, order items, payments, and reviews

Geolocation information (city, state, latitude/longitude)



**Key Analysis Steps:**

Data Cleaning: Removed duplicates, handled missing values, standardized date fields.

EDA:

Orders and review trends over time

Negative review text analysis (Portuguese stopword filtering)

Delivery performance metrics (late ratio, hours per 10km)

Freight costs vs. order growth

Seller-to-carrier and carrier-to-buyer delays

Modeling:

Built a Linear Regression model to predict delivery time from order-level features.

Evaluated with RMSE and R².



**Results & Insights**

Order growth slowed after late 2017 alongside spikes in 1–2★ reviews.

Most complaints related to product quality and delivery delays.

Seller preparation time consumed ~25% of delivery time during peak periods.

Average freight cost per 10km rose in 2018, while delivery time improved, leading to flat order growth.

Linear Regression (R² ≈ 0.11, RMSE ≈ 206 hours) showed limited predictive power, highlighting logistics complexity.



**Recommendations**

Set stricter SLAs for seller-to-carrier handoff (e.g., within 48 hours).

Partner with third-party logistics providers for non-SP regions to cut freight costs.

Anticipate demand spikes (holidays, end-of-month) to improve seller readiness.

Monitor KPIs: late delivery ratio, hours per 10km, freight per 10km.




**How to Run**

Clone the repository

git clone https://github.com/your-username/olist-logistics-analysis.git
cd olist-logistics-analysis


Open main.ipynb or main.py in Google Colab or Jupyter.
