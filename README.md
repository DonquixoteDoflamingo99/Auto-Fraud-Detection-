# Auto-Fraud-Detection-

Story
Considering the magnitude of the consequences, insurance fraud is a particularly difficult problem to solve. Because of the financial burden that fraud places on insurance providers, premiums for drivers may rise. When it comes to vehicle insurance claims, the manual review procedure entails hiring highly trained fraud examiners, which is not only expensive but also inefficient in the face of rising insurance claims volumes.


Problem
An issue that an insurance company faces is identifying false claims that are associated with accidents. They intend to design a fraud detection algorithm that can automatically identify fraudulent claims for vehicle insurance and then manage them in a manner that allows human fraud analysts to decide whether or not the claim should be approved or denied after reviewing it.
Auto insurance fraud encompasses a wide range of illegal activities, including but not limited to the following: falsifying facts on insurance applications; filing false reports of stolen vehicles, nonexistent injuries, or damage; fabricating accidents; and filing claim forms for incidents that never occurred.


For training and evaluating the model performance I have used the following steps.
1.	The first thing was to change the datatypes of categourcal variables to object from int.
2.	Split numerical and categorical variables, dropping numerical variables with correlation >0.8.
3.	Encoding the character data.
4.	Splitting the training data into train and validation sets and stratifying the dependent variable.
5.	Initiating model, I used Random Forest Classifier and XGBoost.
6.	Fitting the training data and making predictions using validation data, and generating classification report.
7.	Using Randomized Search CV to optimize the parameters and using the model with best parameters to fit the training seta again.
8.	Now to optimize the model, I eliminated the unimportant features and trained the model again.
9.	Used the validation set to validate the performance of the model.
10.	Here there is a class imbalance so judging the model only by the Accuracy will be a bad idea, we need the F1 score as well as the AUC because they are the unbiased measures here.
11.	Used the test set to predict the values and again checked the performance of the model.

