# Frame the problem
* What is exactly the business objective? How does the company expect to use and benefit from this model?
* What algorithms will you select? What performance measure will you use? How much effort should we spend tweaking it?
* What does the current solution look like (if there is any)?
* Is it supervised, unsupervised or Reinforcement learning? Is it classification, regression or something else? Should we use batch learning or online learning?

### Our current problem: housing median prices for districts
* Supervised: we have labeled data for some districts
* Regression: we are predicting the housing median price: a number/value
* Batch learning: the data has already been collected. There is no continuous flow of data coming in the system and no need to adjust to changing data rapidly. Also, the data is small enough to fit in memory.

# Select a performance measure
* RMSE
* MAE (if there are multiple outliers)
RMSE is more sensitive to outliers, but when outliers are exponentially rare (like in a normal curve), the RMSE performs very well.

# Check the Assumptions
Is that what we really need? Is the problem correctly defined?

# Get the Data
* Download
* Take a quick look
* Create a test set -> random sampling vs stratified sampling

# Discover and Visualize Data to Gain Insights
* Set aside test set. If dataset is too big, sample an exploration set to make manipulations faster.




