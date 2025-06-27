# 🧠 Text Classification, Sentiment Analysis & Topic Modeling with NLP

Ce projet propose une approche complète de **text mining** basée sur un jeu de données de fake news. Il combine plusieurs techniques du **traitement automatique du langage naturel (NLP)** pour :

- Nettoyer les textes
- Vectoriser via TF-IDF
- Classifier les articles (Fake vs Factual)
- Analyser les sentiments
- Extraire les sujets dominants via le Topic Modeling

---

## 📌 Objectifs

- Appliquer un pipeline NLP sur des articles de presse
- Prédire si un article est une fake news ou une information factuelle
- Visualiser les résultats (accuracy, matrice de confusion, nuages de mots)
- Comprendre le sentiment global des textes
- Explorer les thèmes dominants dans les articles

---

## 🧰 Technologies utilisées

| Outil/Bibliothèque | Description |
|--------------------|-------------|
| `pandas`           | Chargement et manipulation des données |
| `matplotlib/seaborn` | Visualisations |
| `nltk`, `spacy`    | NLP : tokenisation, stopwords, lemmatisation |
| `scikit-learn`     | Classification, TF-IDF, évaluation |
| `gensim`           | Modélisation de sujets (LDA, LSI) |
| `vaderSentiment`   | Analyse de sentiment (rule-based) |

---

## 📂 Structure du projet


---

## 📊 Résultats Clés

- Précision des modèles de classification : **à compléter** (`accuracy_score`)
- Répartition équilibrée ou déséquilibrée des classes visualisée
- Résultats de sentiment pour chaque article (positif, neutre, négatif)
- Topics extraits automatiquement avec LDA/LSI

---

## 🧪 Techniques NLP appliquées

### 🔹 Prétraitement

- Nettoyage (regex, suppression des chiffres, ponctuation)
- Tokenisation : avec `nltk` & `spaCy`
- Stopwords removal : via `nltk`
- Lemmatisation : `WordNetLemmatizer` & `spaCy`

### 🔹 Vectorisation

- `TfidfVectorizer` : transforme les mots en vecteurs numériques pondérés par fréquence inverse

### 🔹 Classification

- Modèles utilisés : 
  - `LogisticRegression`
  - `SGDClassifier`
- Évaluation : 
  - `accuracy_score`
  - `classification_report`

### 🔹 Analyse de sentiment

- Utilisation de `VADER SentimentIntensityAnalyzer` pour obtenir un score de sentiment par document.

### 🔹 Modélisation de sujets (Topic Modeling)

- `gensim.models.LsiModel`, `LdaModel`
- Extraction automatique des sujets dominants dans le corpus

---

## 🚀 Lancer le projet

### 1. Installation
Cloner le repo :

git clone https://github.com/votre-utilisateur/text_classification.git
cd text_classification
Installer les dépendances :

pip install -r requirements.txt

2. Lancer le notebook

jupyter notebook Text_classification.ipynb

🔍 Jeu de Données
Nom : fake_news_data.csv

Colonnes principales :

text : contenu textuel de l’article

fake_or_factual : étiquette de vérité

NB : Le fichier CSV doit être placé dans le même dossier que le notebook.

📈 Visualisations proposées
Répartition des classes (bar chart)

Matrice de confusion

Score de sentiment

Top mots TF-IDF

Sujets par LDA/LSI

📌 À venir
Amélioration du modèle avec XGBoost, BERT

Export en API REST (Flask/FastAPI)

Dashboard interactif (Streamlit)

📚 Ressources utiles
Scikit-learn TF-IDF

NLTK Documentation

VADER Sentiment

Gensim Topic Modeling

👨‍💻 Auteur
Chouaib Khomalli
Master 1 – Ingénierie des Systèmes Intelligents - IA
📍 Casablanca, Maroc
