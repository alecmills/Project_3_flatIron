# Project_3_flatIron
To Start the professional notebook I started with EDA. Took a first look into the data set and went through all of the charges to find out the mean charges of the churned data and the charges of the non churned data. We would that the churned data was charge more money and could be a reason that they left. Nexted looked at the international plans and also compared the data between the two data frames of churned and non churned. Didnt find to much correlation other than almost half of the data in international churns. Next looked into voicemail plan and found that not a ton of people were in the dataset for voicemail. But of the poeple that were the majority of them stayed.

Next is model creation, Started by making a simple dummy model. Also set up a pipe system to run through mulitple models at one time. Next was a Logistic Regression Model. This model only very slightly preformed better than that of the dummy model. However my RAndom Forest model preformed a lot better and with a 94% accuracy score. My Gradient booster model also scored the same as the Random Forest model.

After using grid search and smote to look into the target imbalance I  found my final model and came out to be another Random Forrest model with the paramaters of min_samples_leaf=1,max_features= 'auto', min_samples_split= 2, criterion='entropy', random_state=42). and this model preformed with a 95% accuracy score.

To conclued I would be able to predict if a customer would churn or not with a recall score of 73%.
