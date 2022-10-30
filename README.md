# Random-Forest

Random forests or random decision forests is an ensemble learning method for classification, regression and other tasks that operates by constructing a multitude of decision trees at training time

### Working of Random Forest Algorithm

Before understanding the working of the random forest we must look into the ensemble technique. Ensemble simply means combining multiple models. Thus a collection of models is used to make predictions rather than an individual model.

Ensemble uses two types of methods:

#### 1. Bagging–

It creates a different training subset from sample training data with replacement & the final output is based on majority voting. For example,  Random Forest.

#### 2. Boosting– 

It combines weak learners into strong learners by creating sequential models such that the final model has the highest accuracy. For example,  ADA BOOST, XG BOOST

![image](https://user-images.githubusercontent.com/109084435/198887716-5095a3e2-b3a5-48af-917f-df6b1e7c2dd3.png)

As mentioned earlier, Random forest works on the Bagging principle
 
### Bagging

Bagging, also known as Bootstrap Aggregation is the ensemble technique used by random forest. Bagging chooses a random sample from the data set. Hence each model is generated from the samples (Bootstrap Samples) provided by the Original Data with replacement known as row sampling. This step of row sampling with replacement is called bootstrap. Now each model is trained independently which generates results. The final output is based on majority voting after combining the results of all models. This step which involves combining all the results and generating output based on majority voting is known as aggregation.

![image](https://user-images.githubusercontent.com/109084435/198887821-a1a1bac6-e10d-4cfa-8d57-83540a501a48.png)

![image](https://user-images.githubusercontent.com/109084435/198887914-d2d6b83a-c699-4da3-8328-a56586c2dea9.png)

### Steps involved in random forest algorithm:

##### Step 1: 

In Random forest n number of random records are taken from the data set having k number of records.

##### Step 2: 

Individual decision trees are constructed for each sample.

##### Step 3:

Each decision tree will generate an output.

##### Step 4: 

Final output is considered based on Majority Voting or Averaging for Classification and regression respectively.

### Important Features of Random Forest

##### 1. Diversity-

Not all attributes/variables/features are considered while making an individual tree, each tree is different.

##### 2. Immune to the curse of dimensionality-

Since each tree does not consider all the features, the feature space is reduced.

##### 3. Parallelization-

Each tree is created independently out of different data and attributes. This means that we can make full use of the CPU to build random forests.

##### 4.  Train-Test split- 

In a random forest we don’t have to segregate the data for train and test as there will always be 30% of the data which is not seen by the decision tree.

##### 5.  Stability- 

Stability arises because the result is based on majority voting / averaging.
