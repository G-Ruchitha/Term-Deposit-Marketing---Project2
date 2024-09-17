TERM DEPOSIT SUBSCRIPTION PREDICTION

PROJECT OVERVIEW

PROBLEM STATEMENT

Our project is centered on predicting whether a customer will subscribe to a term deposit based on data from a European bank's direct marketing campaigns. 

The aim is to optimize these marketing strategies by identifying key customer segments and predicting outcomes with high accuracy, thereby enhancing the success rates of these campaigns.

DATA DESCRIPTION

The dataset originates from a European banking institution and includes details from direct marketing efforts (phone calls). The features encompass customer demographics and campaign interactions:

Age, Job, Marital Status, Education: Descriptive information about the customer.

Default, Housing, Loan: Financial standing indicators.

Contact, Month, Day, Duration: Specifics of the communication with customers.

Campaign: Interaction frequency during the campaign.

The target variable, y, indicates whether the customer subscribed to the term deposit.

ANALYTICAL APPROACH AND METHODOLOGY

DATA PREPROCESSING

Encoding: Categorical variables (job, marital status, education, contact type) were transformed using one-hot encoding. Numeric values for month were mapped from names to numbers.

Scaling: Feature values were standardized to ensure uniformity for model input.

Sampling: Techniques like SMOTE for oversampling and Random UnderSampling (RUS) addressed class imbalance.

MODELING AND EVALUATION

Multiple classification algorithms were evaluated:

Random Forest and Extra Trees: Utilized for their robustness against overfitting.

XGBoost and LightGBM: Gradient boosting models known for high performance.

Logistic Regression: Provided a baseline for comparison.

Advanced ensemble techniques were also employed:

Voting Classifier: Combined predictions from multiple models.

Stacking Classifier: Layered approach to utilize the strengths of individual models.

Models were assessed based on precision, recall, F1-score, and overall accuracy.

KEY RESULTS

Highest Accuracy Achieved: 96% with an ensemble approach.

Precision and Recall: Notable improvements in predicting actual subscribers, with recall for the positive class reaching as high as 78% after hyperparameter tuning.

Feature Importance: Duration of calls, customer's balance, and the day of contact were identified as the most influential factors.

INSIGHTS AND BUSINESS RECOMMENDATIONS

Targeting Strategy: Focus on customers identified by the models as having a higher probability of subscription, particularly those with longer call durations and higher balances.

Optimal Contact Times: Insights from data suggest specific months and days where customer engagement is higher.

Resource Allocation: By predicting non-subscribers, the bank can save on resources and time, directing efforts towards more promising leads.

CONCLUSIONS

This project successfully demonstrates the use of machine learning to enhance decision-making in marketing strategies for banking products. 
The models developed not only achieve high accuracy but also provide actionable insights for customer segmentation and campaign optimization.

FUTURE WORK

Expand Feature Set: Incorporate more nuanced customer behavioral data.

Model Deployment: Develop a real-time prediction system integrated with the bank's customer relationship management software.

Continuous Learning: Update models periodically with new data to adapt to changing customer behaviors and market conditions.
