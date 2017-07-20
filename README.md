# blood_donors
A classification problem based on information of blood donors, which is a competition dataset from drivendata.org. Drivendata.org focuses on machine learning competitions for non-profits, and the goal of this competition is to find the probability that a given donor will donate in the coming month. The performance metric is the log-loss function.

The dataset has a slight class imbalance at about a 3:1 ratio. Two of the features are multiples of each other, and most of the features are correlated with each other. The file blood_comp.ipynb contains my entire workflow from exploratory data analysis to model selection and hyperparameter tuning to the final prediction to be submitted to the competition.

Logistic regression and support vector machine were the most reliable models. However, a particular instance of a multi-layered neural network yielded the best score for the competition, but it was likely a bit overfitted and probably would not generalize as well to other unseen data.

The end result was a log-loss of around 0.44, which yielded placed 82nd out of 3019 competitors.
