**📊 Integrated Retail Analytics: Optimization & Demand Forecasting**
**🧾 Project Overview**
This project delivers an end-to-end retail analytics solution designed to bridge the gap between raw data and actionable business strategy. By leveraging 
historical sales data and external economic indicators, the system identifies anomalies, segments stores, and forecasts demand to optimize inventory and operational efficiency.

**🎯 Project Objective**
    The goal is to provide a data-driven framework for retail management to:
    Predict weekly sales with high accuracy.
    Identify sales anomalies and their underlying drivers (e.g., promotions, holidays).
    Segment stores for localized marketing and inventory strategies.
    Quantify the impact of external factors like CPI, Fuel Prices, and Unemployment.
    
**🔍 Methodology & Key Components**
      **1.Data Preprocessing & Feature Engineering**
            Merged disparate datasets (Sales, Store Metadata, and External Features).
            Engineered time-series features: Year, Month, Week, and IsHoliday.
            Handled missing values in promotional markdown data using sophisticated imputation.

      **2. Anomaly Detection**
            Using Isolation Forest and statistical Z-scores, the project flags outliers in sales data. This helps management distinguish 
            between organic growth and data errors or one-time promotional spikes.

    **  3. Store & Department Segmentation**
            Applied K-Means Clustering to categorize stores based on sales volume and economic sensitivity.

**Note: Segmentation quality was validated using the Silhouette Score to ensure distinct, meaningful clusters.**

      **4. Demand Forecasting**
            Built a robust Random Forest Regressor to predict weekly sales.
            Features: CPI, Unemployment, Fuel Price, Store Type, and Seasonality.
            Evaluation: Mean Absolute Error (MAE) and visual trend comparison.

**📈 Tools & Technologies**
       Language: Python 3.x
       Data Manipulation: Pandas, NumPy 
       Visualization: Matplotlib, Seaborn
       Machine Learning: Scikit-learn (Isolation Forest, K-Means, Random Forest)
       Environment: Google Colab / Jupyter Notebooks

**💡 Key Insights**
      Economic Sensitivity: Sales show a notable correlation with CPI and Fuel Prices in specific store segments.
      Seasonality: Holidays contribute to ~20% higher sales volume compared to non-holiday weeks.
      Anomalies: Most detected anomalies were successfully mapped to "Markdown" events, validating the impact of promotional pricing.
