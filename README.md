# Neural Network and Machine Learning

## Project Overview:

In this project we help a the business team of a company named `Alphabet Soup` create a binary classifier. A Binary classifier capable of predicting whether applicants will be successful if funded by Alphabet Soup. We are given a CSV file with more than 34,000 organizations that have received funding from them over time. The dataset provides important metadata about each organization that we will use to complete our project.


## Data:

Provided CSV file of past funding (charity_funding.csv)

* EIN and NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* SPECIAL_CONSIDERATIONS—Special consideration for application
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively

## Methodology:

1. Pre-process the Data for a Neural Network Model
2. Compile, Train, and Evaluate the Model
3. Optimize the Model

## 1. What variable is considered the target for the model?
An "Accuracy of at least 75%" variable is the target for our model as we are trying to predict a level of success if funded.

## 2. What variable(s) are considered to be the features for the model?

The top 10 Features for the model are visualized in the plot below:

<br>

<p align=center>
<img src=Images/importance_top_ten.png>

## 3. What variable(s) are neither targets nor features, and should be removed from the input data?

The 'EIN', 'NAME', 'STATUS' and 'SPECIAL_CONSIDERATION' columns are neither targets nor features and were removed before we trained the model.

<br>

## 4. How many neurons, layers, and activation functions did you select for your neural network model, and why?

In the first optimized layer there were a selected 80, followed by 50, and lastly, 30. A total of three layers were used with "relu" as the activation function. All in an effort to reach the models targeted performance.

<br>

<p align=center>
<img src=Images/neurons_layers.png>

## 5. Were you able to achieve the target model performance?

Yes, an accuracy of 78% was achieved when we ran our random forest model.

<br>

<p align=center>
<img src=Images/D3_3_accuracy_random_forest.png>

## 6. What steps did you take to try and increase model performance?

- The 'EIN', 'NAME', 'STATUS' and 'SPECIAL_CONSIDERATION' columns were dropped and two hidden layers were added and an accuracy of 72.55%.

<br>

<p align=center>
<img src=Images/D3_1_accuracy.png width=800>

- Changed activation functions to "sigmoid" and binned lower occurrence values and our model came back with a accuracy of 74%.

<br>

<p align=center>
<img src=Images/D3_2_accuracy.png width=800>

- Finally, the "NAME" feature was binned into an other category for all values <= 5 and the RandomForestClassifier showed an accuracy of 78% as pictured in question 5 above.

<br>

## Summary::

I recommend a random forest model to solve this classification problem. I ran a random forest model which is quicker and more efficient at running large datasets as such and was able to achieve an accuracy of 78%.

## Resources:

- Data:

    -`charity_data.csv`

    -`UCF-VIRT-DATA-PT-06-2022-U-B-TTH-Module 19 Challenge`

<br>