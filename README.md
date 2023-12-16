# Description
This repository contain big homework for OSDA and first task from fourth homework.
# Big homework description
For big homework I choose these datasets: Wine, Wine_quality, Adult. Result of classification by NeuralFCA is:
Dataset | Wine | Wine_quality | Adult | 
--- | --- | --- | --- |
F1-Score | 0.92 | 0.79 | 0.66 | 
## First dataset: Wine
### Description
Dataset contains information about the chemical composition of three types of wine. Target feature here is origin of wine, which contains of three classes.
### Preprocessing
Here I faced problem with number of target value. NeuralFCA can solve only binary classification prblem, so I picked the least class and dropped it with every row. Other features I binarized by their mediane value and then dropped following features for better time performance -- 'Nonflavanoid_phenols', 'Malicacid', 'Ash', 'Alcalinity_of_ash'. Then I choosed top-7 concepts and build NN using them. After training it look like this: 
[alt text](https://github.com/d1scob4ll/OSDA/tree/main/Big_HW/Wine.png?raw=true)
