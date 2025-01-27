# Predicting-Retail-Loan-Delinquency
Developed a predictive model for retail loan delinquency, focusing on unsecured loans such as personal loans and credit cards in the Indian lending market.

## Context
The landscape of Indian retail lending has experienced significant changes, particularly with the rise in unsecured loans such as personal loans and credit cards. This growth, spurred by digital lending innovations post-COVID-19, brings with it the heightened risk of non-performing assets (NPAs), making effective delinquency prediction more critical than ever for financial stability in the banking sector.

## Problem Statement
The rapid increase in unsecured loans has led to the need for more robust predictive mechanisms to identify potential defaulters. Traditional credit assessment methods are often slow and subject to biases. This project seeks to leverage advanced machine learning techniques to predict loan delinquency, thereby aiding banks in preemptively managing risks associated with unsecured loans.

## Objective
To create a machine learning model that can accurately predict which clients might default on their personal loans and credit cards, based on a detailed analysis of relevant data. This model aims to improve decision-making processes by providing reliable risk assessments tailored to the dynamics of the Indian retail lending market.

## Data Dictionary
The dataset used for this project spans from 2007 to 2014, containing 67,463 records across 44 variables, sourced from Kaggle. Key variables include:
- **Loan Status**: Binary indicator where 1 = Defaulter and 0 = Non-Defaulter.
- **Total Collection Amount**: Total amount collected from the borrower.
- **Debt Consolidation Loan**: Indicates whether the loan is for consolidating debt.
- **Consumer Durable Loan**: Loan for purchasing consumer durable goods.
- **Delinquency in Two Years**: Number of times the borrower was delinquent in the past two years.
- **Inquiries in Six Months**: Number of credit inquiries made in the past six months.
- **Public Records**: Number of derogatory public records the borrower has.
- **Subgrade**: Credit subgrade assigned to the borrower.
- **Batch**: Identifier for the batch of loan applications processed together.
- **Credit Score**: The borrower's credit score at the time of application.
- **Debt-to-Income Ratio**: The borrower's total monthly debt payments divided by their gross monthly income.
- **Loan Amount:** The total amount of the loan issued.

## Model Evaluation and Results
After comparing several models, the Random Forest algorithm was selected due to its superior performance:
- **Accuracy**: 88.9%
- **Precision**: 97.46%
- **Recall**: 79.89%
- **Specificity**: 97.92%
- **F1-Score**: 88%

These metrics demonstrate the model's effectiveness in minimizing both false positives and negatives, crucial for maintaining financial integrity and customer trust.

## Fairness and Explainability
Ensuring fairness and transparency in predictive modeling is crucial to maintaining trust and regulatory compliance. The Random Forest model used in this project includes mechanisms to ensure that the predictions are equitable and free from biases that can skew decision-making. Fairness analysis confirms demographic parity and adherence to regulatory guidelines, with nearly identical predicted positive rates across genders. Moreover, tools like LIME (Local Interpretable Model-agnostic Explanations) provide local explainability, offering insights into individual loan decisions. This level of transparency helps in understanding how and why certain decisions are made, thereby ensuring that all demographic groups are treated fairly.

## Recommendations for Retail Loan Delinquency Prediction

### 1. Focus on Key Risk Indicators
Prioritize key metrics such as Debt-to-Income Ratio, Credit Score, Interest Rate, and Loan Amount. These indicators are critical for evaluating borrower default risk and have been statistically proven to significantly influence loan repayment behavior. They should be at the core of any risk assessment strategy.

### 2. Financial Counselling for High-Risk Borrowers
Implement tailored financial counseling programs aimed at borrowers with high Debt-to-Income Ratios. Providing guidance on effective financial management and structured repayment plans can significantly reduce the likelihood of defaults and enhance the performance of the loan portfolio.

### 3. Implement Strict Approval Thresholds
Establish firm thresholds for high-risk indicators like Debt-to-Income Ratio, Credit Score, Delinquency History, Public Records, Loan Amount, and Inquiries in Six Months. Applicants exceeding these thresholds should be subjected to additional scrutiny or deemed ineligible for loans to ensure responsible lending practices.

### 4. Review and Refine Approval Policies
Regularly review loan approvals that breach predefined thresholds to uncover patterns or justifications for high-risk lending. These analyses can help refine policies to better align with the organization's risk tolerance and strategic goals.

### 5. Strict Delinquency Controls
Enforce stringent cutoff policies for borrowers with histories of delinquencies. Such controls will prevent the approval of loans to high-risk individuals, thus protecting the health of the overall loan portfolio.

### 6. Leverage Explainability Tools for Customization
Utilize tools like LIME for local interpretability and other global feature importance tools to customize loan terms, interest rates, and eligibility criteria to individual borrower profiles. This not only enhances risk assessment but also aligns lending practices more closely with borrower needs.

### 7. Promote Equal Opportunity in Lending
Ensure all demographic groups have equitable access to loan approvals. Continuous monitoring of model performance across various borrower demographics can help avoid systemic biases and promote inclusivity.

### 8. Utilize High-Performing Models for Decision-Making
Deploy the Random Forest model as the primary tool for predicting loan default risk. With its accuracy of 88.9% and precision of 97.46%, it minimizes unnecessary interventions by effectively balancing false positives and false negatives.

### 9. Maintain Trust and Regulatory Compliance
Demonstrate fairness and adherence to regulatory standards across demographic groups, validated by the model’s performance. Employ explainability tools to provide transparent justifications for decisions, which helps in building borrower trust.

### 10. Enhance Borrower Awareness and Credit Education
Invest in financial literacy programs targeting high-risk demographics. Educating borrowers about credit scores, repayment schedules, and risk mitigation can significantly lower default risks and promote a healthier lending environment.

## Conclusion
These recommendations are designed to enhance the predictability and reliability of the loan approval process, ensuring that the bank can effectively manage its portfolio while adhering to best practices and regulatory requirements. By implementing these strategies, lenders can not only reduce defaults but also foster long-term customer relationships and enhance overall market sustainability.
