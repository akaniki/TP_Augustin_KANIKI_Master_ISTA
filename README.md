## TP de BIG DATA & Data Mining – Régression & Classification
# 🧠 Machine Learning sur deux jeux de données : Carte de Crédit & Dermatologie

Ce dépôt présente deux projets de classification supervisée :

1. **Prédiction de défaut de paiement** (finance)
2. **Diagnostic de maladies dermatologiques** (santé)

Les modèles utilisés incluent :
- Réseau de Neurones Supervisé (SNN)
- Régression Logistique
- Forêt Aléatoire (Random Forest)

---

## 📁 Structure du projet
```
.
├── Data/                          # Dossiers contenant les datasets
│   ├── UCI_Credit_Card.csv        # Dataset sur les cartes de crédit (Kaggle)
│   └── dermatology.csv            # Dataset sur les diagnostics dermatologiques (Kaggle)
│
├── TP Credit_Card_SNN.ipynb       # Notebook d'entraînement du SNN sur les données de crédit
├── TP RL_et_RF_Dermato.ipynb      # Notebook de Régression Logistique et Random Forest sur les données dermatologiques
│
├── README.md                      # Description du projet
├── Requirement.txt                # Dépendances Python à installer

``` 
---

## 📌 1. Projet Crédit (UCI Credit Card Dataset)

### 🎯 Objectif
Prédire si un client va faire défaut sur sa carte de crédit le mois suivant (`default_payment_next_month`).

### 📊 Données
- Source : Kaggle - uciml/default-of-credit-card-clients-dataset
- Nombre d’observations : 30 000+
- Variables : `LIMIT_BAL`, `SEX`, `AGE`, `EDUCATION`, `MARRIAGE`, `PAY_0` à `PAY_6`, `BILL_AMT`, etc.
- Cible : `default_payment_next_month`

### ⚙️ Modèle utilisé
- Type : Classification binaire
- Algorithme : Supervised Neural Network (SNN)
- Techniques :
  - Nettoyage des données
  - Encodage des variables catégorielles si besoin
  - Standardisation des features numériques
  - Entraînement du modèle avec Keras
  - Évaluation avec accuracy et matrice de confusion

---

## 📌 2. Projet Dermatologie

### 🎯 Objectif
Classer les patients dans l’une des 6 classes de maladies dermatologiques à partir d'observations cliniques.

### 📊 Données
- Source : Kaggle - olcaybolat1/dermatology-dataset-classification
- Nombre d’échantillons : 366
- Cible (`class`) : 6 types de maladies

### ⚙️ Modèles testés
- Régression Logistique
- Random Forest
- Réseau de neurones multiclasses (optionnel)

### 📈 Évaluation
- Accuracy
- Matrice de confusion
- Visualisation des erreurs

---

## 🚀 Installation

```bash
pip install -r requirements.txt
