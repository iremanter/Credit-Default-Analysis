First of all, the “Loan Status” column has been converted into numerical values by using a mapping method to create bar charts, correlation matrices and heatmaps. 

<img width="638" alt="Screenshot 2025-03-14 at 00 39 40" src="https://github.com/user-attachments/assets/2cc5bebb-9edd-4515-82ba-e2b686364c68" />
<img width="638" alt="Screenshot 2025-03-14 at 00 39 44" src="https://github.com/user-attachments/assets/9d86f93c-83b8-4fe9-823c-32de3bc5b2ba" />
<img width="620" alt="Screenshot 2025-03-14 at 00 39 51" src="https://github.com/user-attachments/assets/d0acd8fc-da97-447b-bced-53aa4b319478" />

Secondly, bar charts have been plotted for education levels, marital statuses, genders, self employment statuses, property areas, and the number of dependents that the customer has. 
The bar chart interpretations can be summarized as follows: The loan applications of graduate applicants are more likely to be approved than those of non-graduate applicants. 
When comparing the loan application status of single and married customers, the bar chart shows that married customers have a higher approval rate than single customers. 
The gender bar chart reveals a significant difference in loan application approval between male and female customers, with the male customers' applications being more likely to be approved. Additionally, it was found that self-employed applicants have a higher risk of being rejected when they apply for a loan. The property area bar chart indicates that the highest, medium, and lowest loan application approval rates occur in semi-urban areas, urban areas, and rural areas, respectively. 
Lastly, customers with no dependents have a higher chance of approval compared to customers with one, two, three, or more dependents.

<img width="616" alt="Screenshot 2025-03-14 at 00 39 57" src="https://github.com/user-attachments/assets/1b2967a0-cdbf-4c5b-8122-3b0bc301f483" />
<img width="643" alt="Screenshot 2025-03-14 at 00 40 02" src="https://github.com/user-attachments/assets/5d8f0efb-5b21-4480-b4ae-4043fcbc695c" />

Histograms have been plotted for the loan amount applied for, loan amount term, and applicants' and co-applicants' income levels. The highest frequency of loan amount applications is around 120,000 Euros, and the most frequent loan term is one year. The loan application dataset contains mostly applicants with approximately 2,500 Euros income, while co-applicants have literally no income.

<img width="316" alt="Screenshot 2025-03-14 at 00 40 07" src="https://github.com/user-attachments/assets/b0d3461f-d45d-4e94-a2ce-515abbe9b570" />
<img width="313" alt="Screenshot 2025-03-14 at 00 40 13" src="https://github.com/user-attachments/assets/48710708-bda5-4277-b1ee-1a4ec309d88f" />

Correlation matrices were created for both numerical and categorical columns. Since correlation matrices can only be applied to numerical attributes, categorical columns were converted into numerical columns using a mapping method. According to the correlation matrices, the attribute with the highest correlation to the target variable (loan application status) is the credit history attribute, with a correlation coefficient of 0.6. This can be interpreted as a strong correlation, as it is higher than 0.5. Also, two different heatmaps of two different groups have been created to visualize the correlation between all attributes.

Min-max scaling has been performed to normalize the data before developing these three different models. Min-max scaling, which enhances the performance of decision tree, logistic regression, and random forest models, normalizes the attributes and converts them into a similar scale. After applying this scaling method, the dataset was divided into training and testing sets. 80% of the data used for training and 20% for testing.

The random forest, decision tree and logistic regression models have been developed, trained and tested by using necessary Python functions which are below. All models outputs and performances have been compared and evaluated in the evaluation part.

The model evaluation techniques have been performed for the Random Forest, Decision Tree and Logistic Regression models. Four different performance metrics, which are accuracy, precision, recall, and f1-score, have been calculated, evaluated and compared to decide which model is the best performed model for this project.

- Accuracy: Random Forest, Decision Tree, and Logistic Regression models have accuracy rates of 0.86, 0.83, and 0.83, respectively.
- Precision: Random Forest, Decision Tree, and Logistic Regression models have precision rates of 0.82, 0.84, and 0.81, respectively.
- Recall: Random Forest, Decision Tree, and Logistic Regression models have recall rates of 1.00, 0.92, and 0.98, respectively.
- F1-Score: Random Forest, Decision Tree, and Logistic Regression models have f1-score rates of 0.90, 0.88, and 0.88, respectively.

To sum up, the best performing model is the Random Forest model with the highest accuracy and f1-score. Additionally, it has perfect recall, which indicates that the algorithm is effective at identifying all positive instances. On the other hand, the Decision Tree model performs well with the highest precision, which indicates the least false positives. However, it has lower recall and accuracy when compared to the Random Forest model. Lastly, the Logistic Regression model has high accuracy, recall, f1-score, but it has lower precision when compared to the Random Forest and Decision Tree models.

<img width="473" alt="Screenshot 2025-03-14 at 00 38 48" src="https://github.com/user-attachments/assets/cab72057-78eb-4ef5-9ec3-89fa1cb72904" />

After conducting the model evaluation part, the ROC Curve (receiver operating characteristic) has been plotted to visualize the models’ performance and, AUC (Area under ROC Curve) has been calculated for each model. 
According to the ROC curves and the AUC values, the Random Forest model with an AUC of 0.82 is the best performing model of loan application dataset when compared to the Decision Tree model with an AUC of 0.78 and the Logistic Regression model with an AUC of 0.79.

The Random Forest model is the best-performing model in terms of accuracy, recall, f1-score, and AUC when compared to the Decision Tree and Logistic Regression models. 

The success of the Random Forest model enables credit risk departments to handle large datasets with higher dimensionality. Therefore, the Random Forest model is an ideal choice for loan approval prediction, where data consists of multiple features with varying significance.

Moreover, integrating this predictive model into the existing loan prediction system provides financial institutions and banks with improved efficiency, reduced processing times, enhanced customer satisfaction, and increased reliability of loan approval processes. Since Credit Risk Departments are responsible for reducing the risk of approving loans that have a high probability of default and rejecting loans that are likely to be repaid, they can apply the Random Forest model.
