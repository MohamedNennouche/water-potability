# Projet classification de l'eau potable
## But du projet
Le but de ce projet est de parvenir à mettre en place un modèle de classification binaire, on a dans notre dataset, trouvable sur Kaggle à [cette adresse](https://www.kaggle.com/adityakadiwal/water-potability) et donc au niveau du dataset on a 10 variables qui sont : 
- Le ph (ph)
- La dureté (Hardness)
- La solidité (Solids)
- La quantité de chloramines (Chloramines)
- La qualité de sulfate (Sulfate)
- La conductivité (Conductivity)
- La quantité de carbone organique (Organic_carbon)
- La quantité de trihalométhanes (Trihalomethanes)
- La turbidité (Turbidity)
## Structure du projet 
- water-notebook.ipynb : Le notebook Jupyter où le projet est fait
- water_potability : Fichier csv téléchargé de Kaggle contenant notre problème
## Quelques remarques 
- Le projet est un problème de classification binaire
- Il y a un certain nombre de lignes qui ne contiennent pas toutes les valeurs, la méthode choisie dans ce projet pour y remédier est de les supprimer car remarquant que leurs suppression impacte très peu la distribution globale des variables
## Pré-recquis logiciels 
Ce projet est fait à base de Python donc pour l'utilisation ou la copie de ce projet vous aurez besoin de : 
- Python 3.8 et + 

Les packages Python suivantes : 
- Numpy
- Matplotlib (et surtout le module pyplot)
- Pandas
- Scikit-learn
- Seaborn
- lightgbm
- xgboost
## Performances atteintes
|   Algorithme choisi    |   Précision en entraînement (%)    |   Précision en test (%)    |
|---    |:-:    |:-:    |
|   KNN    |   100    |   63.74    |
|   MLP    |   77.61    |   66.06    |
|   SVM    |   68.8    |   69.7    |
|   NuSVM    |    77.4   |    67.72   |
|   Random Forrest    |    100   |    68.71   |
|   Gaussian Naive Bayes    |   62.9    |    60.59   |
|   Gradient Boosting    |   82.37    |    65.23   |
|   LGBM    |    77.18   |    68.54   |
|   XGBoost    |   100    |    65.73   |
|   Gaussian Processes    |    61.69    |   60.26    |
|   Extremely randomized tree classifiers    |       |       |
|   Histogram-Based Gradient Boosting    |       |       |