# Projet Quotaclimat - Data For Good Grenoble

## 🗺️ Contexte

Le but du projet **Quotaclimat** est de faire rentrer l’**urgence climatique** dans l’**agenda médiatique**. L'objectif est la constitution d’une **base de données** et d'un **outil valorisant cette donnée** permettant un **observatoire citoyen**. Cela passe par l'**extraction des informations** sur le sujet du **climat** dans la couverture médiatique d’**articles de presse**.

## 🎯 Objectifs détaillés

Afin de mesurer la **couverture des sujets climat/environmentaux**, voici les **différentes thématiques** qu’on aimerait traiter :

1 - **Classifier** les titres d’articles informant l’appartenance ou non au sujet climat.

2 - **Classifier** le sujet des articles afin de pouvoir **comparer** par exemple la **couverture du traitement médiatique** de la **reforme des retraites** à celle de la sortie du **rapport du GIEC**.

3 - **Detecter** les articles **climato-sceptique** et/ou **anti-environnement** (par example vantant les mérites de l’avion ou des températures douces en hiver).

4 - **Comprendre le ton** des articles. Par exemple : “Climat : nous avons encore les moyens d’agir” est positif et subjectif tandis que “Limiter le réchauffement à 1,5 °C ? Trop tard, affirment mille scientifiques” est négatif et objectif(?).

L'attendu pour la contribution est un **notebook propre d'analyse** ou un **script Python**.

## 📚 Données

Les données des articles de presse ont été **scrapées depuis décembre 2022**. Les **titres** des articles de presse ainsi que des **méta-données** ont été récupérées. Les **données** sont présentes dans les fichiers CSV nommé "quotaclimat_fulldataset_1.csv" et "quotaclimat_fulldataset_2.csv". Un **notebook de démarrage** nommé "demarrage.ipynb" est aussi présent.

## 🧰 Ressources et pistes de démarrage

- Dépôt Github avec l'ensemble des contributions nationales du projet Quotaclimat : https://github.com/dataforgoodfr/quotaclimat

- Notebook pour récupérer les données brutes de Quotaclimat (similaires aux données du fichier CSV "quotaclimat_fulldataset.csv") : https://github.com/dataforgoodfr/quotaclimat/blob/main/notebooks/get_started_sitemap.ipynb

- Pistes de démarrage :

    - Utiliser des plongements de mots (word embedding) ou de phrases pour les titres des articles en utilisant des modèles de transformeurs entrainés pour le français comme CamemBERT : https://huggingface.co/dangvantuan/sentence-camembert-large

    - Faire étiqueter les titres des articles grâce à un large modèle de langue (LLM) en faisant de l'ingénierie de prompt avec ChatGPT par exemple : https://openai.com/blog/chatgpt

    - Entrainer un modèle simple de classification grâce aux données étiquetées précédemment avec la bibliothèque Scikit-Learn par exemple : https://scikit-learn.org/stable/auto_examples/classification/plot_classifier_comparison.html