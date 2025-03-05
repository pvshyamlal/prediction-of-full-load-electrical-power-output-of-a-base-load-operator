# prediction-of-full-load-electrical-power-output-of-a-base-load-operator
# Objective:
The goal of this project is to forecast the Full Load Electrical Power Output of a base-load operated combined cycle power plant using Polynomial Multiple Regression. This project integrates Clustering to analyze relationships among key variables. Additionally, Cross-Validation is employed to identify the optimal hyperparameters for model performance. The project also utilizes LASSO regression for feature selection and dimensionality reduction. Finally, Bootstrapping is applied to evaluate the model’s accuracy on the test dataset.

#Motivation:
Accurately predicting the full-load power output of a base-load power plant is essential for optimizing energy generation and maximizing revenue from available megawatt-hours. The efficiency of base-load operations is primarily influenced by four key factors: Ambient Temperature, Atmospheric Pressure, Relative Humidity, and Exhaust Steam Pressure. These parameters serve as input variables in the dataset and significantly impact the plant’s overall performance.

# Workflow :
1. **Exploratory Data Analysis**
2. Clustering :
    - K-Means Clustering.
        - Identification of optimal K.
        - Silhouette Analysis
3. Polynomial Multiple Regression:
    - a.	Data Modelling.
    - b.	Division of dataset into: Train, Test and Validation set.
    c.	Cross-validation to find the optimum degree ‘n’ for the polynomial regression.
    d.	LASSO for dimension reduction:
        -	Cross-Validation on Training and Validation set to find the best ‘alpha’ for LASSO reduction.
    e.	Model Evaluation on the Test data using the metrics R^2, and adjusted R^2.
4.  Bootstrapping : Confidence Interval of R^2 for Test Data.

#Results:
1. EDA helps in giving a preliminary glimpse on how various factors are affecting the Power output.
2. Clustering showcases what factors are responsible for a higher Power output:
    - It suggests to increase Power - Humidity and Pressure should also be increased.
    - shows that for high levels of power to be generated, the Plant Temperature and Vacuum levels should be as low as possible.
3. 10-fold Cross-Validation helps in finding the most optimum degree for Polynomial Regression and level of 'alpha' in the LASSO model.
4. LASSO shows what parameters are important in the final model.
5. Bootstrapping reflects the confidence Interval of Accuracy for the model for unseen data.
# Conclusion:
By fine-tuning the hyperparameters through cross-validation and utilizing LASSO for selecting the most significant features, the model achieves 93% accuracy on the test dataset. This demonstrates its effectiveness in accurately predicting the power output of a combined cycle power plant. Implementing this model can help optimize production costs by managing input parameters efficiently, ultimately enhancing the plant's overall performance and operational efficiency.












