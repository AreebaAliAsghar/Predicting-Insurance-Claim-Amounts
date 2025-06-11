# Insurance Claim Prediction

## Objective
Estimate medical insurance claim amounts based on personal data such as age, BMI, and smoking status. This helps insurance companies better predict medical costs and adjust policies accordingly.

## Dataset
- Source: [Kaggle - Medical Cost Personal Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)
- The dataset contains personal attributes and insurance charges, including:
  - Age, Sex, BMI, Children, Smoker, Region
  - Charges (target variable)

## Approach
1. **Data Exploration**  
   - Checked for missing values and data types.  
   - Visualized relationships between BMI, age, smoking status, and charges using scatter plots and box plots.

2. **Data Preprocessing**  
   - Encoded categorical features (sex, smoker, region) using Label Encoding.  
   - Defined feature matrix (X) and target variable (y).

3. **Modeling**  
   - Used Linear Regression as the baseline model to predict charges.  
   - Trained on 80% of the data and tested on 20%.

4. **Evaluation**  
   - Evaluated model performance using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).  
   - Visualized predicted vs. actual charges to assess model accuracy.

## Results
- Model achieved a MAE of **4186.5** and RMSE of **5799.5**.
- Plots revealed that:
  - Smoking status and BMI strongly influence insurance charges.  
  - Age also has a clear linear relationship with charges.  
  - Outliers (e.g., high charges for smokers) contribute to prediction error.

## Key Insights
- Smoking status is a primary driver of insurance charges, with smokers incurring significantly higher costs.  
- Higher BMI and age also correlate with increased charges.  
- Linear Regression provides a useful baseline, but further model improvements (e.g., Random Forests, XGBoost) could better handle outlier-heavy data.

## Conclusion
This analysis demonstrates how personal factors like smoking status and BMI affect insurance claim amounts. The baseline model shows the relationships clearly, but more advanced models could improve prediction accuracy. Such insights are crucial for insurance companies to tailor policies and manage financial risk.

## References
- Dataset: [Kaggle - Medical Cost Personal Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)
- pandas: [pandas Documentation](https://pandas.pydata.org/docs/)
- seaborn: [seaborn Documentation](https://seaborn.pydata.org/)
- matplotlib: [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)
- scikit-learn: [scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)

