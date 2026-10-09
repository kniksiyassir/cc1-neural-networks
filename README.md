<div align="center">

# 🧠 CC1 : Réseaux de neurones avec TensorFlow / Keras

**Classification (Iris) et régression (House Prices)**
Comparaison de trois approches d'entraînement

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-FF6F00?logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-MLP-F7931E?logo=scikitlearn&logoColor=white)
![Colab](https://img.shields.io/badge/Google-Colab-F9AB00?logo=googlecolab&logoColor=white)

</div>

---

## 📑 Sommaire
- [Objectif](#-objectif)
- [Contenu du dépôt](#-contenu-du-dépôt)
- [Résultats](#-résultats)
- [Lancer les notebooks](#-lancer-les-notebooks)
- [Outils](#-outils)
- [Auteur](#-auteur)

## 🎯 Objectif
Entraîner un réseau de neurones de trois façons différentes et comparer leurs performances :

1. **scikit-learn** : `MLPClassifier` / `MLPRegressor`
2. **TensorFlow / Keras** : API haut niveau (`Sequential`)
3. **TensorFlow bas niveau** : boucle d'entraînement manuelle avec `GradientTape`

## 📂 Contenu du dépôt

| Fichier | Description |
|---|---|
| `iris_classification.ipynb` | **Partie 1** : classification du dataset Iris |
| `house_prices_regression.ipynb` | **Partie 2** : régression sur le dataset House Prices |
| `iris_classification.pdf` | Export PDF du notebook Iris |
| `house_prices_regression.pdf` | Export PDF du notebook House Prices |
| `iris.csv` / `housing.csv` | Données utilisées |

## 📊 Résultats

### Partie 1 : Iris (classification)

| Modèle | Accuracy |
|---|---|
| scikit-learn `MLPClassifier` | **96,67 %** |
| Keras | **96,67 %** |
| TensorFlow (`GradientTape`) | 93,33 % |

### Partie 2 : House Prices (régression)

| Modèle | R² |
|---|---|
| scikit-learn `MLPRegressor` | ≈ 0,617 |
| Keras | **≈ 0,619** (meilleur) |
| TensorFlow (`GradientTape`) | ≈ 0,593 |

> Les trois approches donnent des performances proches. Keras est la plus simple à utiliser, et `GradientTape` offre le plus de contrôle sur l'entraînement.

## 🚀 Lancer les notebooks

| Notebook | Ouvrir dans Colab |
|---|---|
| Iris | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kniksiyassir/cc1-neural-networks/blob/main/iris_classification.ipynb) |
| House Prices | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kniksiyassir/cc1-neural-networks/blob/main/house_prices_regression.ipynb) |

1. Cliquer sur le bouton Colab.
2. Exécuter les cellules dans l'ordre.
3. Importer le fichier CSV demandé (`iris.csv` ou `housing.csv`).

## 🛠️ Outils
Python · pandas · NumPy · matplotlib · scikit-learn · TensorFlow / Keras · Google Colab

## 👤 Auteur
**Yassir KNIKSI**
Master 1 Data Science, École Normale Supérieure de Martil, Université Abdelmalek Essaâdi
[GitHub](https://github.com/kniksiyassir)
