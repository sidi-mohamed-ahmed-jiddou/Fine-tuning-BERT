# Analyse de Sentiment en Arabe Marocain avec un Modèle BERT Fine-Tuné

## Vue d'Ensemble

Ce projet se concentre sur l'analyse de sentiment pour des commentaires en dialecte arabe marocain en utilisant un modèle BERT fine-tuné.
L'objectif est de classer les commentaires en sentiments positifs ou négatifs. Le projet implique le prétraitement des données textuelles, 
le fine-tuning d'un modèle BERT pré-entrainé, et l'évaluation de sa performance à l'aide de classificateurs de machine learning.

## Structure du Projet

- **Données** : Le jeu de données consiste en des commentaires en arabe marocain étiquetés avec des sentiments (0 pour négatif, 1 pour positif).
  
- **Prétraitement** : Cette étape inclut le nettoyage du texte, la suppression des mots vides, le stemming, et la tokenisation.

- **Modèle** : Utilisation du modèle `CAMeL-Lab/bert-base-arabic-camelbert-msa-sentiment` pour le fine-tuning.

- **Entraînement** : Le modèle BERT est fine-tuné sur le jeu de données, et des embeddings sont extraits pour la classification.

- **Évaluation** : Plusieurs classificateurs (par exemple, Régression Logistique, Random Forest) sont entraînés sur les embeddings pour prédire le sentiment.

## Prérequis

- Python 3.x

### Librairies nécessaires :
- `transformers`
- `pytorch`
- `scikit-learn`
- `pandas`, `numpy`
- `evaluate`
- `nltk`, `PyArabic`, `Tashaphyne`, `Arabic-Stopwords`

## Installation

1. Clonez ce dépôt sur votre machine locale.
   ```bash
   git clone git clone https://github.com/sidi-mohamed-ahmed-jiddou/Fine-tuning-BERT.git
