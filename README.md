# Kaggle-Credit-Risk-Assessment
This project explores credit risk assessment using three models: Random Forest, Self-Organizing Maps (SOM), and a hybrid approach combining both. The models are evaluated using a credit card dataset, with a focus on accuracy, precision, recall, F1 score, and AUC, demonstrating the effectiveness of combining supervised and unsupervised techniques.
# Credit Risk Assessment using Combined Supervised and Unsupervised Model

This project explores the use of machine learning models for credit risk assessment, focusing on three different approaches: 
1. **Random Forest (Supervised Learning)**
2. **Self-Organizing Maps (SOM) (Unsupervised Learning)**
3. **Hybrid Model** that combines SOM with Random Forest.

The goal of the project is to improve the accuracy and reliability of credit risk prediction using advanced machine learning techniques. The models are evaluated on key metrics like accuracy, precision, recall, F1 score, and AUC using a credit card dataset.

## Models Tested

### 1. **Random Forest (Supervised Model)**
A widely used machine learning algorithm for classification tasks, Random Forest was first tested to assess its predictive performance in credit risk assessment. It produced strong performance with high precision and recall.

### 2. **Self-Organizing Maps (SOM)**
SOM was employed as an unsupervised learning technique to cluster data based on patterns and similarities. It helps reveal hidden structures in the data and assigns cluster labels to be used in further modeling.

### 3. **Hybrid Model: SOM + Random Forest**
The hybrid approach integrates the clusters generated by SOM as additional features into the Random Forest model. This approach enhances the predictive performance by combining the strengths of both supervised and unsupervised techniques.

## Key Metrics

- **Accuracy**: Measures the proportion of correct predictions.
- **Precision**: Proportion of positive predictions that are actually correct.
- **Recall**: Proportion of actual positives that were correctly identified.
- **F1 Score**: Harmonic mean of precision and recall.
- **AUC**: Area under the ROC curve, indicating the model’s ability to distinguish between classes.
## Results and Findings

### Model Comparison

- **Integrated Model (SOM + Random Forest)**: This hybrid model achieved the highest performance with high accuracy (0.93), precision (0.96), and AUC (0.93). However, the recall (0.69) was lower, indicating that it may miss some defaults. This model leverages the strengths of both unsupervised and supervised techniques.

- **Unsupervised Model (SOM)**: The SOM model, while able to cluster the data, performed weaker in terms of precision (0.68) and recall (0.43). It struggled to capture defaults accurately and showed a higher false positive rate.

- **Supervised Model (Random Forest)**: The Random Forest model balanced precision (0.93) and recall (0.93) well, with a good F1 score of 0.92. While it performed very well, the integrated model slightly outperformed it due to the additional SOM features.

### Risk of Overfitting
The Random Forest model showed potential for overfitting, but the metrics indicated it generalized well. Regularization techniques, such as limiting tree depth, are recommended to mitigate this risk.

## Conclusion

The hybrid SOM + Random Forest model demonstrated the best performance overall, combining the benefits of both unsupervised and supervised techniques. It performed excellently in predicting non-defaults but could miss some defaults. The Random Forest model alone was highly effective, but the hybrid model enhanced its ability to capture complex patterns. The SOM model, on its own, did not perform as well but contributed valuable features to the integrated model.


