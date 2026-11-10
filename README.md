# 📦 Anticipation et Prédiction des Retards de Livraison (Supply Chain)

## 🎯 Objectif du projet
Comment prédire les risques de retard de livraison en fonction des caractéristiques des commandes (produits, régions, modes d'expédition) ? 

Ce projet vise à répondre à cet enjeu majeur pour la Supply Chain : **améliorer le taux de service en anticipant les perturbations au lieu de les subir**. L'objectif final est de modéliser ce risque logistique et d'identifier les facteurs opérationnels qui influencent le plus ces retards.

## 📊 Jeu de données
L'analyse repose sur le fichier `DataCoSupplyChainDataset.csv` (plus de 180 000 lignes), qui offre une vue granulaire de bout en bout sur :
* **Les caractéristiques des commandes** : catégories de produits, prix, volumes.
* **La logistique spatiale** : régions, pays de départ et d'arrivée.
* **L'exécution** : modes d'expédition, délais de livraison prévus vs réels, statuts.

## 🛠️ Méthodologie & Technologies (Machine Learning)
* **Préparation des données (EDA & Feature Engineering)** : Python (Pandas, Numpy)
* **Visualisation** : Plotly / Seaborn / Matplotlib
* **Modélisation prédictive (Classification)** : Scikit-Learn
  * Comparaison de plusieurs modèles de classification (ex: Régression Logistique, Random Forest, XGBoost) pour catégoriser les commandes en "À l'heure" ou "En retard".
  * Analyse de l'importance des variables (Feature Importance) pour isoler les causes racines des retards.

## 🚀 Prochaines étapes
1. **Data Cleaning** : Gestion des valeurs manquantes, formatage des dates et création de la variable cible (Target) basée sur l'écart entre le délai réel et prévu.
2. **Analyse Exploratoire (EDA)** : Cartographie des retards par région et par mode d'expédition.
3. **Feature Engineering** : Encodage des variables catégorielles et normalisation.
4. **Machine Learning** : Entraînement des modèles, évaluation (Accuracy, F1-Score, ROC-AUC) et restitution métier.
