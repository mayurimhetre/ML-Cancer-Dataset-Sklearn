# ML-Cancer-Dataset-Sklearn

The Breast Cancer Dataset is a widely used dataset for predicting whether a tumor is malignant or benign based on clinical features.

## Objective

The goal is to build a classification model that can accurately identify the nature of a tumor to assist in early diagnosis and treatment planning.

### Features

The dataset typically includes numeric features extracted from tumor images, such as:

Radius: mean of distances from center to points on the perimeter
Texture: standard deviation of gray-scale values
Perimeter: length of the tumor boundary
Area: size of the tumor
Smoothness: local variation in radius lengths
Compactness, Concavity, Concave points: shape characteristics
Symmetry and Fractal dimension: structural patterns

The target variable indicates:

0 → Benign tumor
1 → Malignant tumor

This dataset is often used to evaluate machine learning models for medical diagnosis tasks.

---

### Results 
**1.Logistic Regression:**

Scaling Technique used:

**1.StandardScaler**

10 columns not dropped: Accuracy = 98.24%

10 columns dropped : Accuracy = 98.24%

Even if 10 columns removed still accuracy remains the same for logistic regression.

**2.PCA**

NOTE : NO effect on PCA ,even if 10 columns dropped --accuracy remains the same.

**2.DecisionTreeClassifier:**

**Highly correlated columns:**

'area error',
 'mean area',
 'mean concave points',
 'mean perimeter',
 'perimeter error',
 'worst area',
 'worst concave points',
 'worst perimeter',
 'worst radius',
 'worst texture'
 
**NOTE : Accuracy if 10 columns are not dropped :: 91.81 %**
 
 **Accuracy if 10 columns are dropped :: 85.38 %**
       
  **After Grid Search CV:**
       
NOTE : 10 columns not dropped --criterion = 'entropy', max_depth = 3 ,After Hyperparamter tuning accuracy increased to 95.321 %

10 columns dropped -- criterion = 'entropy', max_depth = 6 ,After Hyperparamter tuning accuracy increased to 92.98 %


Conclusion : Those 10 highly coreelated columns should not be removed and logistic or decision tree algorithm can be used.
