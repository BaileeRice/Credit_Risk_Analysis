# Credit_Risk_Analysis

![image](https://user-images.githubusercontent.com/105184244/197450541-f140d924-4bb7-44e2-a692-b852849e1180.png)

OVERVIEW:

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. I'll be using imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

'Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk'.

OUTLINE:

-Step 1: Use Resampling Models to Predict Credit Risk

-Step 2: Use the SMOTEENN Algorithm to Predict Credit Risk

-Step 3: Use Ensemble Classifiers to Predict Credit Risk

---

RESULTS:

   **_Naive Random Oversampling_**

![image](https://user-images.githubusercontent.com/105184244/197461505-bd4662f8-638c-4128-8c65-e36af7a79058.png)

Balanced Accuracy: %64.7

Precision: low for High-risk loans, high for Low-risk loans

Recall Score: High-Low risk = .66/.67

   **_SMOTE Oversampling_**

![image](https://user-images.githubusercontent.com/105184244/197461664-3a0df21e-b4d5-4441-9023-8f9fcca7c9f0.png)

Balanced Accuracy: %62.5

Precision: low for High-risk loans, high for Low-risk loans

Recall Score: High-Low risk = .62/.67

   **_Undersampling_**

![image](https://user-images.githubusercontent.com/105184244/197461708-5a6612de-02b8-4521-bc57-429eede1f27d.png)

Balanced Accuracy: %52.1

Precision: low for High-risk loans, high for Low-risk loans

Recall Score: High-Low risk = .59/.46

   **_Combination Under-Over Sampling_**

![image](https://user-images.githubusercontent.com/105184244/197461743-2ed5ee8c-13d3-45e1-b271-19172039f928.png)

Balanced Accuracy: %62.5

Precision: low for High-risk loans, high for Low-risk loans

Recall Score: High-Low risk = .71/.54

   **_Balanced Random Forest Classifier_**

![image](https://user-images.githubusercontent.com/105184244/197462110-dc9e459b-7f5b-4016-a991-84b26e289f2a.png)

Balanced Accuracy: %78.7

Precision: low for High-risk loans, high for Low-risk loans

Recall Score: High-Low risk = .67/.91

   **_Easy Ensemble AdaBoost Classifier_**

![image](https://user-images.githubusercontent.com/105184244/197462132-294fb58f-abe6-4b3f-b6bd-200c30b3131d.png)

Balanced Accuracy: %92.5

Precision: low for High-risk loans, high for Low-risk loans

Recall Score: High-Low risk = .91/.94

---

SUMMARY:

Based off all the models ran, the **Easy Ensemble AdaBoost Classifier** shines above all the others with a %92.5 accuracy at detecting if someone is a low-credit risk, the next highest only having ~%78. None of the models hold well at determining whether someone is high-risk, that's something to take into account if what youre seeking is pinpointing high-risk individuals. 
