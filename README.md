## 📦 Supply Chain Analytics Project
# 🔍 Overview

This project focuses on analyzing delivery operations for a global e-commerce supply chain to identify delays, uncover root causes, and build a predictive model for late deliveries.

The workflow covers the complete data analytics lifecycle — from data loading and cleaning to exploratory data analysis (EDA), reporting, and presentation.

# 📊 Dataset
- Source: DataCo Supply Chain Dataset
- Total Records: 180,519 orders
- Records Used: ~172,765 (after cleaning)
- Features: 50+ columns (reduced to ~20 relevant features)
- Scope: Multi-region, multi-department, multi-year order data

# 🛠️ Tools & Technologies
- Python (Pandas, NumPy)
- Visualization: Matplotlib, Seaborn
- Machine Learning: Scikit-learn
- Data Balancing: SMOTE
- Presentation: Gamma (for PPT creation)

# ⚙️ Project Steps
1. Data Loading
- Imported dataset using Pandas
- Explored structure, columns, and data types
2. Data Cleaning
- Removed irrelevant columns (PII, IDs, etc.)
- Filtered out cancelled orders
- Handled date formats and inconsistencies
- Ensured no duplicates or missing critical values
3. Feature Engineering
- Created key columns:
  - Delay
  - Is_Delayed (True/False)
  - Order Processing Time
  - Time-based features (Month, Day, Hour)
  - Profitability flag
4. Exploratory Data Analysis (EDA)
- Analyzed delay distribution
- Compared delay across:
  - Regions
  - Shipping modes
  - Customer segments
  - Departments
- Identified high-risk areas and bottlenecks
5. Root Cause Analysis
- Investigated reasons behind delays in worst-performing regions
- Identified patterns like:
- Standard shipping delays
- Department-specific issues
- Geographic challenges
6. 📅 Time-Series Analysis
- Analyzed delay patterns over time to detect trends and seasonality
- Key Insights:
  - Monthly Trends: Delay rates increase during peak shopping periods
  - Day-wise Patterns: Weekend orders show higher delays due to processing lag
  - Hourly Trends: Late-night and post-business-hour orders have higher delay probability
  - Mid-week & morning orders show better on-time performance
➡️ This analysis helps in:
- Workforce planning
- Setting accurate delivery expectations
- Identifying peak-risk periods
7. Machine Learning Model
- Built a Random Forest Classifier
- Applied:
  - Frequency Encoding
  - SMOTE for class imbalance
- Goal: Predict whether an order will be delayed

# 📈 Dashboard / Presentation
- Created a structured report summarizing insights
- Designed a presentation using Gamma
- Included:
  - Key KPIs (Delay %, Profit impact)
  - Visual charts from EDA
  - Business insights and recommendations
  
# 📌 Key Results
- ~54.7% orders were delayed
- Most delays fall within 1–4 days
- Standard Class shipping showed highest delay rates
- Certain regions and departments consistently underperformed
- Built a predictive model with strong accuracy to flag risky orders in advance

# 🚀 How to Run
1. Clone the Repository
- git clone [https://github.com/Srishh-ti/Supply-Chain-Analysis.git]
cd Supply-Chain-Analysis
2. Install Dependencies
- `pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn`
3. Run the Notebook
- `jupyter notebook`
- Open the .ipynb file and run all cells
4. View Outputs
- EDA charts and insights in notebook
- Final report (PDF/Doc)
- Presentation (Gamma PPT)

# 💡 Conclusion

This project demonstrates an end-to-end data analytics workflow with real business impact. It not only identifies operational inefficiencies but also provides a predictive solution to reduce delivery delays and improve customer satisfaction.
