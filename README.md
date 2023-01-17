# credit-risk-sup-machine-learning


Overview:


The goal of the analysis was to use different supervised machine learning models to predict credit risk. We accomplished this by running models that were trained on real credit risk data. We then compared the predictions of these models to actual outcomes to see how accurate our algorithm was at predicting. Because there is unbalanced outcomes, with good-loan outcomes much outnumbering bad-loan outcomes, we used different sampling techniques to bridge the gap.


Results:


Random Oversampling Results: Acc = 63% Rec=68% Spe=58%
![image](https://user-images.githubusercontent.com/112716673/212799163-b61a5e0a-3d2e-4b9e-9efb-6874c57d358f.png)

SMOTE Oversampling Results: Acc=63% Rec=63% Spe=62%
![image](https://user-images.githubusercontent.com/112716673/212799667-e72616d3-b570-40ed-908c-64513fe8d9f3.png)

ClusterCentroids Undersampling Results: Acc=53% Rec=45% Spe=61%
![image](https://user-images.githubusercontent.com/112716673/212799841-543dfba4-b49e-4524-aaea-30d564301e43.png)

SMOTEEN Sampling Results: Acc= 64% Rec=58% Spe=70%
![image](https://user-images.githubusercontent.com/112716673/212799973-eda6f0c7-bb60-484e-b644-6ac0bdef4030.png)

BalancedRandomForestClassifier Results: Acc= 79% Rec=91% Spe=67%
![image](https://user-images.githubusercontent.com/112716673/212800124-53bc679c-0407-448c-ab50-a1b30c8f8f37.png)

EasyEnsembleClassifier Results: Acc=93% Rec=94% Spe=91% 
![image](https://user-images.githubusercontent.com/112716673/212800265-2cff493f-d2d3-422a-a190-2589720d1d18.png)


Summary:


Looking at our results, we can see the the EasyEnsembleClassifier was by far the most accurate model at predicting loan outcomes. It had a total accuracy of 93%. With a recall of 94% it does a great job of detecting high risk loans. However, when looking at the decision matrix we can see that there is a sizeable number of samples (979/17118) that are predicted high-risk, when they actually are low. So although this model is not fool-proof, it is indeed the best model we came up with.
