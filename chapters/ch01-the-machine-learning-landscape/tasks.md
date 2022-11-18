## Exersice solutions for Chapter 01

### 1.
**Q:**
How would you define Machine Learning?

**A:** 
The study of how computers can learn things without explicitly being programmed to do so.

### 2.
**Q:**
Can you name four types of problems where it shines?

**A:**
* natural language processing
* image segmentation
* text summarization
* recommending videos

### 3.
**Q:**
What is a labeled training set?

**A:**
Set of things where we have the true answer to the questions we ask the model.

### 4.
**Q:**
What are the two most common supervised tasks?

**A:**
Classification and regression.

### 5.
**Q:**
Can you name four common unsupervised tasks?

**A:**
Clustering, data visualization, anomaly detection, dimensionality reduction.

### 6.
**Q:**
What type of Machine Learning algorithm would you use to allow a robot to walk in various unknown terrains?

**A:**
Reinforcement learning.

### 7.
**Q:**
What type of algorithm would you use to segment your customers into multiple groups?

**A:**
Clustering algorithm

### 8.
**Q:**
Would you frame the problem of spam detection as a supervised learning problem or an unsupervised learning problem?

**A:**
Its a classification problem which tend to be supervised learning problems.  

### 9.
**Q:**
What is an online learning system?

**A:**
A learning system that changes its policy with new data without retraining. 

### 10.
**Q:**
What is out-of-core learning?

**A:**
Learning on data that cannot fit in memory. It is trained on one portion of the data, then on the next and so on.

### 11.
**Q:**
What type of learning algorithm relies on a similarity measure to make predictions?

**A:**
Instance based learning.

### 12.
**Q:**
What is the difference between a model parameter and a learning algorithm’s hyperparameter?

**A:**
One learning algorithm can be used in many different models. The model parameters refer to how the model is structured, i.e. what things it can learn. The hyperparameters are about how the model learns, (i.e how fast, should it stop if it hasn't been learning anything in a while). 

### 13.
**Q:**
What do model-based learning algorithms search for? What is the most common strategy they use to succeed? How do they make predictions?

**A:**
They search for patterns, emerging from the data.  

### 14.
**Q:**
Can you name four of the main challenges in Machine Learning?

**A:**
* Having representative data
* Having relevant features for the task
* Fitting the data correctly
* Having enough quantity and good quality of data

### 15.
**Q:**
If your model performs great on the training data but generalizes poorly to new instances, what is happening? Can you name three possible solutions?

**A:**
Then the model has probably overfitted the data. Then we can pick a simpler model or reduce the learning rate or contrain the model in some way.

### 16.
**Q:**
What is a test set, and why would you want to use it?

**A:**
A test set is used for measuring performance of the model. It is a portion of the data we have that we don't show the model when training but use it to see how it would perform in a real-world scenario. We have to make the test set representative of the whole data we have in order to have as accurate results as we can. 

### 17.
**Q:**
What is the purpose of a validation set?

**A:**
As the test set is used too much, it is possible to overfit it. Thats why we use another portion of the available data to measure the performance of the model iteratively. Doing this enough times, when finally we are satisfied with the results, we evaluate yet again on the test set, which the model hasn't seen but neither has it been evaluated on.

### 18.
**Q:**
What is the train-dev set, when do you need it, and how do you use it?

**A:**
Train-dev set is a set of data we use during training iterations of the model. Using two disjoint subsets we train on one and evaluate on another in order to see how the model performs. If we're not satisfied then we change the model a bit, referencing the wrong infers, pick two new disjoint subsets and the process repeats.

### 19.
**Q:**
What can go wrong if you tune hyperparameters using the test set?

**A:**
Fine tuning on the test set is a bad idea because then we would have great statistical results about the expected model performance but poor real-life one. This is the result of overfitting the test set.