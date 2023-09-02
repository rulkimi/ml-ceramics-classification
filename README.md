# Ceramic Classification Using Machine Learning
This project focuses on the classification of ancient ceramic samples using machine learning techniques. The main objective is to determine the best-performing model that can accurately identify the type of ceramics based on Fourier Transform Infrared (FTIR) spectroscopy and density measurements.

### 1. Data Preparation

- A dataset of ancient ceramic samples, including 68 samples of three different types (stoneware, porcelain, earthenware), was compiled.
- FTIR spectroscopy and density measurements were performed on each sample, with necessary data preprocessing.
- The dataset was reduced to 469 features representing density and infrared wavelength numbers.

### 2. Data Pre-processing

- Unnecessary data was removed and organized into a single CSV file.
- Dataset splitting into training and testing sets using a 60:40 ratio.
- Handling 'new data' for performance evaluation.

### 3. Data Modeling

- Six classification models (KNN, Naïve Bayes, SVM, Decision Tree, Logistic Regression, Random Forest) were built and trained on the training dataset.
- Evaluation using performance metrics: Precision, Recall, F1-score, Accuracy, AUCROC.

### 4. Model Evaluation

- Quantifying the effectiveness of classifiers in identifying ceramic types.
- Visualizing performance with confusion matrices, ROC curves, and AUC.
- Ensemble learning for model combination.

### 5. Ensemble Learning

- Predictions from individual models combined using majority voting (hard voting).
- Comparison of ensemble performance to individual models.
- Selection of the best-performing ensemble as the final model.

## 6. Classification Predictions
![image](https://github.com/rulkimi/ml-ceramics-classification/raw/main/predictions-output.png)

The Random Forest, Decision Tree, and Naive Bayes algorithms showed high accuracy with 6, 6, and 5 correct predictions out of 7 samples, respectively. This study demonstrates the effectiveness of using FTIR and density data for accurately classifying ceramic materials, suggesting its potential in identifying different ceramic types.

![image](https://github.com/rulkimi/ml-ceramics-classification/raw/main/performance.png)

Among the six models evaluated, NB, LR, and RF consistently demonstrated the highest F1 scores and AUCROC values, indicating their strong performance in precision and recall. Consequently, the ensemble learning approach leverages these three models to collectively enhance prediction accuracy.

## 7. Results

The ensemble learning approach, combining the predictions of top-performing models (NB, LR, RF), resulted in improved ceramic material classification. The ensemble model achieved an impressive F1-score of 0.4595 and an AUCROC value of 0.8461, surpassing the performance of individual models.

![image](https://github.com/rulkimi/ml-ceramics-classification/assets/116322521/b312130b-603e-4746-a8eb-085023e3bd31)

By leveraging the strengths of NB, LR, and RF through ensemble learning, this project demonstrates the effectiveness of ensemble methods in enhancing classification tasks, not only in ceramic material classification but across various domains.

However, despite the overall strong performance of the ensemble model, it is important to note that it still made an incorrect prediction for the third sample. This misclassification could potentially be attributed to the inherent complexity or ambiguity present in the data, which can occasionally lead to misclassifications even when the model performs well. It highlights the need for further data refinement and model fine-tuning to address such cases.
![image](https://github.com/rulkimi/ml-ceramics-classification/raw/main/ml-result.png)

## Code

The project's code, including data preprocessing, model building, and evaluation, is available in the [Code](https://github.com/rulkimi/ml-ceramics-classification/raw/main/python-code.pdf) section of this repository.


## Acknowledgments

Special thanks to my supervisor, Associate Prof. Henk, who has been guiding me throughout this project.
