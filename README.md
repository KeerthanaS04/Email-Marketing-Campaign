# Email-Marketing-Campaign

The goal of this campaign was to inform users about a new feature via email and evaluate the click-through rate (CTR) as a success metric. Ultimately, we want to optimize future campaigns using machine learning to increase engagement.

## Campaign Performance Summary
- Total Emails Sent: 100,000
- Email Open Rate: 10.35%
- Click-Through Rate (CTR): 10.35%

## Can We Predict Clicks to Optimize Email Sends?
Yes. Based on the available features and user behavior data, we built several models to predict whether a user would click the email link.

### Model Performance (ROC AUC)
Model | ROC AUC

Logistic Regression | 0.6745

Random Forest | 0.6002

Gradient Boosting | 0.6855 

Support Vector Machine | 0.5501

K-Nearest Neighbors | 0.5731

KNN Ensemble | 0.6058

Neural Network | 0.6723

XGBoost | 0.6815

CatBoost | 0.6784

Best Model: Gradient Boosting
Reason: Highest AUC (0.6855) — a reliable indicator of ranking power for imbalanced data like this.

### Expected Improvement with Targeting
- Model-targeted CTR: 19.74%
- Baseline CTR: 10.35%
- Estimated Improvement: +90.82%

### Hypothetical ROI:
- Original Clicks: ~10,350
-Predicted Clicks: ~19,740
- Additional Clicks Gained: ~9,390

### Insights from User Segments
#### Email Version
Version | CTR

Generic | 7.93%

Personalized | 12.78% 

#### Day of Week
Weekday | CTR

Tuesday | 12.05% 

Wednesday | 12.03%

Thursday | 11.84%

Monday | 11.61%

Saturday | 8.77%

Sunday | 8.76%

Friday | 7.41%

Early to mid-week (Monday–Thursday) drives better engagement. Avoid sending on Fridays and weekends.

#### User Purchase History
Past Purchases | CTR

0 | 3.83%

1 | 9.28%

2–5 | 10.85%

6+ | 13.34% 

Users with more purchase history are more likely to engage. Segmenting by past behaviour is crucial.

- **Designed and implemented a statistically rigorous A/B testing pipeline** to evaluate email click-through rates (CTR), randomly assigning 50% of users to a control group and the top 20% (based on model-predicted probabilities) to a treatment group.

- **Leveraged a predictive model to identify high-engagement users**, resulting in a treatment group CTR of **18.65%**, significantly outperforming the control group CTR of **10.46% (Z = -23.21, p < 0.0001)**.

- **Achieved a ~78% lift in CTR through data-driven targeting**, demonstrating the effectiveness of integrating machine learning with experimentation for marketing impact.
