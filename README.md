## TP de BIG DATA & Data Miningl – Régression & Classification

Ce repository contient deux travaux pratiques  mettant en application des algorithmes  de machine learning avec Python en utilisant un notebook Jupyter

Notre dataset contient 35 colonnes, dont 34 features (attributs) et 1 colonne cible class que l'on souhaite prédire.

Chaque ligne représente un patient.

Les colonnes décrivent des caractéristiques cliniques et histopathologiques de maladies dermatologiques.

Exemple de colonnes :

erythema, scaling, itching → caractéristiques visibles sur la peau (rougeur, desquamation, démangeaison)
follicular_papules, oral_mucosal_involvement → présence de papules, atteinte des muqueuses
age → âge du patient
class → la maladie dermatologique diagnostiquée (c’est ce que us voulons prédire)


 Objectif : Entraîner un modèle de Machine Learning pour prédire la maladie (class) à partir des 34 autres colonnes.

Techniques et Methodes utilisees :

1. Nettoyer et préparer les données
2. Encoder les variables si nécessaire
3. Choisir un modèle (Logistic Regression et Random Forrest)
4. L'entraîner et l’évaluer (MSE, Accuracy, ...)

Fichier : TP_RL_et_RF_Demato.ipynb

