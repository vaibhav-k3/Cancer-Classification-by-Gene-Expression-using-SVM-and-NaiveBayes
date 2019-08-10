## Cancer Classification using Gene Expression (SVM and NaiveBayes)

> #### 1- Result Comparision after data pre-processing and Model Implementation

Before PCA                                           | After PCA
:--------------------------------------------------------:|:---------------------------------------------------------:
![cross_tab](https://user-images.githubusercontent.com/32847030/62818004-54e8f400-bb0e-11e9-866a-135f2c3c3052.GIF) | ![cross_tab2](https://user-images.githubusercontent.com/32847030/62818005-561a2100-bb0e-11e9-8fc7-d29ea920c29e.GIF)

*Even though the computation time has improved the accuracy has also decreased. However, the main reason behind using PCA was to reduce the dimension of the data set from 7128 variables to 72 variables which can still explain same variation in data with little loss on information. The next step shows the results of applying PCA.* 

#### 2- Dimension Reduction (Implementation of PCA)

![snap2](https://user-images.githubusercontent.com/32847030/62817974-c4121880-bb0d-11e9-9c20-b5830d476402.GIF)

*This plot represents the feature selection process of PCA. We can see that as the number algorithm increases the number of variables to be selected the variation explained by those variables is also increasing. At selecting 72 variables out of 7000 variables, more than 99% variablity is explained.*


#### 3- To regain accuray we need Hyperparameter tuining because the model gave lower accuracy after dimension reduction. 

![snap](https://user-images.githubusercontent.com/32847030/62818006-59151180-bb0e-11e9-94c3-13f5b95e4750.GIF)

*This is the compairsion of perfromance of both the algorithms as feature selection grows. We see that SVM is performaing better than Naive Bayes and hence we can use hyperparameter tuning on SVM to improve the accuracy.

#### 4- Here is the results after tuning

![accuracy](https://user-images.githubusercontent.com/32847030/62818007-5aded500-bb0e-11e9-83b8-7a9d54c9190c.gif)

### Linear Kernal works best for SVM providing 100% accurate results
