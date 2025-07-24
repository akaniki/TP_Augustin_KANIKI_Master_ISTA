## TP de BIG DATA & Data Mining – Régression & Classification

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

# 📊 UCI Credit Card Default Prediction

Ce projet utilise le célèbre dataset *UCI Credit Card Default* pour prédire si un client de carte de crédit fera défaut de paiement le mois suivant. Il s'agit d'un problème de classification binaire avec un fort potentiel pour l'analyse prédictive et l'apprentissage automatique.

## 🧠 Objectif

Développer et évaluer des modèles de Machine Learning capables de prédire le champ `default_payment_next_month` en fonction des autres caractéristiques du client (démographiques, comportement de paiement, montants facturés, remboursements…).

## 📁 Description du Dataset

Le dataset contient **30 000 lignes** et **24 colonnes**, dont :

| Colonne | Description |
|---------|-------------|
| `ID` | Identifiant du client (à ignorer dans les modèles) |
| `LIMIT_BAL` | Limite de crédit (en NT$) |
| `SEX` | Sexe (1 = Homme, 2 = Femme) |
| `EDUCATION` | Niveau d'éducation (1 = Graduate school, 2 = University, 3 = High school, 4 = Autre) |
| `MARRIAGE` | Statut marital (1 = Marié, 2 = Célibataire, 3 = Autre) |
| `AGE` | Âge |
| `PAY_0` à `PAY_6` | Historique de paiement mensuel (de avril à septembre) |
| `BILL_AMT1` à `BILL_AMT6` | Montants de facturation (avril à septembre) |
| `PAY_AMT1` à `PAY_AMT6` | Montants remboursés (avril à septembre) |
| `default_payment_next_month` | **Variable cible** (1 = défaut, 0 = pas de défaut) |

## 🔍 Explorations possibles

- Analyse de corrélation entre les variables de paiement et le défaut
- Étude des profils à risque (par sexe, âge, éducation…)
- Prétraitement des données (normalisation, gestion des outliers)
- Sélection de variables pertinentes pour la prédiction

## 🚀 Modèles à expérimenter

- Régression Logistique
- Arbre de décision & Random Forest
- Support Vector Machines (SVM)
- Réseaux de Neurones (Keras / TensorFlow)
- XGBoost / LightGBM

## 🛠️ Structure du Projet

```bash
📦 UCI_Credit_Default_Prediction/
├── data/
│   └── UCI_Credit_Card.csv
├── notebooks/
│   └── Exploratory_Analysis.ipynb
│   └── Model_Training.ipynb
├── models/
│   └── trained_model.pkl
├── README.md
├── requirements.txt
└── main.py
