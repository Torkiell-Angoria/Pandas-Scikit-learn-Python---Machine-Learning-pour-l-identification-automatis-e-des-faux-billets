# Application pour l'identification automatisé de faux billets en utilisant le Machine learning

Dans le cadre de sa lutte contre la contrefaçon de billets en euros, l’ONCFM souhaite mettre à disposition de ses équipes une **application capable de détecter automatiquement les faux billets** à partir de caractéristiques physiques (longueur, largeur, hauteur, etc.).

En tant que **data analyst senior**, ma mission consiste à :

- **Analyser un jeu de données** de 1500 billets (1000 vrais, 500 faux) fourni par l'ONCFM.
- Tester plusieurs **algorithmes de machine learning** afin d’identifier le modèle le plus performant pour détecter les faux billets.
- Développer une **application simple et efficace** permettant d’effectuer des prédictions à partir de nouvelles données.
- Présenter de manière claire et synthétique la démarche, les résultats obtenus et les choix réalisés tout au long du projet.

---

##  Outils et technologies utilisés

Ce projet a été entièrement réalisé en **Python**.  
Les bibliothèques et outils suivants ont été utilisés :

- **Pandas / NumPy** : pour la manipulation et le traitement des données
- **Matplotlib / Seaborn** : pour la visualisation des distributions et des résultats
- **Scikit-learn** : pour l’entraînement et l’évaluation des modèles de machine learning
- **Jupyter Notebook** : pour structurer les analyses, le développement de l’application et les visualisations
- **PowerPoint** : pour la présentation finale destinée au client

---

## 📦 Livrables attendus

Le projet doit être livré sous la forme d’un dossier compressé `.zip`, contenant les éléments suivants :

### 1. Notebook création du modèle
Ce notebook contient :

- L’importation, l’exploration et le nettoyage des données
- L’analyse descriptive des variables
- La mise en œuvre des différents modèles recommandés :
  - K-means (méthode non supervisée)
  - Régression Logistique
  - K-Nearest Neighbors (KNN)
  - Random Forest
- La comparaison des performances des modèles
- La justification du **modèle final retenu**

![Modele](https://github.com/Torkiell-Angoria/Pandas-Scikit-learn-Python---Machine-Learning-pour-l-identification-automatis-e-des-faux-billets/blob/main/img/creation-modele.gif)

---

### 2. Notebook de l'application
Ce deuxième notebook constitue une **application fonctionnelle** permettant à l’ONCFM de :

- Saisir les caractéristiques d’un billet (ou utiliser un fichier de test)
- Obtenir une prédiction immédiate : **vrai** ou **faux billet**
- Utiliser facilement le modèle final dans un cadre opérationnel

![Application](https://github.com/Torkiell-Angoria/Pandas-Scikit-learn-Python---Machine-Learning-pour-l-identification-automatis-e-des-faux-billets/blob/main/img/application.gif)

---

### 3. Présentation Power Point
Une **présentation claire et synthétique** du projet, à destination du client, qui contient :

- Le contexte et les enjeux de la mission
- La méthodologie suivie étape par étape
- Les résultats obtenus pour chaque modèle
- Le choix du modèle retenu et les raisons de ce choix
- Une démonstration de l'application développée

![Presentation](https://github.com/Torkiell-Angoria/Pandas-Scikit-learn-Python---Machine-Learning-pour-l-identification-automatis-e-des-faux-billets/blob/main/img/pr%C3%A9sentation.gif)

---

##  Résultat attendu

Le livrable final doit permettre à l’ONCFM de disposer d’un outil de **prédiction fiable, rapide et simple d’utilisation**, basé sur une analyse rigoureuse des données.  
Grâce à cette application, les équipes de terrain pourront **identifier en temps réel les faux billets** et ainsi renforcer l’efficacité de leur lutte contre le faux-monnayage.

---
