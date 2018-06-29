# Prediction of Age of Abalone(sea snails)

## Regressin Analysis
Abalone are sea snails and in this project we are going to predict the age of abalone based on 8 pysiological characteristics. The age of abalone can be counted from the number of rings on it. So, we will be actually predicting the ring count and in turn geting the age. The data is collected from the UCI machine learning repository. The data set has 4177 samples and of the physiological charaacteristics most important is sex. We hardcoded the string male, female and young as 1, 2, 3. Other features we know includes Length,	Diameter,	Height,	Whole,	Shucked,	Viscera and	Shell. Keras + Scikit learn is the prediction library we are gonna use first in this study.

![EEG](https://raw.githubusercontent.com/jobinregina/prediction/master/head.PNG)

***Image1:*** *CSv dataset of abalone with its features*

I did a preprocessing of the data to see some relevant info, what is the avaerage age of abalone, so we have a general idea about the number of each group and understand how diverse is the group.

![EEG](https://raw.githubusercontent.com/jobinregina/prediction/master/ring.PNG)

***Image2:*** *Age data of abalone plotted against the count*

Then to understand the age of different sex, we plotted the count of male, female and young with their age

![EEG](https://raw.githubusercontent.com/jobinregina/prediction/master/sex.PNG)

***Image3:*** *Age data of abalone plotted against the count*

A scatter plot on the age of the abalone will give u a crystal clear picture of the datset and how u can randomly divide the data for validation, training and test set.

![EEG](https://raw.githubusercontent.com/jobinregina/prediction/master/scat.PNG)

***Image4:*** *Age data of abalone plotted against the count as a scatter plot*

I employed regression algorithm to first to do the prediction, the results of accuracy ws as follows:

![EEG](https://raw.githubusercontent.com/jobinregina/prediction/master/reg.PNG)

***Image5:*** *Comparison of regression analysis*

## Artificial Neural Network
Then I wanted to try with Keras plus theasno how the results will look like and this time it is artificial neural network with the LSTM support. First I use min-max scaler to normalize data between 1 and 0. Then used ANN to perfrom the training and test with a ratio of 
0.75, 0.25.

![EEG](https://raw.githubusercontent.com/jobinregina/prediction/master/pre.PNG)

***Image6:*** *Preprocessing of data into input and target set*

I employed backpropagation through time algorithm to first to do the prediction, the results of accuracy ws as follows:

![EEG](https://raw.githubusercontent.com/jobinregina/prediction/master/ann1.PNG)

***Image7:*** *MSE of test and training set of ANN prediction*

The test set is input to the network and prediction is done on that, I got the following results:

![EEG](https://raw.githubusercontent.com/jobinregina/prediction/master/ann2.PNG)

***Image7:*** *Output of the test data*


