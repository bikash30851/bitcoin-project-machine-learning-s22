# Machine-Learning-Project
Repository of all project documentation and Code

# Link to 5 markdown documents
* [RAW_DATA](RAW_DATA.md)
* [DATA](DATA.md)
* [ANALYSIS](ANALYSIS.md)
* [CONCLUSIONS](CONCLUSIONS.md)

## Introduction
In this project, I am hoping to classify and predict the price of a popular cryptocurrency `Bitcoin`. Features like the volume of the stock, opening and closing price and the market cap might be of particular importance for this study and could help develop a good model. The crypto market is notorious, and it is known to surge certain times of the year, therefore, the date along with the closing price and the market volume might be of particular importance in this study.

## Goals
My goal in this project is to predict the high price of the bitcoin cryptocurrency based upon the origin pirce.

## Changes to initial proposal
I have modified my initial project idea of including both Bitcoin and Ethereum and moved forward with Bitcoin data only. I have made this decison because of the unavailability of proper ethereum data and the inconsistency of the data observed after an initial screening. However, Bitcoin is definitely more popular and would make more a great project. 
  
## Initial Exploration
The data contained in `bitcoin.csv` was particulary interesting because of the combination of relevant information it contained. The initial `.info()` analysis revealed the detailed data present in the open high and closing tables. Most of the data contained is either a float or an integer which makes it ideal for mathematical analysis. 

An initial look at this data shows an ideal data set which is ready for linear regression analysis. 

## Linear Regression
In order to perform the linear regression, using the train_test_split() function the data was split into a training(75%) and a test(25%) set. First the open and high prices were picked as inital X and Y values for our model which yeilded promising R2 values but not so great mean squared and root mean squared values. 

Furthermore, in order to make the model better and in the hope of better metrics 3 other features were picked in conjunction with Open price and linear regresssion analysis was performed. It must be a result of using extra parameters to overfit the model, but the model did very well with 3 parameters. The metrics got better as more parameters were added. The volume and market cap I think would be two of the important parameters to look at for further data analysis.

## Classification
In order to perform the classification, decision tree and SVM were chosen. First of all the data was read into a pandas dataframe called dataframe_btc. An initial exploration of the data was performed again in order to obtain a closer view of the data and to look at different features in order to get ready for decision tree and SVM classification. For decision tree, since the data that I have picked was the High price as the target, the value is a float64 which is continuous in nature.

Therefore, a grader function was introduced which allowed for bucketing of the data ultimately facilitating the decision tree classification. All the metrics were calculated and then SVM was performed on the data. Similar to decision trees, metrics for the SVM were also calculated and comparison was done.

A final commentary has been done on the performance of the model and all the metrics. 

## Clustering
Performed clustering analysis on the data with 4 features and obtained the results. 
The clusters and centroids are pretty conjusted which shows that acute clustering of the data. 
Performed dimensional reduction and visualized the data using scatter plots and scatter matrix. 
Visualization of the data revealed positive correlation among the features which might be somewhat concerning
however, there could be several other lurking factors that should be considiered. 

Random Forrest analysis yeilded an accuracy of 0.99 for both the testing and training sets.
Further analysis is performed with Neural Nets. 

## Final Changes
My decision tree was overfitting and I was missing an analysis on my test set. As advised by Dr. Hoot I performed an analysis on my test set and actually got better metrics that could be used for better inference and analysis. I went ahead and did the same thing with the SVM classifier and got meaningful metrics. 

## Poster pptx and Poster pdf

* [Poster Powerpoint](AdhikariBFinalPoster.pptx)
* [Poster PDF](AdhikariBFinalPoster.pdf)

## Narrative Conclusion
After applying various models and analyzing the metrics, it can be concluded that the high price of bitcoin has a strong positive correlation with the opening price. A PCA exploration might be handy and useful in order to deermine and gain more confidence to realize if the change in high price can solely be attributed to the opening price of the currency. 

