# Metal_Detection_Sonar_Data
## Overview
* This machine learning project aims to train a model that can differentiate between sonar signals reflected off a metal cylinder and those reflected off a roughly cylindrical rock.
* The data consists of 60 features and a categorical target for each pattern, the features are obtained from sonar signals obtained from a variety of different aspect angles, spanning 90 degrees for the cylinder and 180 degrees for the rock.
* The labels associated with each record contain the letter "R" if the object is a rock and "M" if it is a mine (metal cylinder). The numbers in the labels are in increasing order of aspect angle, but they do not encode the angle directly.
* The project is implemented using Jupyter Notebook, Python, Sci-kit-learn, pandas, numpy, and matplotlib. The dataset is preprocessed then Sci-kit-learn is used to split the dataset into training and testing sets, standardize the data, and build and train the machine learning model.

## Objectifs
Overall, the project aims to provide an accurate and efficient method for detecting metal on the seafloor using sonar data, which can be applied to real-world situations.

## Techologies used in this project:
* Python
* Jupyter Notebook
* Sci-kit-learn
* Pandas
* Numpy
* Matplotlib

## Procedure
After the conditioning and preprocessing of the data, we tested several machine learning models in order to evaluate their performance and choose the best performing model to be used for our project, the tested models are the following:
* Logistic Regression
* K-Nearest-Neighbors
* Support Vector Machine (SVM)
* Random Forest
* Artificial Neural Network (MLP)

After the evaluation of each model and the tuning of the hyper parameters, we moved forward with the Artificial Neural Network algorithm "Multi Layer Perceptron" using the following hyper parameters:
* activation': 'relu'
* hidden_layer_sizes : (100, 100)
* solver': 'adam'
* max_iter: 1200
* learning_rate: 'constant'
* alpha: 0.0001

## Results: after the deep evaluation of our model we obtained the following scores
* Accuracy: 86%
* Precision: 87%
* Recall: 86%
* f1-score: 86%
