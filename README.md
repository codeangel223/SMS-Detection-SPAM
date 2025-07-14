# 📩 Détection de SPAM dans les SMS

<!-- IMAGE D'EN-TÊTE -->
<p align="center">
  <img src="Images/SPAM-DETECTION.png" alt="Bannière de Détection de Spam"/>
</p>

---

## 📌 Présentation du projet

Ce projet est un système de **détection de spams dans les SMS**, basé sur les techniques de **traitement du langage naturel (NLP)** et le **Machine Learning**.  
Il utilise plusieurs modèles de classification, dont **Naive Bayes**, **SVM** et **Régression Logistique**, pour déterminer si un message est **normal** ou **indésirable (spam)**.

---

## ⚙️ Fonctionnalités

- Nettoyage et prétraitement des données (stopwords, ponctuation, doublons)
- Analyse exploratoire des données (EDA)
- Vectorisation des textes avec **TF-IDF**
- Entraînement de plusieurs modèles de machine learning
- Sélection automatique du **modèle le plus performant**
- Application en ligne de commande pour la prédiction de nouveaux SMS

---

## 🧰 Prérequis

Voici les dépendances nécessaires pour exécuter le projet :

- [Python 3.x](https://www.python.org/downloads/)
- pandas
- numpy
- scikit-learn
- nltk
- ....

Installation des paquets :

```bash
pip install -r requirements.txt
```

---

## 📂 Le Dataset

Le jeu de données contient environ **5 572 SMS**, chacun étiqueté comme suit :

- `spam` : message indésirable
- `ham` : message normal (non-spam)

Ce dataset est disponible sur Kaggle.

---

## 🧠 Structure du code

### 🔹 Partie 1 — Préparation des données

1. **Chargement du dataset**
2. **Nettoyage du texte** (suppression des stopwords, ponctuations, doublons)
3. **Analyse exploratoire des données (EDA)**
4. **Vectorisation des messages** via TF-IDF
5. **Découpage** des données en ensembles d'entraînement et de test

### 🔹 Partie 2 — Entraînement et évaluation des modèles

Trois modèles ont été entraînés :

- **Naive Bayes**
- **SVM (Support Vector Machine)**
- **Random Forest**

### 🔍 Comparaison des modèles

| Modèle                | Accuracy | Precision | Recall | F1-score |
| --------------------- | -------- | --------- | ------ | -------- |
| Naive Bayes           | 0.97     | 0.95      | 0.93   | 0.94     |
| SVM                   | 0.98     | 0.97      | 0.94   | 0.955    |
| Random Forest         | 0.97     | 0.96      | 0.92   | 0.94     |

✅ **Modèle sélectionné** : **SVM**, car il présente le meilleur compromis entre précision, rappel et F1-score.

#### 📊 Performances détaillées des modèles

**Naive Bayes**
<p align="center">
  <img src="Images/naives-bayes-perf.png" alt="Performance du modèle Naive Bayes"/>
</p>

**Random Forest**
<p align="center">
  <img src="Images/random-forest-perf.png" alt="Performance du modèle Random Forest"/>
</p>

**SVM (Support Vector Machine)**
<p align="center">
  <img src="Images/svm-perf.png" alt="Performance du modèle SVM"/>
</p>

---

## 💻 Démo en ligne de commande

L'application permet de prédire en ligne de commande si un message est un **spam** ou non.

<p align="center">
  <img src="Images/cli_apptest.png" alt="Démo CLI de l'application"/>
</p>

---

## 🚀 Lancer le projet

1. **Cloner le dépôt**

```bash
git clone https://github.com/codeangel223/Spam-Detection-IN-SMS-NLP
```

```bash
cd Spam-Detection-IN-SMS-NLP
```

2. **(Optionnel)** Entraîner à nouveau les modèles via le notebook ou script Python.

3. **Lancer l'application CLI**

```bash
python run.py
```

Saisissez un message lorsque demandé, et le programme indiquera s'il s'agit de **SPAM** ou de **NORMAL**.

---

## 📚 Références

- [Détection de spam avec le ML](https://bit.ly/3nwiKtA)
- [Algorithme Naive Bayes](https://bit.ly/3zc9SLH)
- [Évaluation de modèles](https://bit.ly/3B12VOO)

---

## 📬 Contact

**Moussa Mallé**

- GitHub : [@codeangel223](https://github.com/codeangel223)
- E-mail : [codeangel223@gmail.com](mailto:codeangel223@gmail.com)
- E-mail Perso: [mallemoussa091@gmail.com](mailto:mallemoussa091@gmail.com)

---

> 🧠 Projet éducatif basé sur le NLP, le Machine Learning et la mise en pratique de la détection automatisée de messages indésirables.