# Delivery-Status-Prediction-Model-capstone-project-
1. Data Understanding 
The dataset contains 126,363 entries and 28 columns, with a mix of numeric and categorical data. 
Key Observations 
* Target Variable Delivery_Status seems to be the target variable (classification problem). It 
indicates if the delivery was successful (1) or not (0).
* Categorical Columns Customer_Category, Cust_State, Order_zone, CategoryName, 
Transcation, Dept_Name, Product_type, Shipping_Class, Warehouse_Region. 
*  Numerical Columns Columns like Sales, Price, Profit_Ratio, Discount, Quantity, 
Order_Profit, ProductLength, ProductWeight, Delivery_Review, Session_Ordered, 
WeekdayOrder. 
*  Missing Values Some columns like Sales, Discount, ProductLength, ProductWeight, and 
Delivery_Review have missing values. 
* Potential Features  
Product-related features Product_type, ProductLength, ProductWeight, 
Prod_Category_Id. 
Order-related features Order_zone, Sales, Price, Order_Profit, Discount. 
Customer-related features Customer_Category, Customer_Id, Cust_State, Zipcode. 
2. Data Preprocessing  
Handling Missing Values 
Missing data can reduce the accuracy of machine learning models and introduce bias. Common 
strategies include: 
* Imputation Replacing missing values with estimates, such as the mean, median, or mode 
of the feature. 
* Removal Dropping rows or columns with missing data if the proportion of missing values 
is significant. 
* Predictive Models Using algorithms to predict the missing values based on other features. 
Encoding Categorical Variables 
Categorical variables, which represent discrete values (like "red," "blue," "green"), need to be 
converted into numerical format for most machine learning algorithms. Common techniques 
include: 
* One-Hot Encoding Creates a new binary column for each category (e.g., for a "Color" 
feature with values "red," "blue," "green," you would get three new columns, each 
representing one of the colours).
* Label Encoding Assigns a unique integer to each category (e.g., "red" = 0, "blue" = 1, 
"green" = 2). 
Normalizing Numerical Features 
Normalization scales numerical data to a standard range, which helps some algorithms like 
gradient descent converge faster. Key methods are: 
* Min-Max Scaling Rescales features to a range of [0, 1]. 
* Z-score Normalization (Standardization) Transforms data to have a mean of 0 and a 
standard deviation of 1, useful when the data has a Gaussian distribution. 
3. Exploratory Data Analysis (EDA) Investigate key features influencing delivery success, including 
customer categories, order zones, and product characteristics. 
4. Model Building Use machine learning algorithms like logistic regression, decision trees, and 
random forests to predict delivery status. 
5. Model Evaluation Evaluate models using performance metrics such as accuracy, precision, 
recall, and F1-score. 
* Accuracy The proportion of correctly predicted instances (both true positives and true 
negatives) out of the total predictions. 
* Precision The ratio of true positives to the sum of true positives and false positives, 
measuring the accuracy of positive predictions. 
* Recall The ratio of true positives to the sum of true positives and false negatives, 
indicating how well the model captures actual positives. 
* F1-Score The harmonic mean of precision and recall, balancing the two metrics to handle 
imbalanced datasets. 
* ROC AUC Score The area under the ROC curve, representing the model's ability to 
distinguish between classes across different thresholds, where a score of 1 indicates 
perfect classification. 
6. Conclusion & Reporting Report findings and insights into the factors that influence delivery 
success, with recommendations for improving supply chain performance.
