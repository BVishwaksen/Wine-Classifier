# Wine-Classifier
A machine learning based system that can be used to predict the class of wines grown in the same region in Italy but derived from three different cultivars.
## Table of Contents
[Introduction](#Introduction)
[Requirements](#Requirements)
[How-To-Use](#How-To-Use)
[Dataset](#Dataset)
[Technical-Details](#Technical-Details)
[Algorithm](#Algorithm)
[Lisence](#Lisence)
### Introduction
All the wines are not same.The contents of wine may be same but we can classify them based on their composition mixture and their geographic locations.Here we are only dealing only with the composition mixture ratio but we are not taking the geographical location into condsideration. To classify a wine we neeed to perform critical analysis. But manual analysis is not reliable when compared to system analysis. So the main objective of the project is to design a machine learning model that can classify wines.
### Requirements
Python 3.5 or above version with numpy,pandas,matplotlib,scikit-learn and pickle packages.
Jupyter lab/Jupyter notebook
No specific hardware requirements and runs on any operating system
### How-To-Use
After downloading and extracting the repository open it in jupyter notebook.Then open the `wine_class_predictor.ipynb` file. In that file change the values of `wine_report` variable.
The order of the values are `'alcohol','malic_acid','ash','alcalinity_of_ash','magnesium','total_phenols','flavanoids','nonflavanoid_phenols','proanthocyanins','color_intensity','hue','od280/od315_of_diluted_wines','proline'` and then run all the cells.The class of wine is displayed as the output of the last cell.

### Dataset
The dataset used in this project is wine dataset from scikit learn dataset library.
It can be loaded as `sklearn.datasets.load_wine()`
### Technical-Details
##### Dataset Details
The dataset contains 13 attributes and 178 instances.
The column details are
 'alcohol',
 'malic_acid',
 'ash',
 'alcalinity_of_ash',
 'magnesium',
 'total_phenols',
 'flavanoids',
 'nonflavanoid_phenols',
 'proanthocyanins',
 'color_intensity',
 'hue',
 'od280/od315_of_diluted_wines',
 'proline'
##### Files Organization
The project is implemented in python in Jupyter Notebook environment.It mainly contains two parts.The `wine_class_trainer.ipynb` is for training the data and the `wine_class_predictor.ipynb` is to load the trained data and to predict results.The `wine_model.sav` is the model that is saved.
### Algorithm
The Wine-Classifier is a classification problem.As here there are more than two types of target values this comes under `multinominal classification`.
The algorithm used in this is `Naive Bayes`.More details about this algorithm can be found at <https://en.wikipedia.org/wiki/Naive_Bayes_classifier>
### Lisence
This is a public repository and you can be used in research,commercial and non-commercial applications without any restrictions.
