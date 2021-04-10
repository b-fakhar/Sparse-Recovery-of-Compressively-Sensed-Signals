# Data-Compression
### Project Objective 
The data explosion in the digital age has created a demand in proposing strategies to manage data acquisition, transmission and data storage. In this project, an optimization algorithm based on L0-minimization is develloped with the goal of: (1) improving the speed and quality recovery of the state-of-the-art MAX FS L0-minimization methods, and (2) improving the compression ratio of the well-known Compressive Sensing (CS) sparse recovery methods. 

### Challenges 
The newly developed classification algorithm is based on solution methods for the Maximum Feasible Subsystem (MAX FS) problem. The literature MAX FS algorithms are already known to give very high accuracy for binary classification. However, the state-of-the-art MAX FS algorithms have rarely been used and investigated in the literature since they are slow. Therefore, the main requirement is to increase their speed without loss of accuracy.

### Achievements
According to the experimental results, the introduced classification algorithm

- Provides better total accuracy compared to KNN, SVM, NB, and LR methods with and without hyperparameter tuning. 
- Improves the speed of the literature MAX FS classification methods by about 94% while improving the accuracy.
- Provides promising results for recall-oriented machine learning tasks such as disease diagnosis. 

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
###### Some details of the experimental setup are summarised in below. For more detail refer to our papers titled "A Faster MAXimum Feasible Subsystem Algorithm for Binary Classification" and " Faster Maximum Feasible Subsystem Solutions for Dense Constraint Matrices".

### Datasets
 Binary classification problems are derived from datasets in the UCI Repository of Machine Learning Databases https://archive.ics.uci.edu/ml/datasets.php. The following tables summarize the characteristics of the datasets used in two set of experiments (Scenario I and Scenario II). In the first scenario, the training set is identical to the entire dataset to compare with previous results of Chinneck's paper (https://pubsonline.informs.org/doi/abs/10.1287/ijoc.13.3.210.12632 ). In Scenario II, real-world medical and biological datasets for disease diagnosis are used. The task is to predict whether the patient has the disease (Class 1) or not (Class 0). The same folds are used throughout the implementation for all the models to ensure uniformity.

![ClassificationData](https://user-images.githubusercontent.com/59096353/114231621-a9c6b880-9948-11eb-9bc4-508e4ba45e78.png)

### Hyperparameter Tuning

Hyperparameter tuning is required to obtain best performance for some classifiers. For the methods that require hyperparameter tuning, two sets of results are reported: (1) default settings without hyperparameter tuning "Def", and (2) with hyperparameter tuning "Tune" ("Def" applies if unspecified). A recent study (Bahel et al. paper https://pubsonline.informs.org/doi/abs/10.1287/ijoc.13.3.210.12632), is considered here to select hyperparameter optimization methods and search ranges.

### Tools/Software
Python (Scikit-learn, Pandas, Seaborn, Matplotlib, and Plotly), MATLAB, MOSEK, Latex.
