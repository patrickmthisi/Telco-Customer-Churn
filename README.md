# Telco-Customer-Churn
## Project objectives and description

The dataset used in the project was sourced from: https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data.

The project analyzes customer data to develop a targeted retention program by predicting customer behavior, specifically churn. It involves:
- Exploring various machine learning models to predict customer churn.
- Creating a production-ready scorecard to rank Telco customers by their likelihood of churn.
- Utilizing feature engineering techniques, including binning variables and selecting the most predictive ones based on Information Value (IV) and Gini coefficients.
- Applying Weight of Evidence (WoE) transformation to the selected variables before integrating them into the scorecard.
- Grouping customers into deciles based on their churn probability.
- Assessing the scorecard's stability using Population Stability Index (PSI) and Characteristic Stability Index (CSI) with test data to measure how well the scorecard adapts to evolving data.

## Conclusion and recommendations:
In this project, we created a customer attrition scorecard that can be used to evaluate clients based on their likelihood of attrition. The scorecard shows stellar performance, achieving a ROC AUC of 87% (and Gini of 0.74), which is quite comparable, if not better, than most models that were presented on Kaggle by other participants:

The performance of the scorecard was evaluated using out-of-sample "evolved" data. The scorecard effectively ranked risk, as demonstrated by the decile distribution and the churn versus non-churn distribution shown below:

![deciles](out_of_sample_decile_distribution.png)

![churn](churn_no_churn_distribution.png)


Other models can be explored in this project, as well as other variable selection criteria.
