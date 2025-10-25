# telecom_subscriptions_churn_prediction_sys
"A machine learning solution for predicting telecom subscriber churn in India (2009–2025). Features data cleaning, engineered metrics, and accurate models (XGBoost, LightGBM), plus a dashboard for risk monitoring and business impact. Production-ready and fully documented."

**Objective:**

The main objective is to develop a robust machine learning system that predicts telecom subscriber churn using India’s operator and circle-level subscription data (2009–2025).
This enables telecom companies to:

- Accurately identify potential churn customers early,

- Understand market structure and competitive risks,

- Quantify business impact and campaign ROI,

- Support targeted retention strategies via an interactive dashboard,

- Maintain high performance and adaptability for real-world deployments.

This drives actionable insights that help reduce churn rates and maximize business value.

**Scope of the Project:**

- Covers India’s telecom subscriptions (wireline & wireless) for all major operators and circles, from 2009 to 2025.

- Includes data preprocessing, feature engineering, churn modeling, and business impact analysis.

- Applies multiple ML algorithms (XGBoost, LightGBM, ensemble) for churn prediction.

- Delivers an interactive dashboard for monitoring churn risk, market trends, and financial impact.

- Supports production deployment, campaign ROI tracking, and quarterly model retraining.

- Enables targeted interventions for the most at-risk regions and operators, driving effective retention strategies.

**Data Description:**

- Monthly telecom subscription data (India, 2009–2025)

- 70,000+ records for all operators and circles

- Main fields:

-  Circle

-  Operator

-  Month/Year

-  Connection Type (Wireline/Wireless)

-  Subscriber Count

- Used for market, trend, and churn analysis

**Installation :**

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/telecom-churn-prediction.git
   cd telecom-churn-prediction
   ```

2. Install required libraries:
   ```
   pip install -r requirements.txt
   ```

3. (Optional) Launch the dashboard:
   ```
   streamlit run app.py
   ```

Ready to use! (You may need to update file paths or configs as per your setup.)

**Data Preprocessing:**

- Removed duplicates and fixed missing values

- Standardized text (operator, circle names)

- Filtered invalid records (like zero or negative subscribers)

- Converted dates and numbers to correct formats

- Made the data clean and ready for modeling

**Feature Engineering :**

- Created over 40 new columns to provide more insights for modeling.

- Added growth rates (Month-on-Month, Year-on-Year).

- Classified circles as Metro or Non-Metro.

- Created features for connection type (Wireline/Wireless).

- Calculated market share, competition metrics, and lagged subscriber values.

- Added rolling averages and volatility measures.

- These features helped improve model prediction accuracy.

**Modeling Approach :**

- Split data into training and test sets by time (to avoid data leakage).

- Used preprocessing pipelines for categorical and numeric features.

- Trained several machine learning models: Logistic Regression, LightGBM, XGBoost, and Ensemble Voting Classifier.

- Tuned model hyperparameters (especially XGBoost with Optuna for best results).

- Chose the best model based on accuracy, ROC AUC, and precision/recall.

- Used feature importance (like SHAP) to interpret which features impact churn predictions most.

**Model Performance :**

- Best model: XGBoost (Optuna tuned)

- Accuracy: 87%

- ROC AUC: 0.91 (very strong classification)

- Precision: 87%, Recall: 80% (high reliability)

- Ensemble Classifier (Voting): Accuracy 84%, ROC AUC 0.91

- Outperformed baseline (Logistic Regression: 71% accuracy)

- Accurately identified high-risk churn cases with few false alarms.

**Business Impact :**

- Helps telecom companies spot churn risks early and take action.

- Supports targeted customer retention campaigns.

- Can protect revenue—up to INR 30 lakh per campaign.

- ROI from retention campaigns can reach up to 4,700%.

- Dashboard and predictions guide resource allocation and strategy.

- Enables executives to react quickly to changing market trends.

**Dashboard & Visualization :**

- Interactive dashboard built with Streamlit.

- Shows key metrics: churn risk, market trends, operator/circle performance.

- Includes risk heatmaps, trend lines, and segment filters.

- Supports real-time data drilldown and export of results.

- Visuals help teams quickly find high-risk areas and track campaign impact.

**Usage Instructions :**

1. Place your data file(s) in the project folder (update path in code if needed).
2. Run the main notebook or Python script to preprocess data and train models.
3. To launch the dashboard:  
   ```
   !streamlit run app.py
   ```
4. Explore model results, predictions, and insights through the dashboard.
5. Adjust settings or retrain by updating code or parameters as needed.

That’s it! Follow on-screen instructions in the dashboard for further analysis.

**Results & Insights :**

- Best model (XGBoost) achieved 87% accuracy and ROC AUC of 0.91.
- Churn risk accurately highlighted for specific circles and operators.
- Dashboard visualizations exposed key trends and high-risk segments.
- Retention actions, if taken early, can deliver up to 4,700% ROI.
- Analysis revealed market share loss patterns and competition effects, helping guide proactive business strategies.

**Limitations & Future Work :**

- Dataset may contain outdated or missing subscription info for some regions.
- Only monthly data granularity; finer trends (e.g., weekly) not captured.
- Churn definitions and business impact calculations may differ by company.
- Current dashboard is local; cloud deployment and mobile support can be added.
- **API development planned:** Future enhancements will include REST API endpoints, enabling integration with company systems and real-time predictions.
- Additional experimentation with deep learning and external customer data sources is possible.

**Contact :**

For questions or support, please contact:  
Siva Narayana Muppidi  
Email: sivanarayanamuppidi11329@gmail.com

You can also openly contact for project-related queries.
