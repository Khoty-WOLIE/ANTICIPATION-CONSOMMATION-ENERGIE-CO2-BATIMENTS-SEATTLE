## Aperçu de l'entreprise

![Aperçu du site web](images/DS_projet4.PNG)

## 📌 Contexte professionnel

Dans le cadre des efforts de la ville de **Seattle** pour atteindre la **neutralité carbone d’ici 2050**, j’ai été chargé de développer des **modèles prédictifs** pour estimer la **consommation d’énergie** et les **émissions de CO2** des bâtiments non résidentiels.  
L’objectif : éviter les campagnes de relevés coûteuses en s’appuyant sur les **caractéristiques structurelles** des bâtiments.

Le projet comprend également l’évaluation de l’intérêt du **"Energy Star Score"**, un indicateur environnemental complexe, dans les prédictions. Il repose sur l’application de **plusieurs algorithmes de machine learning** et sur une forte démarche exploratoire et interprétative.

---

## 🎯 Objectifs de la mission

1. Réaliser une **analyse exploratoire approfondie** des données
2. Développer et comparer plusieurs **modèles de prédiction** (ML)
3. Optimiser les modèles via **validation croisée** et **Grid Search**
4. Identifier les variables les plus influentes (via **SHAP**, **LIME**, etc.)
5. Évaluer la **pertinence du Energy Star Score** dans les prédictions

---

## 🧩 Étapes de réalisation

### 1. Analyse exploratoire des données (EDA)

- Visualisation de la distribution des variables
- Détection de valeurs aberrantes et traitement des valeurs manquantes
- Étude des corrélations entre caractéristiques et cibles

### 2. Modélisation initiale

- Développement de modèles simples (régression linéaire) pour établir une baseline
- Validation croisée (K-Fold) avec évaluation : **R²**, **MAE**, **RMSE**

### 3. Feature Engineering

- Encodage des variables catégorielles
- Création de nouvelles variables : ratios, indicateurs énergétiques
- Normalisation / standardisation
- PCA (si pertinent)

### 4. Modélisation avancée et optimisation

- Test d’algorithmes :
  - **ElasticNet**
  - **SVM**
  - **Random Forest**
  - **Gradient Boosting**
- Optimisation via **Grid Search** ou **Random Search**
- Comparaison des performances

### 5. Analyse de l’importance des variables

- Interprétation des modèles avec **SHAP**, **LIME**, coefficients
- Visualisation des variables les plus influentes
- Recommandations basées sur les insights

### 6. Évaluation du Energy Star Score

- Comparaison des performances avec et sans cette variable
- Analyse de sa contribution à la prédiction
- Justification de son utilité ou non dans le modèle final

### 7. Modélisation de la seconde target

- Reproduction du pipeline complet pour la deuxième variable cible
  (émissions ou consommation selon le choix initial)

---

## 📂 Livrables

- **Notebook de préparation des données**
- **Notebook de modélisation initiale et avancée**
- **Notebook d’analyse des variables importantes**
- **Rapport d’évaluation du Energy Star Score**
- **Présentation finale** des résultats et recommandations

---

## 🛠️ Compétences mobilisées

- **EDA avancée** et visualisation (matplotlib, seaborn)
- Feature engineering, traitement des outliers, normalisation
- Modélisation avec **scikit-learn** (régressions, SVM, RF, GB)
- **Optimisation des hyperparamètres** (GridSearchCV)
- **Interprétabilité des modèles** (SHAP, LIME)
- Communication claire des résultats à une audience métier

---

## ✅ Résultats et impact

- Modèle prédictif performant pour estimer consommation et émissions
- Identification des **caractéristiques clés influençant la performance énergétique**
- Aide à la **priorisation des interventions** sans mesures physiques coûteuses
- Support aux décisions stratégiques de la ville dans le cadre de sa **politique climat**

---

## 🔍 Aperçu

> Ce projet illustre mes compétences en **machine learning appliqué aux problématiques environnementales**, en **interprétabilité de modèles**, et en **mise en œuvre de pipelines complets** pour des cas réels à fort impact sociétal.

---

*Mission réalisée dans un cadre professionnel simulé, avec des responsabilités équivalentes à celles d’un Data Scientist pour une collectivité territoriale engagée dans la transition écologique.*
