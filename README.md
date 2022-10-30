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

### Benefits and challenges of random forest

There are a number of key advantages and challenges that the random forest algorithm presents when used for classification or regression problems. Some of them include:

### Key Benefits

##### Reduced risk of overfitting:

Decision trees run the risk of overfitting as they tend to tightly fit all the samples within training data. However, when there’s a robust number of decision trees in a random forest, the classifier won’t overfit the model since the averaging of uncorrelated trees lowers the overall variance and prediction error.

##### Provides flexibility: 

Since random forest can handle both regression and classification tasks with a high degree of accuracy, it is a popular method among data scientists. Feature bagging also makes the random forest classifier an effective tool for estimating missing values as it maintains accuracy when a portion of the data is missing.

##### Easy to determine feature importance:

Random forest makes it easy to evaluate variable importance, or contribution, to the model. There are a few ways to evaluate feature importance. Gini importance and mean decrease in impurity (MDI) are usually used to measure how much the model’s accuracy decreases when a given variable is excluded. However, permutation importance, also known as mean decrease accuracy (MDA), is another importance measure. MDA identifies the average decrease in accuracy by randomly permutating the feature values in oob samples.

### Key Challenges

##### Time-consuming process: 

Since random forest algorithms can handle large data sets, they can be provide more accurate predictions, but can be slow to process data as they are computing data for each individual decision tree.

##### Requires more resources: 

Since random forests process larger data sets, they’ll require more resources to store that data.

##### More complex: 

The prediction of a single decision tree is easier to interpret when compared to a forest of them.

### Random forest applications

The random forest algorithm has been applied across a number of industries, allowing them to make better business decisions. Some use cases include:

##### Finance: 

It is a preferred algorithm over others as it reduces time spent on data management and pre-processing tasks. It can be used to evaluate customers with high credit risk, to detect fraud, and option pricing problems.

##### Healthcare: 

The random forest algorithm has applications within computational biology (link resides outside IBM) (PDF, 737 KB), allowing doctors to tackle problems such as gene expression classification, biomarker discovery, and sequence annotation. As a result, doctors can make estimates around drug responses to specific medications.

##### E-commerce: 

It can be used for recommendation engines for cross-sell purposes.
