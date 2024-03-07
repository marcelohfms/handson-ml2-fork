# How would you define Machine Learning?
Machine Learning is a programming technique that allows computers to learn from example instead of explicitly programming rules to be followed.

# Can you name four types of problems where it shines?
Machine Learning can be used:
* When the rules are too complex for them to be programmed explicitly
* When rules might change over time
* When there is a complex problem with a huge amount of data available
These might include, but not be restricted to: email spam detection, clustering, image/sound recognition, predicting classes/values based on previous data

# What is a labeled training set?
It is a set of data in which the instances (or samples) have a corresponding result that wants to be guessed for new data.

# What are the two most common supervised tasks?
Regression, in which we want to predict a number (value) and Classification, in which we predict a class or category.

# Can you name four common unsupervised tasks?
Clustering, anomaly/novelty detection, association rules and visualization and dimensionality reduction.

# What type of Machine Learning algorithm would you use to allow a robot to walk in various unknown terrains?
Reinforcement learning. We reward or punish an action and let the robot learn from experience which path leads to the desired result.

# What type of algorithm would you use to segment your customers into multiple groups?
Clustering algorithms, such as K-Means, DBSCAN or Hierarchical Cluster Analysis (HCA).

# Would you frame the problem of spam detection as a supervised learning problem or an unsupervised learning problem?
Supervised learning. We need to know first what category each email falls into (spam or ham) before being able to guess the category for new emails.

# What is an online learning system?
It is a system that learns continuously with new data and doesn't need to be retrained on the full dataset.

# What is out-of-core learning?
It is a system that learns "online" from a full dataset but in chunks. It is not actually online because the data has already been collected, but the dataset is so large that it needs to be chunked so that we have enough memory to fit in the machine's main memory. It can be thought as "incremental learning".

# What type of learning algorithm relies on a similarity measure to make predictions?
The instance-based algorithms. One example is kNN(k-Nearest Neighbors). The counterpart of this type would be model-based algorithms.

# What is the difference between a model parameter and a learning algorithm's hyperparameter?
A model parameter is (one of) the found value(s) for the model that minimizes the cost function (or maximizes a utility function). A learning algorithm's hyperparameter is applied to control the regularization of the learning.

# What do model-based learning algorithms search for? What is the most common strategy they use to succeed? How do they make predictions?
Model-based learning algorithms search for parameters that are used to estimate a function that describes the problem mathematical model. The most common strategy used is the optimization of a cost function. They make predictions by applying these parameters to a function along with the features of new data and thus getting back a prediction.

# Can you name four of the main challenges in Machine Learning?
* Unrepresentative data
* Insufficient data
* Model overfitting and underfitting
* Poor quality data

# If your model performs great on the training data but generalizes poorly to new instances, what is happening? Can you name three possible solutions?
The model is overfitting. You could try regularizing the model through hyperparameters, choosing a different learning algorithm, reducing the number of attributes used to train or getting better quality data to train the model (i.e. removing outliers or fixing data errors)

# What is a test set and why would you want to use it?
It is a chunk of data that is used to evaluate the generalization error of the trained model. We would want to use it because if the model is trained on the full dataset, we would be unable to know if the model is overfitting or not.

# What is the purpose of a validation set?
A validation set is used to make sure that the trained model isn't simply the best model trained for that specific test set, but the best model overall.

# What can go wrong if you tune hyperparameters using the test set?
You might produce the best model for that particular test set.

# What is repeated cross-validation and why would you prefer it to using a single validation set?
Using many validation set, evaluating the model once per validation set, after it is trained on the rest of the data and then averaging out all the evaluations of a model, so we get a much more accurate measure of its performance. Its drawback is that it requires a lot more training time.
