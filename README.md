# Insights from hosuing Data
Predict the probability that a customer would buy a quoted insurance plan
Home Site Quite Conversion Challenge
Before asking someone on a date or skydiving, it's important to know your likelihood of success. The same goes for quoting home insurance prices to a potential customer. Homesite, a leading provider of homeowners insurance, does not currently have a dynamic conversion rate model that can give them confidence a quoted price will lead to a purchase.

Using an anonymized database of information on customer and sales activity, including property and coverage information, Homesite is challenging you to predict which customers will purchase a given quote. Accurately predicting conversion would help Homesite better understand the impact of proposed pricing changes and maintain an ideal portfolio of customer segments.

Main Challenges
This dataset was huge ~260K rows( aka samples) and 298 (features) and to add to that challenge the data was anonymized so doing feature engineering would be very random and usually brute force . I though of handeling this via feature selection and boosting methodology

I implemented two feature selection stratergies

(1) Experiment with SMOTE (or its variations) using different percentages to get a higher accuracy on minority class prediction.

(2) Perform ensemble predictions (one-layer stacking) by combining predictions from the various algorithms. For stacking, try at least five different models - e.g. decision tree, random forest, support vector machines, multilayer perceptron and K-nearest neighbors.

(3) In addition, perform hyperparameter tuning on the stacked model. You can do hyperparameter tuning on individual models 
