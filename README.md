# PCA_Project_over_Breast_Cancer_Digit_Recognition_Dataset
# Project Title: Principal Component Analysis for Dimensionality Reduction: A Comparative Study of Feature Structure and Classification Performance
## Abstract:
This study investigated how Principal Component Analysis (PCA) affected dimensionality reduction and classification performance using the Breast Cancer and Digits datasets. The datasets were selected because they had different feature structures. Pearson correlation, KMO, and Bartlett's test were used to analyse relationships among the features. PCA was applied after standardisation using different numbers of principal components, while the same Logistic Regression classifier was used before and after PCA for comparison. The evaluation considered explained variance, classification accuracy, F1-score, dimensionality reduction, training time, and reconstruction error. For the Breast Cancer dataset, 10 components retained 95.27% of the variance with 66.67% dimensionality reduction and achieved 96.49% test accuracy. For the Digits dataset, 50 components retained 98.33% of the variance with 21.88% dimensionality reduction and achieved 96.67% test accuracy. The results showed that PCA effectiveness depended on the feature structure of the dataset, and selecting the number of components required a balance between information retention, classification performance, and dimensionality reduction.

## Datasets: Breast Cancer {0/1} and Digits {0-9} datasets Loaded from sklearn
## Scree Plot (Explained Variance and CUMULATIVE Variance) for Breast Cancer

<img width="1790" height="690" alt="image" src="https://github.com/user-attachments/assets/69573d31-8a75-4423-81c4-f230170d2a75" />

## Scree Plot (Explained Variance and CUMULATIVE Variance) for Digit Recognition
<img width="1789" height="690" alt="image" src="https://github.com/user-attachments/assets/feb76a1e-44ad-4900-92ab-ff1a98be4550" />


## Visualization of Train and Test accuracy over different Principle Components
<img width="1589" height="590" alt="image" src="https://github.com/user-attachments/assets/656c8fe3-e601-421b-b3ba-14b2cf3e68e6" />


## Visualization of Test Accuracy vs Variance Retained
<img width="1588" height="590" alt="image" src="https://github.com/user-attachments/assets/ad0fd045-1906-474b-970d-374c9737ecd6" />

## PCA Projection: Categorywise Scatter plot (PC1 vs PC2) both Breast Cancer and Digit Dataset
<img width="1585" height="590" alt="image" src="https://github.com/user-attachments/assets/fd59342e-1c2d-441f-84b0-50571e2061fe" />


## Discussion:
The main findings of this study are summarized as follows:

- Feature Structure: The Breast Cancer dataset showed stronger overall feature relationships than the Digits dataset, based on its higher mean absolute correlation and KMO value.
- Breast Cancer Dataset: Ten components retained 95.27% of the variance with 66.67% dimensionality re- duction and achieved 96.49% test accuracy. Increasing to 25 components retained 99.95% of the variance and recovered the 98.25% baseline accuracy.
- Digits Dataset: The Digits dataset required more com- ponents to preserve comparable information. Fifty com- ponents retained 98.33% of the variance with 21.88% dimensionality reduction and achieved 96.67% test accu- racy, while 60 components matched the 97.22% baseline.
- Performance Trade-off: Increasing the number of com- ponents consistently increased variance retention, but classification performance did not always improve. This showed that variance retention and predictive perfor- mance were related but not identical..
- Overall Finding: PCA effectiveness depended on the feature structure of the dataset. Therefore, component selection should balance variance retention, classification performance, reconstruction quality, and dimensionality reduction

## Conclusion
This study showed that PCA reduced feature dimensionality while preserving useful information and classification performance, although its effectiveness depended on the feature structure. For the Breast Cancer dataset, 10 components retained 95.27% of the variance with 66.67% dimensionality reduction and achieved 96.49% test accuracy, while 25 components retained 99.95% variance and recovered the 98.25% baseline accuracy. For the Digits dataset, 50 components retained 98.33% variance with 21.88% dimensionality reduction and achieved 96.67% test accuracy, while 60 component retained 99.92% variance and matched the 97.22% baseline. These results showed that PCA component selection should jointly consider variance retention, predictive performance, and dimensionality reduction rather than relying on a single criterion.


