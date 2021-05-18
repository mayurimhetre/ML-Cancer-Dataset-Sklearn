# ML-Cancer-Dataset-Sklearn

**1.Logistic Regression:**

Scaling Technique used:

1.StandardScaler

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
 
NOTE : Accuracy if 10 columns are not dropped :: 91.81 %

       Accuracy if 10 columns are dropped :: 85.38 %   
       
** After Grid Search CV:**
       
NOTE : 10 columns not dropped --criterion = 'entropy', max_depth = 3 ,After Hyperparamter tuning accuracy increased to 95.321 %

10 columns dropped -- criterion = 'entropy', max_depth = 6 ,After Hyperparamter tuning accuracy increased to 92.98 %
