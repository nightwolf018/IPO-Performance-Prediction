# Deep Learning Classification for IPO Performance Prediction

This project demonstrates building a deep learning classification model using TensorFlow/Keras to predict whether an Initial Public Offering (IPO) will list at a profit or loss. The dataset contains information on past IPOs in the Indian market sourced from Moneycontrol.

## Dataset Information
The dataset used in this project provides information about IPO performance in the Indian market. It includes the following columns:

| Variable | Description |
| --- | --- |
| Date | IPO listing date |
| IPOName | Name of the company going public |
| Issue_Size | Size of the IPO issue in crores |
| Subscription_QIB | Qualified Institutional Buyers subscription rate |
| Subscription_HNI | High Net Worth Individual subscription rate |
| Subscription_RII | Retail Individual Investor subscription rate |
| Subscription_Total | Total subscription rate across all categories |
| Issue_Price | Price per share at which IPO was offered |
| Listing_Gains_Percent | Percentage gain/loss on listing day (target variable) |

The dataset contains 319 complete records with no missing values, representing IPOs from 2010 to recent years.

## Objective
The main objective of this project is to develop a deep learning classification model that can accurately predict whether an IPO will be profitable or loss-making based on subscription patterns and issue characteristics. The model converts continuous listing gains into binary classification (profit vs loss) and provides insights into factors influencing IPO performance.

## Approach
The project involves comprehensive data science methodology:
- **Data preprocessing**: Outlier treatment using IQR method, min-max normalization of features
- **Exploratory data analysis**: Statistical analysis, correlation studies, and comprehensive visualization
- **Feature engineering**: Binary target variable creation, feature selection based on predictive power
- **Deep learning model**: Multi-layer neural network with ReLU activation and sigmoid output
- **Model evaluation**: Training/test split validation with accuracy and loss metrics

Key preprocessing steps include systematic outlier capping, feature scaling, and creation of balanced binary target variable (54.5% profitable vs 45.5% loss-making IPOs).

## Results
- **Model Architecture**: 5-layer neural network (32-16-8-4-1 neurons) with 929 trainable parameters
- **Training Performance**: 73.5% accuracy with 0.52 loss after 250 epochs
- **Test Performance**: 71.9% accuracy with 0.69 loss, showing good generalization
- **Key Insights**: Subscription rates show strong correlations, with total subscription being highly predictive
- **Feature Importance**: QIB and HNI subscription rates demonstrate strongest correlation with IPO success

## Impact
Accurate IPO performance prediction has significant implications for various stakeholders in the financial markets. Investment banks can better assess IPO pricing strategies and market timing. Retail and institutional investors can make more informed decisions about IPO participation. Regulatory bodies can gain insights into market dynamics and subscription patterns. Additionally, companies planning to go public can optimize their issue characteristics based on historical performance patterns.

By leveraging deep learning techniques, this project provides valuable insights into IPO performance prediction and contributes to more data-driven decision making in the primary equity markets.
