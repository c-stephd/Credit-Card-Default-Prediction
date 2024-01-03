# Credit Card Default Prediction Model

## Project Overview
This project involves the creation of a predictive model to identify potential credit card defaults. It leverages advanced data analysis techniques to ensure reliability and cost-effectiveness in prediction. The model is built and tested on two separate cohorts of 200 applicants each, aiming for the highest sustainable performance.

## Features
- **Binary Classification Model**: Predicts the likelihood of a credit card holder defaulting on payments.
- **Performance Metrics**: Utilizes Area Under Curve (AUC) for robust performance validation.
- **Financial Value Analysis**: Employs techniques to quantify and maximize the financial impact of the model.
- **Threshold Optimization**: Identifies optimal decision-making thresholds for minimizing costs per event.
- **Eggertopia Scores**: Incorporates a specialized method for enhancing prediction accuracy and cost savings.

## Tools Used
- **Excel with Advanced Features**: Model developed using macros and formulae in Excel for data analysis and prediction.

## How to Use
1. **Data Preparation**: Input your dataset of credit card applicants into the model.
2. **Model Training**: Use the training set (200 applicants) to train the model.
3. **Validation and Testing**: Validate the model's performance using the AUC metric on a separate test set (200 applicants).
4. **Apply Thresholds**: Implement the optimized thresholds for cost-per-event minimization in real-world scenarios.
5. **Evaluate Savings**: Calculate the financial impact using Eggertopia scores and the cost savings achieved.

## Findings

### Model Description
Model formula:
\( 2 \times [\text{Years at current employer} + \text{Credit Card Debt}] + \text{Age} + \text{Automobile Debt} \)

### Performance Metrics
- **AUC (Area Under Curve):** Achieved an AUC of 0.81 on the Training Set and 0.85 on the Test Set, indicating consistent and possibly improved performance on unseen data.
- **Cost Per Event:** With cost estimates of $5,000 per False Negative and $2,500 per False Positive, the ideal metric changes from AUC to average cost-per-event at the model’s threshold score.
- **Thresholds and Cost-per-Event:** The example model has a minimum cost-per-event of $713 on the Training Set at a threshold of 0.2. On the Test Set, the sustainable cost-per-event is $763, suggesting minimal over-fitting.

### Considerations
- **Model Robustness:** Comparing cost-per-event on the Test Set and Training Set is a rigorous test of model robustness. A dramatic increase in cost-per-event indicates over-fitting, and the model should be reconsidered.
- **Base Rate Understanding:** A crucial aspect of predictive modeling is understanding the base rate and cost-per-event at the base rate. Any classification model to be useful must outperform base-rate forecasting, evidenced by a Test Set AUC greater than 0.5, and cost-per-event less than $1,250.
- **Incremental Value:** The model demonstrates significant savings per event, indicating its effectiveness over base-rate forecasting.

### Conclusion
The provided model serves as a testament to the potential of predictive analytics in financial decision-making, with significant savings and reliable performance demonstrated. Understanding the balance between complexity and utility is critical for efficient model design and application.



This project was gotten from a Mastering Data Analytics in Excel course on Coursera
