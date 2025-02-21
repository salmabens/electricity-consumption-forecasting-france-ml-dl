# 🔋 Prévision de la Consommation Électrique en France avec ML & DL  

## 📖 Présentation  
Ce projet vise à **prévoir la consommation d'électricité en France** en utilisant des techniques de **Machine Learning (ML) et Deep Learning (DL)**. Grâce aux données historiques issues de la **plateforme Open Data de RTE**, nous développons des modèles prédictifs pour optimiser la gestion des ressources énergétiques et améliorer la précision des prévisions.  

## 🎯 Objectifs  
- Développer des modèles ML & DL pour anticiper la consommation électrique à différentes échelles de temps.  
- Analyser les données historiques (2012-2024) pour identifier les tendances et facteurs influençant la consommation.  
- Améliorer l'efficacité du réseau en réduisant la dépendance aux énergies fossiles et en optimisant l’utilisation des ressources.  

## 📊 Données  
Les données utilisées dans cette étude proviennent de la **plateforme Open Data de RTE** :  
- **Données consolidées (2012-2022)** : `eco2mix-national-cons-def.csv`  
- **Données en temps réel (2023-2024)** : `eco2mix-national-tr.csv`  

### 🔑 **Principales Caractéristiques**  
- **Consommation** : Données réelles et prévisions (MW).  
- **Production d'électricité** : Nucléaire, Énergies fossiles, Renouvelables (éolien, solaire, hydraulique, bioénergies).  
- **Échanges internationaux** : Flux d'électricité avec les pays voisins.  
- **Émissions de CO₂** : Intensité carbone de la production électrique.  

## 📈 Analyse Exploratoire des Données  
- **Saisonnalité de la consommation électrique** : Forte demande en hiver, baisse en été.  
- **Évolution des émissions de CO₂** : Tendance à la baisse grâce au développement des énergies renouvelables.  
- **Variabilité de la production** : Stabilité du nucléaire, forte fluctuation de l'éolien et du solaire.  

## 🧠 Approche de Modélisation  
Nous testons et comparons plusieurs approches de prévision :  
1. **Modèles de Machine Learning** : XGBoost et LightGBM.  
2. **Modèles de Deep Learning** : LSTM.

## 🚀 Comment Exécuter le Projet  

### 1️⃣ **Exécuter le Notebook sur Google Colab**  
Les fichiers étant volumineux, nous recommandons d'utiliser **Google Colab**.  

### 2️⃣ **Ajouter les Données sur Google Drive**  
- Créez un dossier nommé **"Data"** dans votre Google Drive.  
- Importez les fichiers de données (`eco2mix-national-cons-def.csv`, `eco2mix-national-tr.csv`) dans ce dossier.  

### 3️⃣ **Monter Google Drive dans Colab**  
Ajoutez ce code dans votre notebook pour accéder aux données :  

```python
from google.colab import drive
drive.mount('/content/drive')

data_path = "/content/drive/My Drive/Data/"
```

### 📂 **Structure du Projet**
📂 `electricity-consumption-forecasting-france-ml-dl`  
│── 📁 `Data` ➜ Fichiers de données (à ajouter sur Google Drive)  
│── 📁 `Modeles sauvegardes` ➜ Modèles entraînés et sauvegardes  
│── `Notebook` ➜ Notebook Jupyter pour l’analyse et la modélisation  
│── `.gitattributes` ➜ Configuration Git LFS pour gérer les fichiers volumineux  
│── `README.md` ➜ Documentation du projet  
│── `éCO2mix - Description des fichiers des données en puissance.pdf` ➜ Description des jeux de données utilisés  


