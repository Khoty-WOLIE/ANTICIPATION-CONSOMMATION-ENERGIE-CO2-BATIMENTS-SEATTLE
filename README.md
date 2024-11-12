# OPC_DATA_SCIENTIST_PROJET4
Anticipez les besoins en consommation de bâtiments


# Anticipation des Besoins en Consommation d'Énergie et d'Émissions de CO2 des Bâtiments - Ville de Seattle

## Aperçu de l'entreprise

![Aperçu du site web](images/DS_projet4.PNG)

## Contexte

Je travaille pour la ville de **Seattle** dans le cadre de son objectif de neutralité carbone à l’horizon 2050. Mon équipe s'intéresse à la consommation d'énergie et aux émissions de CO2 des bâtiments non résidentiels. Des relevés minutieux ont été réalisés en 2016, mais ces relevés sont coûteux et difficiles à reproduire à grande échelle. L'objectif est donc de prédire la consommation d'énergie et les émissions de CO2 des bâtiments non mesurés à partir de leurs caractéristiques structurelles (taille, usage, date de construction, etc.).

En parallèle, je dois également évaluer l’intérêt du **"ENERGY STAR Score"**, un indicateur complexe à calculer, pour estimer les émissions et la consommation d’énergie. Le projet inclut la comparaison de plusieurs algorithmes de machine learning pour trouver les meilleurs modèles prédictifs.

## Objectifs du Projet

1. **Analyse Exploratoire des Données** : Explorer et comprendre les données collectées, identifier les variables pertinentes et nettoyer les valeurs manquantes et aberrantes.
   
2. **Modélisation Prédictive** : Développer plusieurs modèles de machine learning pour prédire les émissions de CO2 et la consommation d'énergie des bâtiments non mesurés. Tester au minimum quatre algorithmes issus de différentes familles (par exemple : ElasticNet, SVM, Gradient Boosting, Random Forest).

3. **Optimisation des Modèles** : Ajuster et optimiser les hyperparamètres des modèles en utilisant des techniques de validation croisée et de recherche d’hyperparamètres.

4. **Analyse de l'Importance des Variables** : Comprendre l'importance des variables structurelles dans la prédiction des émissions et de la consommation d'énergie, notamment l’impact du **"ENERGY STAR Score"**.

## Étapes du Projet

### Étape 1 : Analyse Exploratoire des Données

- **Objectif** : Explorer les données pour mieux comprendre la distribution des variables, identifier les valeurs aberrantes et les relations entre les variables.
- **Détails** :
  - Calculer des statistiques descriptives sur les variables principales.
  - Réaliser des visualisations (histogrammes, boxplots, nuages de points) pour examiner les relations entre les variables et les cibles (émissions de CO2 et consommation d'énergie).
  - Nettoyer les données, gérer les valeurs manquantes, et traiter les valeurs aberrantes.
- **Livrable** : Un notebook contenant les statistiques descriptives, visualisations et premières idées de transformations des variables.

### Étape 2 : Développement et Simulation d'un Premier Modèle

- **Objectif** : Développer un modèle initial de prédiction des émissions de CO2 et de la consommation d'énergie.
- **Détails** :
  - Commencer avec un modèle simple (par exemple, une régression linéaire) pour établir une ligne de base.
  - Utiliser une validation croisée pour évaluer la performance du modèle sur des données non vues (mesures : R², MAE, RMSE).
  - Documenter les premiers résultats pour voir si des améliorations sont possibles à travers un meilleur feature engineering.
- **Livrable** : Un premier modèle de prédiction avec les évaluations de performance.

### Étape 3 : Amélioration du Feature Engineering

- **Objectif** : Optimiser le modèle initial en améliorant les caractéristiques utilisées pour la prédiction.
- **Détails** :
  - Appliquer des transformations (normalisation, encodage de variables catégorielles) pour améliorer la pertinence des variables.
  - Créer de nouvelles caractéristiques pertinentes, comme la proportion de sources d'énergie ou des indicateurs géographiques.
  - Tester différentes techniques de réduction de dimensions comme **PCA** (analyse en composantes principales) si nécessaire.
- **Livrable** : Un notebook montrant les étapes du feature engineering et l'impact sur la performance des modèles.

### Étape 4 : Test de Différents Modèles et Choix du Modèle Final

- **Objectif** : Tester différents modèles et sélectionner le meilleur.
- **Détails** :
  - Tester plusieurs algorithmes de machine learning, tels que **ElasticNet**, **SVM**, **Gradient Boosting**, et **Random Forest**.
  - Utiliser des techniques de recherche d'hyperparamètres (Grid Search ou Random Search) pour optimiser les modèles.
  - Comparer les performances des modèles avec des métriques comme le R², MAE, et RMSE.
- **Livrable** : Un modèle final optimisé avec les hyperparamètres ajustés et les évaluations de performance.

### Étape 5 : Analyse de l'Importance des Variables

- **Objectif** : Analyser les variables les plus importantes dans les prédictions du modèle final.
- **Détails** :
  - Utiliser des techniques comme **SHAP**, **LIME**, ou les coefficients des modèles linéaires pour interpréter l'importance des caractéristiques.
  - Visualiser l'importance des variables pour comprendre leur influence sur les prédictions.
  - Documenter les résultats et les implications pour la prise de décision.
- **Livrable** : Un rapport contenant une analyse de l’importance des variables et des visualisations pertinentes.

### Étape 6 : Évaluation de l’Influence de l'EnergyStarScore

- **Objectif** : Évaluer si l'**EnergyStarScore** a un impact significatif sur la performance du modèle.
- **Détails** :
  - Créer un sous-ensemble de données incluant et excluant l'EnergyStarScore.
  - Tester l'influence de cette caractéristique sur l’entraînement et les performances des modèles.
  - Comparer les résultats pour déterminer si l’EnergyStarScore est nécessaire pour prédire efficacement les émissions de CO2 et la consommation d'énergie.
- **Livrable** : Un rapport analysant l'impact de l'EnergyStarScore sur les modèles de prédiction.

### Étape 7 : Modélisation de la Deuxième Target

- **Objectif** : Reproduire le processus de modélisation pour la deuxième cible (émissions de CO2 ou consommation d’énergie, selon la cible initiale).
- **Détails** :
  - Répéter les étapes de nettoyage des données, de modélisation, d’optimisation des hyperparamètres et d’analyse des variables.
  - Documenter les résultats et comparer avec la première target.
- **Livrable** : Un deuxième notebook avec les résultats de la modélisation pour la deuxième cible.

## Détails Techniques

- **Fichiers** :
  - `Dataset des bâtiments de Seattle` : Données des bâtiments non résidentiels de la ville de Seattle, incluant leurs caractéristiques structurelles et énergétiques.
  - **Notebook de Préparation des Données** : Contient les étapes de nettoyage, de gestion des valeurs manquantes, et de transformation des variables.
  - **Notebook de Modélisation** : Contient les tests des différents algorithmes et les évaluations des performances.
  - **Notebook d’Analyse de l’Importance des Variables** : Contient les analyses de l’importance des variables et l’influence de l'EnergyStarScore.

- **Outils Utilisés** :
  - **Python**, avec les bibliothèques **pandas**, **scikit-learn**, **SHAP**, **LIME**, **matplotlib**, **seaborn** pour la préparation des données, la modélisation, et la visualisation.
  - **Grid Search** et **Random Search** pour l’optimisation des hyperparamètres.

- **Compétences Utilisées** :
  - Analyse exploratoire des données (EDA).
  - Feature engineering et gestion des valeurs aberrantes et manquantes.
  - Modélisation de machine learning et optimisation d’hyperparamètres.
  - Analyse de l’importance des caractéristiques (SHAP, LIME).

## Résumé

Ce projet vise à prédire la consommation d'énergie et les émissions de CO2 des bâtiments non résidentiels à Seattle. Grâce à l’utilisation de techniques avancées de machine learning et d’analyse des données, je fournis un modèle prédictif robuste et une analyse approfondie de l'importance des variables, notamment l’influence de l’**EnergyStarScore**. Les résultats contribueront aux efforts de la ville pour atteindre ses objectifs de neutralité carbone d’ici 2050.
