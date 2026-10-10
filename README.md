<div align="center">

# 🧠 CC1 : Réseaux de neurones

**Classification (Iris) et régression (House Prices)**
Comparaison de trois approches d'entraînement

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-FF6F00?logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-MLP-F7931E?logo=scikitlearn&logoColor=white)
![Colab](https://img.shields.io/badge/Google-Colab-F9AB00?logo=googlecolab&logoColor=white)

</div>

---

## Sommaire

- [Objectif](#objectif)
- [Contenu du dépôt](#contenu-du-dépôt)
- [Partie 1 : Iris](#partie-1--iris-classification)
- [Partie 2 : House Prices](#partie-2--house-prices-régression)
- [Ouvrir dans Colab](#ouvrir-dans-colab)
- [Lancer le projet](#lancer-le-projet)
- [Outils utilisés](#outils-utilisés)
- [Auteur](#auteur)

## Objectif

Entraîner un réseau de neurones de trois façons et comparer leurs performances :

1. **scikit-learn** : `MLPClassifier` / `MLPRegressor`
2. **Keras** : API haut niveau avec `Sequential`
3. **TensorFlow bas niveau** : boucle d'entraînement manuelle avec `GradientTape`

## Contenu du dépôt

| Fichier | Description |
|---|---|
| `iris_classification.ipynb` | Partie 1 : classification Iris |
| `house_prices_regression.ipynb` | Partie 2 : régression House Prices |
| `iris_classification.pdf` | Export PDF du notebook Iris |
| `house_prices_regression.pdf` | Export PDF du notebook House Prices |
| `iris.csv` | Données Iris |
| `housing.csv` | Données House Prices |

---

## Partie 1 : Iris (classification)

**Données** : 150 fleurs, 4 mesures (longueur et largeur des sépales et des pétales), 3 espèces : *Setosa*, *Versicolor*, *Virginica*.

**Préparation** : encodage des classes (`LabelEncoder`), séparation 80 % / 20 % stratifiée, standardisation (`StandardScaler`).

**Modèles** : deux couches cachées de 10 neurones (ReLU), sortie softmax à 3 classes.

| Modèle | Accuracy |
|---|---|
| scikit-learn `MLPClassifier` | **96,67 %** |
| Keras `Sequential` | **96,67 %** |
| TensorFlow `GradientTape` | 93,33 % |

---

## Partie 2 : House Prices (régression)

**Données** : 545 logements, 13 colonnes (surface, chambres, salles de bain, étages, équipements, etc.). La variable à prédire est le **prix**.

**Préparation** : conversion des variables yes/no et de l'ameublement en valeurs numériques, séparation 80 % / 20 % (436 en entraînement, 109 en test), standardisation des variables et du prix.

**Modèles** : deux couches cachées (32 puis 16 neurones, ReLU), une sortie.

| Modèle | R² | RMSE | MAE |
|---|---|---|---|
| scikit-learn `MLPRegressor` | 0,6173 | 1 390 902 | 1 032 534 |
| Keras `Sequential` | **0,6189** | **1 387 836** | **998 208** |
| TensorFlow `GradientTape` | 0,5933 | 1 433 713 | 1 080 473 |

---

## Conclusion

Les trois approches donnent des performances proches. **Keras** obtient les meilleurs scores sur House Prices et fait jeu égal avec scikit-learn sur Iris. `GradientTape` est un peu en retrait, mais offre le plus de contrôle sur l'entraînement.

## Ouvrir dans Colab

| Notebook | Lien |
|---|---|
| Iris | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kniksiyassir/cc1-neural-networks/blob/main/iris_classification.ipynb) |
| House Prices | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kniksiyassir/cc1-neural-networks/blob/main/house_prices_regression.ipynb) |

## Lancer le projet

1. Cliquer sur le bouton **Open in Colab** du notebook voulu.
2. Importer le fichier de données demandé (`iris.csv` ou `housing.csv`).
3. Exécuter les cellules dans l'ordre (*Exécution → Tout exécuter*).

## Outils utilisés

Python · pandas · NumPy · matplotlib · scikit-learn · TensorFlow / Keras · Google Colab

## Auteur

**Yassir KNIKSI**
Master 1 Data Science, École Normale Supérieure de Martil, Université Abdelmalek Essaâdi

[![GitHub](https://img.shields.io/badge/GitHub-kniksiyassir-181717?logo=github)](https://github.com/kniksiyassir)
