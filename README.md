# Breast Cancer Data Analysis
The objective of this project is to develop a model that can predict whether a patient has malignant cancer or not. The dataset used in this project is sourced from the UIC machine learning database.

The independent or predictor variables in this dataset are ClumpThickness, Cell Size, Cell Shape, Marginal Adhesion, Single Epithelial Cell Size, Bare Nuclei, Normal Nucleoli, Bland Chromatin, and Mitoses. The target variable that the model aims to predict is the class of the cancer, which is classified as either benign (2) or malignant (4).

## Model Building
The original dataset was used with all variables, but the number of categories for each variable was substantially reduced by grouping them into 2, 3, or 4 clusters as appropriate. The logistic regression model was constructed with a focus on recall, which is critical for identifying every positive case. The model achieved an accuracy score of 96% on the train data and 97% on the test data, with a recall, precision, and f1 score of 96%. The ROC AUC was 97%.

## Conclusion
In conclusion, the analysis of the dataset revealed that certain features are more prevalent in either benign or malignant cases. For instance, marginal adhesion and single epithelial cell size of size 4 and above were found to be more common in malignant cases. On the other hand, benign cases were mostly observed in categories 1, 2, and 3 for both of these features.

The number of normal nuclei was found to be lower in categories 1, 2, and 3 for malignant cases and higher in categories 4 and above, while the opposite was observed for benign cases. Bland chromatin was also found to be more prevalent in malignant cases in categories 3 and above.

For mitosis, benign cases were mostly observed in category 1 and few in category 2 and above, whereas malignant cases were mostly seen in categories 1, 2, 3, and 4. Therefore, it was suggested to club categories 2 and above for modeling and to set the cut-off at 1.

Regarding clump thickness, benign cases were observed in all categories, while malignant cases had a lower thickness in the first four categories. For cell size, most of the benign cases were observed in categories 1, 2, and 3, while malignant cases were more prevalent after category 4. Similarly, for cell shape, most of the benign cases were observed in categories 1, 2, and 3, whereas malignant cases were higher in categories 3 and above, especially in category 5. Lastly, most of the benign cases for bare nuclei were observed in category 1, followed by categories 2 and 3, whereas malignant cases were higher in categories 3 and above, especially in category 10.
