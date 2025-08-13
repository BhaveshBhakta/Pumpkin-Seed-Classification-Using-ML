## Pumpkin Seed Classification

### Project Overview

This project focuses on **classifying pumpkin seeds** into two distinct species based on various geometric and shape-based features. Using a dataset of image-derived properties like area, perimeter, and eccentricity, the goal is to develop a machine learning model that can accurately distinguish between the 'Çerçevelik' and 'Ürgüp Sivrisi' pumpkin seed types. This task has potential applications in agricultural quality control and food science.

-----

### Technical Highlights

  * **Dataset**: [Kaggle - Pumpkin Seeds Dataset](https://www.kaggle.com/datasets/muratkokludataset/pumpkin-seeds-dataset)
  * **Size**: 2500 entries, 13 columns.
  * **Key Features**:
      * **Geometric Properties**: `Area`, `Perimeter`, `Major_Axis_Length`, `Minor_Axis_Length`, `Convex_Area`, `Equiv_Diameter`.
      * **Shape Descriptors**: `Eccentricity`, `Solidity`, `Extent`, `Roundness`, `Aspect_Ration`, `Compactness`.
  * **Approach**:
      * **Data Cleaning**: The dataset was clean with no missing values or duplicates.
      * **Exploratory Data Analysis**: Histograms and boxplots were used to visualize the distribution of numerical features. A heatmap was generated to show the correlation between these features, revealing strong positive correlations between many of the geometric properties (`Area`, `Perimeter`, `Convex_Area`, `Equiv_Diameter`).
      * **Label Encoding**: The target variable `Class` was converted into numerical labels.
      * **Binary Classification**: The target variable has two classes: `Çerçevelik` and `Ürgüp Sivrisi`. The dataset is well-balanced with 1300 and 1200 entries, respectively.
      * **Models Used**:
          * Logistic Regression, Ridge Classifier, SVC, Random Forest, XGBoost, AdaBoost, Gradient Boosting, Bagging, Decision Tree.
  * **Best Accuracy**:
      * **87.4%** with the Gradient Boosting Classifier.
      * Most other models achieved scores in the **81-86%** range, indicating that the features are effective for this classification task.

-----

### Purpose and Applications

  * **Automate the sorting and quality control of pumpkin seeds** in agricultural and food processing industries.
  * Assist in the identification of different pumpkin varieties, which is important for breeding and seed production.
  * Provide a foundation for developing computer vision systems that can classify seeds directly from images.
  * Demonstrate how machine learning can be used to analyze and classify objects based on their geometric properties.

-----

### Installation

Clone the repository:

```bash
git clone https://github.com/BhaveshBhakta/Pumpkin-Seed-Classification-Using-ML.git
cd Pumpkin-Seed-Classification-Using-ML
```

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost openpyxl
```

-----

### Collaboration

We welcome contributions to improve the project. You can help by:

  * Performing hyperparameter tuning on the Gradient Boosting model to see if the accuracy can be further improved.
  * Investigating different feature engineering techniques to create more powerful classification features.
  * Exploring the use of a deep learning approach, such as a simple CNN, for this task to compare performance with traditional machine learning models.
  * Adding a more detailed analysis of the misclassified cases to understand the model's limitations.
