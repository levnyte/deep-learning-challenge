# Report
<ins>Overview</ins>

The purpose of this analysis is to determine which machine learning algorithm will produce the most accurate binary classifier.  The following algorithms were used:

* a neural Network with two hidden layers,
* a neural Network with three hidden layers,
* a decision tree,
* and a random forest classifier.

<ins>Results</ins>

*  Data Preprocessing
	*  The IS_SUCCESSFUL column is the target for the model.
	*  APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT are the features for the model.
	*  EIN and NAME are neither targets nor features so they are removed.

*  Compiling, Training, and Evaluating the Model
	*  The neural network model has two hidden layers with 70 neurons on the first layer, and 20 neurons on the second layer.  Those numbers were suggested by the instructor.  The rectified linear unit (ReLU) is used in the hidden layers because it is computationally efficient.  Sigmoid is used in the output layer because it is commonly used for binary classification where the output is interpreted as a probability.
	*  The original neural network had an accuracy score of 72.93 percent, falling short of the target of 75 percent.
	*  I first attempted to optimize the neural network by adding a third hidden layer.  When it failed to reach the target, I experimented with the number of neurons in each layer and used different activation functions.  This produced a similar accuracy score of 72.82 percent.  I later tried a decision tree and a random forest classifier.  They produced accuracy scores of 70.75 percent and 71.02 percent respectively.

<ins>Summary</ins>

The algorithms used in this analysis could only produce accuracy scores that are shy of the target model performance of 75 percent.  The common factors of this performance are the preprocessing, and mainly the dataset itself.  While keeping the target and feature columns the same, I would suggest collecting more data over time then run the algorithm again to see if the accuracy score increases.

# Reference
edX. "Module 21 Challenge." 15 February 2024, bootcampspot.instructure.com/courses/4916/assignments/61922?module_item_id=1077730.