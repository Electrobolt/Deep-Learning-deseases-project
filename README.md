# Deep-Learning-deseases-project


# Prédiction du Cancer du Sein à l'aide de Réseaux de Neurones

Ce Jupyter Notebook démontre un projet d'apprentissage profond pour prédire le cancer du sein en utilisant un réseau de neurones implémenté avec PyTorch. Le projet utilise le jeu de données Wisconsin Breast Cancer pour classer les tumeurs comme malignes ou bénignes.

## Aperçu du Projet

Ce projet vise à construire un modèle prédictif pour le diagnostic du cancer du sein basé sur des caractéristiques extraites des biopsies de masses mammaires. Le modèle est entraîné en utilisant une architecture de réseau de neurones dans PyTorch. Le jeu de données Wisconsin Breast Cancer est utilisé à la fois pour entraîner et évaluer les performances du modèle. L'objectif est d'atteindre une haute précision dans la distinction entre tumeurs malignes et bénignes.

## Jeu de Données

Le projet utilise le jeu de données Wisconsin Breast Cancer Diagnostic. Ce jeu de données contient des caractéristiques calculées à partir d'images numérisées d'aspirations à l'aiguille fine de masses mammaires. Chaque instance dans le jeu de données représente une tumeur avec des caractéristiques associées et un label binaire indiquant si la tumeur est maligne ou bénigne.

## Méthodologie

1. **Chargement et Prétraitement des Données :**
   - Le jeu de données Wisconsin Breast Cancer est chargé en utilisant scikit-learn.
   - La mise à l'échelle des caractéristiques est effectuée à l'aide de `StandardScaler` pour normaliser les caractéristiques d'entrée.
   - L'encodage des labels est appliqué pour convertir les labels catégoriels (M/B) en représentations numériques (0/1).
   - Le jeu de données est divisé en ensembles d'entraînement et de test.
   - Les données sont chargées dans le `DataLoader` de PyTorch pour un traitement par lots efficace lors de l'entraînement.

2. **Architecture du Modèle :**
   - Une architecture de réseau de neurones est définie en utilisant le module `nn` de PyTorch.
   - L'architecture se compose de plusieurs couches entièrement connectées avec des fonctions d'activation appropriées (par exemple, ReLU, sigmoïde).
   - La couche de sortie a un seul neurone avec une activation sigmoïde pour produire un score de probabilité pour la malignité.

3. **Entraînement :**
   - Le modèle est entraîné en utilisant un optimiseur approprié (par exemple, Adam) et une fonction de perte (par exemple, l'entropie croisée binaire).
   - Le processus d'entraînement implique d'itérer à travers le jeu de données d'entraînement par lots, de calculer la perte et de mettre à jour les poids du modèle en utilisant la rétropropagation.
   - Les progrès de l'entraînement et les métriques (par exemple, précision, perte) sont surveillés et visualisés.

4. **Évaluation :**
   - Après l'entraînement, les performances du modèle sont évaluées sur l'ensemble de test réservé.
   - Des métriques telles que la précision, la précision, le rappel, le score F1 et l'AUC sont calculées.
   - Les résultats sont visualisés pour évaluer les capacités prédictives du modèle.

## Structure du Code

Le notebook est structuré comme suit :

1. **Importation des Bibliothèques :** Importer les bibliothèques nécessaires (PyTorch, scikit-learn, matplotlib). (Voir l'extrait de code ci-dessous)
2. **Préparation des Données :** Charger, prétraiter et diviser les données.
3. **Définition du Modèle :** Définir l'architecture du réseau de neurones.
4. **Boucle d'Entraînement :** Implémenter le processus d'entraînement.
5. **Évaluation :** Évaluer le modèle entraîné sur les données de test.
6. **Visualisation :** Afficher les résultats et les visualisations.

## contributeurs 
**TCHAFA TCHUITCHOU ELSY**
**EDO VOUNDI NICOLAS**
**FLORA PANSY**
**DJIFACK LINE AUDREY**
**TAZO TOUKEM BELLE-NICKELLE**
**TAPAMO DEMANOU FRANTZ**
**MBANG BELVINE**
