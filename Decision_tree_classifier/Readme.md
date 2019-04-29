# Assignment 2

In this assignment you will be implementing your own decision trees. 

  * Build a **decision tree classifier** from the given training data set. Then, apply it on the test set and submit your code to generate predictions.
      - You need to build the decision tree classifier **from scratch**. (I.e., it is not allowed to use existing machine learning libraries or packages such as sklearn.)
      - You may use any programming language/environment of your choice, but you are required to submit the complete source code to produce the output 
        - If you use anything other than jupyter notebook, submit an executable and run that from the main function of the jupyter notebook so that the prediction generation is automated. We can provide assistance with this.
      - The output (a single file with the predictions for each test instance) **must be generated automatically using the decision tree approach implemented by you**. Submitting predictions/code from any other source (Internet, another student, etc.) is considered cheating and will result in immediate disqualification (i.e., dismissal from the course).   
      - You may assume the test data is present data/housing_price_test.csv on autograder.
      - The autograder will automatically run your jupyter notebook ([this notebook](Decision_tree.ipynb)) to generate the predictions in a file called "submission.csv" and the autograder script will compute a score automatically. So you are not required to upload the submissions file but rather the code to generate the submissions file.
      - In order to pass this assignment, you need to reach a **Score of at least 70%** in autograder. This will be computed based on the Root Mean Square Error w.r.t to the test data.
      - A skeleton of a possible implementation in Python for an example dataset is made available in [this notebook](Decision_tree.ipynb).
      - Deadline for the assignment is 25.02.2019 by 23.59 CET.

* Dataset:
  - The dataset is taken from an ongoing [Kaggle competition](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
  - Optionally feel free to submit to the Kaggle competition
  - The dataset is for housing price prediction. Dataset description is found [here](data/data_description.txt)
    - The goal is predict the price of a house given its attributes
    - So it is a regression problem
    - Therefore your decision tree should be able to predict a value (housing price) rather than a class
    - Use appropriate splitting criterion and error function
    - The dataset has a lot of missing values denoted as NaN you may replace them with appropriate categorical value like None or mean/mode approrpiately.
    - You may also apply dimensionality reduction like PCA before training.
    - At the leaf node you may use the average value as the predicted value or if there are many instances you may use additional classifiers like linear regression.
    
  - The performance is evaluated using RMSE [Root Mean Square Error](https://en.wikipedia.org/wiki/Root-mean-square_deviation)
  - Training data set is [here](data/housing_price_train.csv)
  - Test data is [here](data/housing_price_test.csv)
