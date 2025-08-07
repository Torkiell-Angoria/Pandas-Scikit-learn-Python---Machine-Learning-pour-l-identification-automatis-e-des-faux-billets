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

##  Livrables attendus

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

##  Choix du modèle final

Après avoir testé plusieurs algorithmes de classification (K-means, Régression Logistique, KNN, Random Forest), j’ai retenu **le modèle de régression logistique** comme modèle final pour cette mission.

Bien que tous les modèles aient présenté des scores de performance très élevés (notamment au niveau du F1-score), la régression logistique s’est distinguée par plusieurs avantages clés :

- Elle offre une **excellente performance prédictive** dans ce contexte.
- Elle permet d’**interpréter facilement l’importance des variables** utilisées dans le modèle, ce qui est un atout important pour la compréhension et la confiance des utilisateurs.
- Elle est **plus rapide à entraîner et à exécuter** que certains modèles plus complexes comme la Random Forest.

Cependant, il est important de noter que ce modèle repose sur une séparation essentiellement linéaire des classes. Si, à l’avenir, de nouvelles variables venaient à être ajoutées et rendaient la frontière de décision plus complexe (non linéaire), il faudra envisager de **changer de modèle** pour un algorithme plus flexible adapté à ces situations.

---

##  Description de l’application finale

L’application développée prend en entrée un **fichier Excel contenant des données géométriques des billets** (longueur, largeur, hauteur, etc.). 

Elle effectue pour chaque billet :

- Le calcul de la **probabilité** qu’il soit un vrai ou un faux billet,
- La **prédiction finale** : classée comme **VRAI** ou **FAUX** billet.

L’application génère ensuite un **nouveau fichier Excel** enrichi avec ces résultats, facilitant ainsi l’analyse et la prise de décision pour les équipes de l’ONCFM.

Cette solution simple, rapide et efficace permettra une utilisation opérationnelle immédiate dans la lutte contre la contrefaçon.
