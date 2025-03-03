# E-Commerce Customer Segmentation & Dashboard Project

This project analyzes an e-commerce dataset to build a comprehensive dashboard for business managers and marketing teams, and to perform customer segmentation using unsupervised learning. The project is divided into two main parts:

1. **Dashboard for Stakeholders (Power BI):**  
   A well-structured Power BI dashboard that presents key insights from the dataset including:
   - **Customer Demographics:** Breakdown of customers by gender and city (pie charts).
   - **Coupon Usage Trends:** Analysis of coupon transaction status (claimed vs. burned) over time (line charts).
   - **Top-Performing Cities/Branches:** Identification of cities or branches with the highest number of successful coupon burns (heatmaps/bar charts).
   - **Customer Retention and Loyalty:** Insights into customer coupon usage frequency and trends over time (histograms, box plots, and cohort analysis).
   - **Key Performance Indicators (KPIs):** Including total customers, total transactions, burn rate, average time to redemption, etc.

2. **Customer Segmentation Using Unsupervised Learning (Python):**  
   A Python-based analysis that segments customers based on their transactional behavior and demographics. Key steps include:
   - **Data Preparation & Feature Selection:** Merging and aggregating data from multiple tables (customers, genders, cities, transactions, branches, and merchants).
   - **Model Development:** Implementing K-Means clustering (with additional experiments using DBSCAN and Agglomerative Clustering) to identify meaningful customer groups.
   - **Model Evaluation:** Using metrics such as inertia and silhouette score to determine the optimal number of clusters.
   - **Segment Analysis & Coupon Strategy Recommendations:** Analyzing clusters to understand customer behavior and providing actionable recommendations for targeted coupon offers.

## Dataset Description

The dataset is composed of six interrelated tables:

- **Customers Table:**  
  - `customer_id`: Unique identifier for each customer.  
  - `join_date`: The date the customer joined.  
  - `city_id`: The ID representing the customer's city.  
  - `gender_id`: The ID representing the customer's gender.

- **Genders Table:**  
  - `gender_id`: Unique identifier for each gender.  
  - `gender_name`: Name of the gender (e.g., male, female).

- **Cities Table:**  
  - `city_id`: Unique identifier for each city.  
  - `city_name`: Name of the city.

- **Transactions Table:**  
  - `transaction_id`: Unique identifier for each coupon transaction.  
  - `customer_id`: ID of the customer who performed the transaction.  
  - `transaction_date`: The date the coupon was claimed.  
  - `transaction_status`: Status of the coupon (e.g., claimed, burned).  
  - `coupon_name`: The name of the coupon.  
  - `burn_date`: The date the coupon was burned.  
  - `branch_id`: ID of the branch where the coupon was burned.

- **Branches Table:**  
  - `branch_id`: Unique identifier for each branch.  
  - `merchant_id`: ID of the merchant who owns the branch.

- **Merchants Table:**  
  - `merchant_id`: Unique identifier for each merchant.  
  - `merchant_name`: Name of the merchant.

## Installation & Setup

### Power BI Dashboard

1. **Load the Dataset:**  
   Open Power BI Desktop and load the `E-commerce_data.xlsx` file.  
2. **Data Modeling:**  
   Ensure that relationships between tables (e.g., Customers ↔ Genders, Customers ↔ Cities, Branches ↔ Merchants, Transactions ↔ Customers, Transactions ↔ Branches) are correctly established.
3. **Create Visuals:**  
   Follow the provided steps/documentation to build pie charts, line charts, heatmaps, bar charts, histograms, and KPI cards.
4. **Publish & Share:**  
   Once your dashboard is ready, publish it to Power BI Service to share with stakeholders.

### Python Environment for Customer Segmentation

1. **Clone the Repository:**
   git clone https://github.com/yourusername/ecommerce-customer-segmentation.git
   cd ecommerce-customer-segmentation

2. Set Up a Virtual Environment (Optional):
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate

3.Install Dependencies:
  pip install -r requirements.txt

The requirements.txt should include:
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

4. Run the Notebooks/Scripts:
Execute the data preparation, clustering, and segment analysis scripts/notebooks provided in the repository.

## Usage
### Dashboard:
Use the interactive Power BI dashboard to explore customer demographics, coupon usage trends, top-performing regions, and retention insights.

### Customer Segmentation:
Run the Python scripts to:

Prepare and clean your data.
Perform clustering (try different methods like K-Means, DBSCAN, Agglomerative Clustering).
Evaluate and analyze the segments.
Generate coupon strategy recommendations for each customer segment.

## Conclusion
This project provides both a Power BI dashboard and a Python-based unsupervised learning approach to gain actionable insights into customer behavior. The insights can help design targeted coupon strategies to increase customer loyalty and satisfaction.

## Contributing
Contributions are welcome! Fork the repository, create a branch for your feature or bug fix, and submit a pull request.

## Contact
For inquiries or collaboration opportunities, please reach out to me:

**Name**: Malak Ismail  

**Email**: malakismail706@gmail.com 

**LinkedIn**: https://www.linkedin.com/in/malakismail0/




