# Project Summary
This project sought to develop a supervised classification model to forecast whether a product will be clicked in an e-commerce environment based on user, product, and session attributes. With a dataset having attributes like category, product_type, item_price, app_code, and device-related variables, various machine learning models were trained and tested, such as Logistic Regression, Decision Tree, Random Forest, and SVM.

The analysis was both model performance and interpretability-oriented. Random Forest and Decision Tree models performed best with regard to prediction accuracy and feature importance. Feature importance analysis revealed that features like dayofweek, is_4G, category, item_price, and session_id had the greatest impact on user click behavior, with different models prioritizing different features. The results underscore the importance of model selection based on the nature of the input data and the patterns of prediction each model is most suited to detect.

# Dataset Overview
The dataset used in this project contains user interaction logs from an e-commerce platform. It consists of session-level data including both user and product-related features, and whether the user clicked on the product. 

device_type indicates the type of device used, such as mobile or desktop. 
user_id and session_id are unique identifiers for the user and their browsing session, respectively. 
Each product is represented by a unique item_id. 
item_price reflects the cost. 
The category column provides a broad classification of the item, while product_type offers a more specific subtype. 
The impression_time marks the exact timestamp when the product was shown to the user.
app_code, represents the application version or variant.
os_version, which records the device’s operating system version. 
The is_4G column indicates whether the user was on a 4G network during the session. 
The target variable is_click denotes whether the product was clicked, with 1 indicating a click and 0 otherwise.

# About Project
In this project, we analyzed feature importance across Logistic Regression, Decision Tree, Random Forest, and SVM models to identify key factors influencing whether a product is clicked in an e-commerce setting.

The analysis showed that different models prioritize different features. For instance, dayofweek was a significant predictor in Logistic Regression, indicating a strong linear relationship with user clicks, but was negligible in tree-based models and SVM. Features like os_version_old and os_version_latest were more important in Logistic Regression and SVM, suggesting system versions impact click behavior. The hour of interaction was especially important in SVM, highlighting how time of day may influence user engagement.

Technical attributes like is_4G and app-specific features such as category and app_code were particularly influential in SVM, while Random Forest and Decision Tree models relied more heavily on product-related variables like item_price and product_type. Session-level data, including session_id and item_id, also showed moderate importance in these tree-based models.

# Conclusion
Model interpretability highlighted the diverse factors influencing click behavior, including time, product details, and device characteristics. Since each model emphasizes different variables, aligning model selection with the structure and dynamics of the dataset is key to enhancing predictive accuracy. Understanding feature importance not only improves performance but also supports more informed decision-making in optimizing e-commerce strategies.








