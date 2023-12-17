# Repository description
This repository contain big homework for OSDA and first task from fourth homework.
# Big homework description
For big homework I choose these datasets: Wine, Wine_quality, Adult. Result of classification by NeuralFCA and baselines is:
Model | Dataset | Accuracy | 
--- | --- | --- |
DecisionTreeClassifier | Wine | 0.96 | 
RandomForestClassifier | Wine | 0.96 | 
XGBClassifier | Wine | 0.97 | 
KNeighborsClassifier | Wine | 0.96 | 
LogisticRegression | Wine | 0.96 | 
**NeuralFCA** | Wine | 0.92 | 
DecisionTreeClassifier | Wine_quality | 0.73 | 
RandomForestClassifier | Wine_quality | 0.74 | 
XGBClassifier | Wine_quality | 0.74 | 
KNeighborsClassifier | Wine_quality | 0.72 | 
LogisticRegression | Wine_quality | 0.72 | 
**NeuralFCA** | Wine_quality | 0.79 | 
DecisionTreeClassifier | Adult | 0.63 | 
RandomForestClassifier | Adult | 0.63 | 
XGBClassifier | Adult | 0.63 | 
KNeighborsClassifier | Adult | 0.60 | 
LogisticRegression | Adult | 0.62 | 
**NeuralFCA** | Adult | 0.66 | 


For every dataset test size is 0.3.
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
