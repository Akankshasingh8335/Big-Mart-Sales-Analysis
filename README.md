🏁 **Project Overview**

This project aims to build a machine learning model to predict the sales of various products at different Big Mart outlets using historical sales data.

Accurate sales prediction will help Big Mart optimize their inventory, marketing strategies, and resource allocation.

🎯 **Problem Statement**

Predict the Item_Outlet_Sales for each product-store combination based on product attributes and outlet information.

The main objective is to understand the factors that drive sales and build a model that can accurately forecast future sales.

🤖**Machine Learning Models Used**

Model	Description

1. Linear Regression	          : Baseline model to measure basic predictive power

2. Random Forest Regressor      : Ensemble model with better non-linear fitting

3. XGBoost Regressor	          : Advanced boosting model; prone to overfitting without tuning


📈 **Model Performance**

  Model	Training              |     R²	|Testing R²

1. Linear Regression          |   0.50  | 0.49

2. Random Forest Regressor 	 |   0.87	  |0.55

3. XGBoost Regressor	       |    0.87	|  0.50

🔎 **Observation:**

1. XGBoost performed very well on training but poorly on test → overfitting detected.

2. Random Forest showed the best generalization on unseen data with R² ≈ 0.55.

🔍 **Key Insights**

1. Products with higher MRP tend to have higher sales.

2. The type of outlet (e.g., Supermarket Type 1) significantly impacts sales.

3. Outlet establishment year can influence store popularity.

4. Item visibility needed normalization to improve model stability.


✅ **Conclusion**

1. RandomForestRegressor was the best model with a balance between bias and variance.

2. Feature engineering (interaction terms) and transformation (log-scaling) improved model performance.

3. The project highlights the importance of avoiding overfitting through careful model selection and validation.

💡 **Future Work**

1. Implement hyperparameter tuning (GridSearchCV / RandomizedSearchCV) to improve model accuracy.

2. Try advanced feature selection techniques (like Recursive Feature Elimination).

3. Explore more complex models like CatBoost or LightGBM.

4. Deploy the model using a simple web app (e.g., Streamlit or Flask).

