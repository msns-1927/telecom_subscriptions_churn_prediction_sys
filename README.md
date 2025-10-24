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

**Data Preprocessing:**

- Removed duplicates and fixed missing values

- Standardized text (operator, circle names)

- Filtered invalid records (like zero or negative subscribers)

- Converted dates and numbers to correct formats

- Made the data clean and ready for modeling
