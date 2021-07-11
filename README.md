# Credit_Risk_Analysis
#Overview of the analysis: Explain the purpose of this analysis.

This analysis is based on the models crerated using different machine learning algorithms (Logistic regression with different sampling techniques, Ensemble Learners) that has been used. 

#Results: 

##Logistic regression with Oversampling (using RandomOverSampler from imblearn)


	- The accuracy of the model to predict a high risk loan is 64% based on the score recieved. 
	- Precision is around 69%~ (70/ (70+31) = 0.69) which is nothing but model is correct 69% of the time.
	- Recall is around 1% (70/(70+6813) = 0.01) which is nothing but model identifies 1% of High risk loans.

https://github.com/asitkumar26/Credit_Risk_Analysis/blob/main/LogisticRegression-RandomOverSampler.png


##Logistic regression with Oversampling (using SMOTE from imblearn)

	- The accuracy of the model to predict a high risk loan is 66% based on the score recieved. 
	- Precision is around 63%~ (64/ (64+37) = 0.63) which is nothing but model is correct 63% of the time.
	- Recall is around 1% (64/(64+5291) = 0.01) which is nothing but model identifies 1% of all loans as High risk loans.

https://github.com/asitkumar26/Credit_Risk_Analysis/blob/main/LogisticRegression-SMOTE.png

##Logistic regression with Undersampling (using ClusterCentroids from imblearn )

    - The accuracy of the model to predict a high risk loan is 54% based on the score recieved. 
	- Precision is around 69%~ (70/ (70+31) = 0.69) which is nothing but model is correct 69% of the time.
	- Recall is around 0.6% (70/(70+10340) = 0.006) which is nothing but model identifies 0.6% of all loans as High risk loans.

https://github.com/asitkumar26/Credit_Risk_Analysis/blob/main/LogisticRegression-ClusterCentroids.png



##Logistic regression with Combination Sampling(using SMOTEENN from imblearn)

    - The accuracy of the model to predict a high risk loan is 64% based on the score recieved. 
	- Precision is around 72%~ (73/ (73+28) = 0.72) which is nothing but model is correct 72% of the time.
	- Recall is around 0.9% (73/(73+7412) = 0.009) which is nothing but model identifies 0.9% of all loans as High risk loans.


https://github.com/asitkumar26/Credit_Risk_Analysis/blob/main/LogisticRegression-SMOTEEN.png


##Balanced Random Forest Classifier from imblearn

    - The accuracy of the model to predict a high risk loan is 78% based on the score recieved. 
	- Precision is around 70%~ (71/ (71+30) = 0.70) which is nothing but model is correct 70% of the time.
	- Recall is around 3%~ (71/(71+2153) = 0.031) which is nothing but model identifies 3% of all loans as High risk loans.


https://github.com/asitkumar26/Credit_Risk_Analysis/blob/main/BalancedRandomForest.png


##Easy Ensemble AdaBoost Classifier

    - The accuracy of the model to predict a high risk loan is 93% based on the score recieved. 
	- Precision is around 92%~ (93/ (93+8) = 0.92) which is nothing but model is correct 92% of the time.
	- Recall is around 8%~ (93/(93+1017) = 0.083) which is nothing but model identifies 8% of all loans as High risk loans.
	
https://github.com/asitkumar26/Credit_Risk_Analysis/blob/main/EasyEnsembleAdaboost.png




#Summary: 

Among all the models, based on accuracy of predictions, precision and recall...the best performed model is
	- the one which is created using Adaboost Classifier algorithm, because 93% score on predictions is quite acceptable one in this case. This model predicts correctly 92% of time which is
	  the precision value. Among all models also this one predicts highest number of high risk loans (recall is 8%).
