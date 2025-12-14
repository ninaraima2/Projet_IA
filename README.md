# Projet Titanic - Prédiction de la survie des passagers

## Description
Ce projet utilise le célèbre dataset **Titanic** pour prédire la survie des passagers.  
L’objectif est de comparer plusieurs modèles de machine learning et de sélectionner celui qui offre les meilleures performances.

---

##  Étapes du projet
1. **Exploration des données (EDA)**  
   - Analyse des colonnes, valeurs manquantes et distribution de la cible.  
   - Visualisations : histogrammes, boxplots, heatmap de corrélation.  

2. **Prétraitement**  
   - Imputation des valeurs manquantes (médiane).  
   - Encodage des variables catégorielles avec `LabelEncoder`.  
   - Normalisation des variables numériques avec `StandardScaler`.  

3. **Modélisation**  
   - **XGBoost**  
   - **Random Forest**  
   - **Neural Network (MLP)**  
   - Optimisation des hyperparamètres avec `GridSearchCV` et validation croisée (5-fold stratifiée).  

4. **Évaluation**  
   - Métriques : Accuracy, ROC-AUC, matrice de confusion, rapport de classification.  
   - Visualisations : courbes ROC et heatmaps.  

5. **Prédictions sur test.csv**  
   - Application du même pipeline de prétraitement.  
   - Génération des fichiers de soumission :  
     - `submission_xgboost.csv`  
     - `submission_randomforest.csv`  
     - `submission_neural_network.csv`  

---

##  Résultats
- **XGBoost** : Accuracy ≈ 84%, ROC-AUC ≈ 0.89  
- **Random Forest** : Accuracy ≈ 81%, ROC-AUC ≈ 0.86  
- **Neural Network (MLP)** : Accuracy ≈ 81%, ROC-AUC ≈ 0.86  

 **XGBoost est retenu comme modèle final** car il combine performance, stabilité et adaptation aux données tabulaires.

---

## Fichiers générés
- `histogrammes.png` : distributions des variables numériques  
- `correlation_matrix.png` : matrice de corrélation  
- `diagrammes_de_dispersion.png` : boxplots par classe  
- `*_confusion_matrix_cv.png` : matrices de confusion par modèle  
- `*_roc_curve_cv.png` : courbes ROC par modèle  
- `submission_xgboost.csv`  
- `submission_randomforest.csv`  
- `submission_neural_network.csv`

---

## 👩‍💻 Auteur
Projet réalisé par **Adja Mamaro Nina Raima Traoré**, étudiante en informatique à l’UQAR – Campus de Lévis.  
