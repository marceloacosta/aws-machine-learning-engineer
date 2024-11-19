# Data Preparation: Feature Selection for Mortgage Loan Processing

## Question
A financial adviser plans to use machine learning to improve the efficiency and accuracy of processing mortgage loan requests. By incorporating relevant financial and behavioral data, they aim to reduce the time needed to evaluate applications.

Which options are important for gathering data during model training?

A. Credit bureau data

B. Education History

C. Medical history

D. Employment history

## Correct Answer
A: Credit bureau data

## Explanation

Let's break this down in simple terms:

### What is a mortgage loan?
Think of a mortgage loan as a huge IOU - you're borrowing money to buy a house, and the bank needs to be really sure you can pay it back over many years.

### Why is Credit Bureau Data the BEST choice?
Credit bureau data is like a financial report card that tells the complete story of someone's financial behavior:
1. Shows pattern of payments over time
2. Includes multiple types of loans and credit
3. Provides standardized, reliable metrics
4. Best predictor of future payment behavior

### Why not the other options?

1. **Employment History**
   - While important, it's less predictive than credit history
   - Can change frequently
   - Doesn't show how responsibly someone handles debt

2. **Education History**
   - Not directly related to ability to repay
   - Many successful people with different education levels can repay loans
   - Poor predictor of loan repayment behavior

3. **Medical History**
   - Protected by laws (HIPAA in US)
   - Discriminatory to use for financial decisions
   - Not directly related to ability to repay
   - Using this could lead to legal issues

### Key ML Principle: Feature Predictive Power
In machine learning, we want the feature with the strongest predictive power for our target variable. Credit bureau data has consistently proven to be the single best predictor of loan repayment behavior because:
1. It's based on actual financial behavior
2. Contains long-term historical patterns
3. Includes standardized metrics (credit scores)
4. Aggregates multiple types of financial interactions

### AWS ML Perspective
This aligns with Domain 1 (Data Preparation) of the AWS ML Engineer exam, specifically:
- Selecting the most predictive features
- Understanding data quality and reliability
- Considering compliance and bias implications

### Real-world Application
When implementing this in AWS:
- Use Amazon SageMaker Feature Store to manage credit bureau features
- Implement data quality checks using SageMaker Data Wrangler
- Use SageMaker Clarify to ensure fair lending practices

## Key Takeaways
1. Credit bureau data is the single most predictive feature for loan repayment
2. Historical financial behavior is the best predictor of future financial behavior
3. Always consider both predictive power and compliance requirements
4. Focus on standardized, reliable data sources

## References

1. [What is Credit Risk Analytics? - Experian](https://www.experian.com/blogs/insights/what-is-credit-risk-analytics/)
2. [Prepare data for predicting credit risk using Amazon SageMaker Data Wrangler and Amazon SageMaker Clarify - AWS ML Blog](https://aws.amazon.com/blogs/machine-learning/prepare-data-for-predicting-credit-risk-using-amazon-sagemaker-data-wrangler-and-amazon-sagemaker-clarify/)
3. [Amazon SageMaker Cheat Sheet - Tutorials Dojo](https://tutorialsdojo.com/amazon-sagemaker/)
