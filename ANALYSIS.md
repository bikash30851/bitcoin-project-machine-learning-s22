# ANALYSIS and Technical Results)

I used the models listed below for my analysis.

## 1. Linear Regression

To check the notebook for linear regression [click here](linear_regression.ipynb).

`On training set`

```
LinearRegression()
value of R2
0.9987710387231933
The value of Mean Squared Error is:  164915.7227507638
The root mean squared error is  406.0981688591612
```
* The value of R2 is 0.998 which is very close to 1 and it shows that the fit is great. A high R2 value for linear regression suggests an
excellent fit and shows strong relationship between the opening and the high price. 

`On Test Set`

```
LinearRegression()
0.9994568683960177
Mean Squared Error:  75744.28108339632
Root Mean Squared Error:  275.21678924694316

```


## 2. Decision Trees

To check the notebook for decision trees [click here](Classification.ipynb).

`On training set`

```
Accuracy:  1.0
Precision:  1.0
Sensitivity:  1.0
F1 Score:  1.0

```

* Since the metrics are a perfect 1 for the training set, it was suspected that the decision tree was overfitting. In the next step the decsion tree was applied on the test set. 

`On Test Set`

```
Accuracy:  0.982620320855615
Precision:  0.985942915466421
Sensitivity:  0.982620320855615
F1 Score:  0.9824600428406657
```

* Here analysis of the decision tree on the test set yeilded metrics that are very close to 1 and the suspicion of the decision tree overfitting the training set might be wrong. However, an analysis of the data with Random Forrest classifier has been done and it will help to clarify things up a little more. *

## 3. SVM

To check the notebook on SVM [click here](Classification.ipynb).

```
Accuracy is  0.7647058823529411
Sensitivity is  0.7647058823529411
Precision is  0.7057921541660694
F1 is  0.7176769726075992
```

* SVM metrics seem to be poor. It could be because the dataset is imbalanced, or the kernel choice was not the best


## 4. Random Forrest
To check the notebook on Random Forrest [click here](Clustering.ipynb).

```
Accuracy (training): 0.9999296833312191
Accuracy (testing): 0.9994286956435832
R2 score : 1.00
Mean squared error: 79673.21
Root Mean squared error: 282.26
```

* To address overfitting of the decision tree metrics Random Forrest with 1000 trees was employed and high metrics yielded suggest it might not be overfitting. 

* Random Forrest seems to do a better job. The R2 score seems to be a perfect 1.0 which could be a result of slight overfitting. Overall random forrest does better than decision tree alone.

## Challenges Faced 

1. I don't think I can call it a challenge, but when I was performing the decision tree analysis on my test set, it yeilded perfect metrics of 1.0 which seemed as if the decision tree was overfitting the training data. Therefore, I tried it on the test set and later used a random forrest which still yeilded very good results. 

2. Using SVM was also challenging task for me. The choice of the kernet was the difficult part. 


## Improvements and Future Prospects

1. It would be interesting to use the date feature for prediction in order to analyse how the currency does during different times of the year. 

2. I think a different size of split might be particulary useful in order to make better prediction.

3. A PCA model can be employed in the future in order to determine if the predictions can be based off a single variable.

4. It would also be interesting to predict by how much the high price would increase given an opening price and time of the year. 






