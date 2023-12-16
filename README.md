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
Here I faced problem with number of target value. NeuralFCA can solve only binary classification prblem, so I picked the least class and dropped it with every row. Other features I binarized by their mediane value and then dropped following features for better time performance -- 'Nonflavanoid_phenols', 'Malicacid', 'Ash', 'Alcalinity_of_ash'. Then I choosed top-7 concepts and build NN using them. After training it looks like this: 
[Wine](https://github.com/d1scob4ll/OSDA/tree/main/Big_HW/Wine.png?raw=true)
## Second dataset: Wine_quality
### Description
Dataset contains information about the chemical composition red wine. Target feature here is quality of wine rated from 1 to 10.
### Preprocessing
Problem with binarization of target feature I solved similarly with other features -- just picked mediane value and binarized all of them by it. For dropping I choose 'free_sulfur_dioxide', 'pH', 'sulphates'. Then I choosed top-7 concepts and build NN using them. After training it looks like this: 
[Wine_quality](https://github.com/d1scob4ll/OSDA/tree/main/Big_HW/Wine_quality.png?raw=true)
## Second dataset: Adult
### Description
Dataset contains various information about USA citizens, like their age, sex, marital status, race, occupation and etc. Target here is to define whether their year sallary more than 50k$ or not.
### Preprocessing
For categorical features I decided to choose mode of every feature and binarize by it. For every numerical feature approach is the same, as with the other datasets -- just picked mediane value. For dropping I choose 'race', 'marital-status'. Then I choosed top-10 concepts and build NN using them. After training it looks like this: 
[Adult](https://github.com/d1scob4ll/OSDA/tree/main/Big_HW/Adult.png?raw=true)
