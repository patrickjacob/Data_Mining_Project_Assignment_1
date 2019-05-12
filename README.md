# Data Mining Project Assignment 1
This is the results of the first Data Mining Project from 2017

[Here the Assignment Report](https://github.com/patrickjacob/Data_Mining_Project_Assignment_1/blob/master/Data_Mining_Assignment1.pdf)

### PART 1: CLASSIFICATION 
Classification of chronic-kidney-disease-2016.arff
1. This part of the assignment is concerned with the file:
[chronic-kidney-disease-2016.arff](https://github.com/patrickjacob/Data_Mining_Project_Assignment_1/blob/master/files/chronic-kidney-disease-2016.arff)
There is a description of the data in the file
[chronic-kidney-disease.info.txt](https://github.com/patrickjacob/Data_Mining_Project_Assignment_1/blob/master/files/chronic-kidney-disease.info.txt)
2. Run the following classifiers, with the default parameters, on this data: ZeroR, OneR, J48, IBK and construct a table of the training and cross-validation errors. You can get the training error by selecting “Use training set” as the test option.
What do you conclude from these results?

|Run No |Classifier|Parameters |Training Error| Cross-valid Error| Overfitting|
|-------|----------|-----------|--------------|------------------|------------|
| 1     | ZeroR    | None      |30.0%         |30.0%             |None        |

3. Using the J48 classifier, can you find a combination of the C and M parameter values that minimizes the amount of overfitting? Include the results of your best five runs, including the parameter values, in your table of results.
4. Reset J48 parameters to their default values. What is the effect of lowering the number of examples in the training set? Include your runs in your table of results.
5. Using the IBk classifier, can you find the value of k that minimizes the amount of overfitting? Include your runs in your table of results.
6. Try a number of other classifiers. Aside from ZeroR, which classifiers are best and worst in terms of predictive accuracy? Include 5 runs in your table of results.
7. Compare the accuracy of ZeroR, OneR and J48. What do you conclude?
8. What are the implications of the above range of accuracies for developing amedical application using classification techniques?
9. What golden nuggets did you find, if any?
10. [OPTIONAL] Use an attribute selection algorithm to get a reduced attribute set. How does the accuracy on the reduced set compare with the accuracy on the full set.

### PART 2: NUMERIC PREDICTION
Numeric Prediction of the Age attribute in the kidney disease data of part 1.
1. Run the following classifers, with default parameters, on this data: ZeroR, MP5, IBk and construct a table of the training and cross-validation errors. You may want to turn on “Output Predictions” to get a better sense of the magnitude of the error on each example. What do you conclude from these results?
2. Explore different parameter settings for M5P and IBk. Which values give the best performance in terms of predictive accuracy and overfitting. Include the results of the best five runs in your table of results.
3. Investigate three other classifiers for numeric prediction and their associated parameters. Include your best five runs in your table of results. Which classifier gives the best performance in terms of predictive accuracy and overfitting?
4. What golden nuggets did you find, if any?

### PART 3: CLUSTERING 10 marks
Clustering of the chronic kidney disease data of part 1. For this part use only the attributes Age,bp,rbc,pc and hemo.
1. Run the Kmeans clustering algorithm on this data for the following values of K: 1,2,3,4,5,10,20. Analyse the resulting clusters. What do you conclude?
2. Choose a value of K and run the algorithm with different seeds. What is the effect of changing the seed?
3. Run the EMalgorithm on this data with the default parameters and describe the output.
4. The EM algorithm can be quite sensitive to whether the data is normalized or not. Use the weka normalize filter
(Preprocess --> Filter --> unsupervised --> normalize) to normalize the numeric attributes. What difference does this make to the clustering runs?
5. The algorithm can be quite sensitive to the values of minLogLikelihoodImprovementCV minStdDev and minLogLikelihoodImprovementIterating, Explore the effect of changing these values. What do you conclude?
6. How many clusters do you think are in the data? Give an English language description of one of them.
7. Compare the use Kmeans and EMfor these clustering tasks. Which do you think is best? Why?
8. What golden nuggets did you find, if any?

### PART 4: ASSOCIATION FINDING
Association finding in the files [bakery-data1.arff](https://github.com/patrickjacob/Data_Mining_Project_Assignment_1/blob/master/files/bakery-data1.arff) and [bakery-data2.arff](https://github.com/patrickjacob/Data_Mining_Project_Assignment_1/blob/master/files/bakery-data2.arff)
These files contain the same details of shopping transactions represented in two different ways. You can use a text viewer to look at the files.
1. What is the difference in representations?
2. Load the file bakery-data1.arff into weka and run the Apriori algorithmon this data. Youmight need to restrict the number of attributes and/or the number of examples. What significant associations can you find?
3. Explore different possibilities of themetric type and associated parameters. What do you find?
4. Load the file bakery-data2.arff into weka and run the Apriori algorithmon this data. What do you find?
5. Explore different possibilities of themetric type and associated parameters. What do you find?
6. Try the other associators. What are the differences to Apriori?
7. What golden nuggets did you find, if any?
8. [OPTIONAL] Can you find any meaningful associations in the kidney disease data?
