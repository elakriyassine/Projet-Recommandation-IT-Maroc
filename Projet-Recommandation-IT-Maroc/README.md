# Projet de Recommandation IT Maroc

## Résumé du Projet
Ce projet de Data Science a pour objectif d'analyser le marché de l'emploi IT au Maroc. En utilisant des techniques de **web scraping**, il collecte des données sur les offres d'emploi et les formations universitaires. Le but final est de construire un **système de recommandation** qui aide les jeunes diplômés et étudiants à s'orienter vers les formations les plus adaptées aux compétences recherchées par les entreprises.

Le projet couvre l'ensemble du cycle de vie d'un projet de données :
* **Web Scraping & Nettoyage** : Collecte, fusion et nettoyage des données.
* **Analyse de Données** : Exploration et visualisation des tendances clés du marché.
* **Modélisation** : Création d'un modèle de classification et d'un système de recommandation.

## Structure du Dépôt
Le dépôt est organisé de manière logique pour suivre le flux de travail du projet :

* **`data/`** : Contient tous les fichiers de données.
    * `raw/` : Données brutes issues des sources.
    * `processed/` : Données nettoyées, fusionnées et prêtes pour l'analyse.
* **`notebooks/`** : Contient tous les notebooks Jupyter, répartis en sous-dossiers pour une meilleure lisibilité.
    * `scraping_and_cleaning/` :
        -   `rekrute.ipynb` : Script de web scraping pour les offres d'emploi sur Rekrute.
        -   `emploi2020.ipynb` : Script de web scraping pour les offres d'emploi sur Emploi.
        -   `merge.ipynb` : Script pour la fusion des différentes sources de données.
        -   `cleandata.ipynb` : Script pour le nettoyage et la préparation du jeu de données final.
    * `analysis/` :
        -   `analysis.ipynb` : Analyse exploratoire des données, statistiques descriptives et visualisations.
        -   `analysis2.ipynb` : Analyse plus poussée des tendances du marché.
    * `classification_and_recommendation/` :
        -   `Classification.ipynb` : Construction et évaluation d'un modèle de classification pour catégoriser les offres d'emploi.
        -   `CodeRecommandationV4.ipynb` : Implémentation du système de recommandation.
* **`sql/`** : Contient les scripts SQL pour la création de la base de données et l'importation des données.

## Technologies Utilisées
Ce projet est principalement développé en **Python** et s'appuie sur les outils et bibliothèques suivants :

* **Analyse de Données** : `Pandas`, `NumPy`
* **Web Scraping** : `BeautifulSoup`, `requests`
* **Traitement du langage** : `NLTK`, `re`
* **Machine Learning** : `scikit-learn`
* **Visualisation** : `Matplotlib`, `Seaborn`
* **Base de Données** : SQL

## Comment Utiliser ce Projet
Pour explorer ce projet sur votre machine locale, suivez ces étapes :

1.  **Clonez le dépôt** depuis GitHub.
2.  **Installez les dépendances** Python nécessaires en utilisant `pip`.
3.  **Suivez l'ordre logique** des notebooks dans le dossier `notebooks/` pour reproduire le projet, du scraping initial à la recommandation finale.
