# Modélisation des Flux de Transport Urbain en Graphe Orienté - Cas des Taxis New-Yorkais

## Description du Projet

Ce projet analyse et modélise les flux de transport urbain à New York en utilisant les données des taxis. L'objectif est de créer un modèle de graphe orienté pour comprendre les patterns de mobilité, prédire l'affluence et classifier les stations de transport. Le projet utilise diverses techniques de machine learning incluant le clustering, la classification et la régression.

## Objectifs

1. **Exploration et nettoyage des données** : Analyse des données de trajets de taxis new-yorkais
2. **Clustering** : Classification des stations selon leur affluence et caractéristiques
3. **Classification** : Prédiction du type de station et de son utilisation
4. **Régression** : Prédiction de l'affluence future dans les stations
5. **Visualisation géographique** : Cartes interactives des flux de transport

## Technologies Utilisées

- **Python** : Langage de programmation principal
- **Pandas** : Manipulation et analyse des données
- **NumPy** : Calculs numériques
- **Scikit-learn** : Machine learning (KMeans, DBSCAN, KNN, DecisionTree, RandomForest)
- **Folium** : Visualisations géographiques interactives
- **Matplotlib/Seaborn** : Graphiques et visualisations
- **NetworkX** : Modélisation de graphes (si applicable)
- **Jupyter Notebook** : Environnement de développement

## Données

- **Source** : Données de trajets de taxis new-yorkais (yellow_tripdata)
- **Variables** : Coordonnées GPS (pickup/dropoff), timestamps, distances, tarifs, etc.
- **Période** : Données historiques de trajets

## Méthodologie

### 1. Nettoyage et Exploration
- Nettoyage des données manquantes et aberrantes
- Analyse exploratoire des données (EDA)
- Visualisation des points de départ sur carte

### 2. Clustering
- **K-Means** : Regroupement des stations par similarité
- **DBSCAN** : Détection de clusters de densité variable

### 3. Classification
- **KNN** : Classification par plus proches voisins
- **Decision Tree** : Arbre de décision pour la classification
- **Random Forest** : Ensemble d'arbres de décision

### 4. Régression
- Prédiction de l'affluence future
- Modèles de régression pour les prévisions temporelles

### 5. Visualisation
- Cartes hexagonales des flux
- Cartes interactives avec Folium
- Graphiques de distribution et corrélations

## Structure du Projet

```
├── README.md
├── code.ipynb                          # Notebook principal
├── nettoyage_et_exploration.ipynb     # Nettoyage et EDA
├── clustering.ipynb                     # Analyse de clustering
├── classification.ipynb                 # Modèles de classification
├── regression.ipynb                     # Modèles de régression
├── map.html                            # Carte interactive des points de départ
└── map_hexagonale.html                 # Carte hexagonale des flux
```

## Utilisation

1. Installer les dépendances :
```bash
pip install pandas numpy scikit-learn folium matplotlib seaborn jupyter
```

2. Préparer les données :
   - Télécharger les données de trajets de taxis new-yorkais
   - Placer les fichiers CSV dans le répertoire approprié
   - Modifier les chemins dans les notebooks si nécessaire

3. Exécuter les notebooks dans l'ordre :
   - `nettoyage_et_exploration.ipynb`
   - `clustering.ipynb`
   - `classification.ipynb`
   - `regression.ipynb`

## Résultats

- Identification des zones à forte affluence
- Classification des stations selon leur type d'utilisation
- Prédictions d'affluence pour la planification
- Visualisations géographiques des patterns de mobilité

## Applications

Ce projet peut être utilisé pour :
- Optimisation des réseaux de transport
- Planification urbaine
- Prédiction de la demande de transport
- Analyse des patterns de mobilité urbaine

## Notes

- Les données peuvent être volumineuses, un échantillonnage peut être nécessaire
- Les cartes interactives sont générées en HTML et peuvent être ouvertes dans un navigateur
- Les modèles peuvent être ajustés selon les besoins spécifiques
