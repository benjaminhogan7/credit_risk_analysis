# credit_risk_analysis

## Overview
This project was to use a credit card dataset from LendingClub, a p2p lending company to identify key risk features and to predict instances of real-world credit card risk using supervised machine learning. The dataset and type by nature is unbalanced. To account for this a variety of methods had to be used to train and evaluate the models. I used oversampling, SMOTE, undersampling, ClusterCentroids, SMOTEEN, BalancedRandobForestClassifer, and EastEnsembleClassifier.


## Results

### Deliverable 1

In this deliverable, the three required methods proved to be lackluster in their accuracy

* RandomOverSampler - Random Oversampling

<img width="782" alt="Screen Shot 2022-12-12 at 8 32 13 PM" src="https://user-images.githubusercontent.com/108236450/207204143-96d5736d-4a08-4ce0-bc46-e7f02b1134bf.png">


* SMOTE Oversampling

<img width="759" alt="Screen Shot 2022-12-12 at 8 32 32 PM" src="https://user-images.githubusercontent.com/108236450/207204175-61bb1233-5ec0-4db9-80ad-629319f342cf.png">


* RandomUnderSampler - Undersampling

<img width="755" alt="Screen Shot 2022-12-12 at 8 32 50 PM" src="https://user-images.githubusercontent.com/108236450/207204220-4fe8c282-6101-47a9-b7dd-87ec3f427309.png">


### Deliverable 2

Using SMOTEEN to over and then undersample, too proved to have low accuracy

* Combination (Over and Under) Sampling - SMOTEEN

<img width="769" alt="Screen Shot 2022-12-12 at 8 33 15 PM" src="https://user-images.githubusercontent.com/108236450/207204269-ecc15075-ba2e-4272-b9ab-9400192e20bd.png">

### Deliverable 3

Using the Balanced Random Forest Classifier, the accuracy increased significantly. With Easy Ensemble AdaBoost Classifier the accuracy of the model increased to a usable value: 93%

* BalancedRandomForestClassifier - Ensemble Learners

<img width="773" alt="Screen Shot 2022-12-12 at 8 34 41 PM" src="https://user-images.githubusercontent.com/108236450/207204439-47777d43-1308-4515-8db7-1f5c21f83c9e.png">

* Easy Ensemble AdaBoost Classifier

<img width="768" alt="Screen Shot 2022-12-12 at 8 36 24 PM" src="https://user-images.githubusercontent.com/108236450/207204647-a5f74ed0-3c6e-4083-bfcd-1c84a6dbd68e.png">

## Summary

As mentioned previously, 5 out of the 6 models used did not return results that I found usable. If I had to recommend one, it would be Easy Ensemble Adaboost Classifier. This returned an accuracy of 93%. I did also find that the Balanced Random Forest Classifier was interesting in that it allowed for me to output the most important features for the model. If used in tandem, it could be a way to reduce the amount of data required for predictions of this type and speed up calculations. In some instances, it could also reduce the necessary paperwork and data entry for customers and increase customer satisfaction and conversion.

In general, while there are models that I wouldn't put into production for this use case, it was helpful to see the different types ways to model the machine learning and compare the outputs.


