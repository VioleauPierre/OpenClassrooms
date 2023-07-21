# Openclassroom_Project_Analysez_donnees_systemes_educatifs

Projet n°2 du parcours Data Scientist d'Openclassroom

## Contexte

Vous êtes Data Scientist dans une start-up nommée Academy, qui propose des contenus de formation en ligne pour un public de niveau lycée et université. Mark, votre manager, vous a convié à une réunion pour vous présenter le projet d’expansion à l’international de l’entreprise. Il vous confie une première mission d’analyse exploratoire, pour déterminer si les données sur l’éducation de la banque mondiale permettent d’informer le projet d’expansion. Voici les différentes questions que Mark aimerait explorer, que vous avez notées durant la réunion :
1. Quels sont les pays avec un fort potentiel de clients pour nos services ?
2. Pour chacun de ces pays, quelle sera l’évolution de ce potentiel de clients ?
3. Dans quels pays l'entreprise doit-elle opérer en priorité ?

Mark vous a donc demandé de réaliser une analyse pré-exploratoire de ce jeu de données. Il vous a transmis cet email à la suite de la réunion : 
Hello, Les données de la Banque mondiale sont disponibles à l’adresse suivante : https://datacatalog.worldbank.org/dataset/education-statistics Ou en téléchargement direct à ce lien. Je te laisse regarder la page d'accueil qui décrit le jeu de données. En résumé, l’organisme “EdStats All Indicator Query” de la Banque mondiale répertorie 4000 indicateurs internationaux décrivant l’accès à l’éducation, l’obtention de diplômes et des informations relatives aux professeurs, aux dépenses liées à l’éducation... Tu trouveras plus d'info sur ce site : http://datatopics.worldbank.org/education/ Pour la pré-analyse, pourrais-tu : 
- Valider la qualité de ce jeu de données (comporte-t-il beaucoup de données manquantes, dupliquées ?) 
- Décrire les informations contenues dans le jeu de données (nombre de colonnes ? nombre de lignes ?) 
- Sélectionner les informations qui semblent pertinentes pour répondre à la problématique (quelles sont les colonnes contenant des informations qui peuvent être utiles pour répondre à la problématique de l’entreprise ?) 
- Déterminer des ordres de grandeurs des indicateurs statistiques classiques pour les différentes zones géographiques et pays du monde (moyenne/médiane/écart-type par pays et par continent ou bloc géographique) 

Ton travail va nous permettre de déterminer si ce jeu de données peut informer les décisions d'ouverture vers de nouveaux pays. On va partager ton analyse avec le board, alors merci de soigner la présentation et de l'illustrer avec des graphiques pertinents et lisibles !

## Compétences

- Mettre en place un environnement Python
- Utiliser un notebook Jupyter pour faciliter la rédaction du code et la collaboration
- Maîtriser les opérations fondamentales du langage Python pour la Data Science
- Manipuler des données avec des librairies Python spécialisées
- Trier et réduire un jeu de données
- Effectuer une représentation graphique à l'aide d'une librairie Python adaptée
- Effectuer des prévisions à l'aide d'un modèle de prédiciton linéaire

## Librairies utilisées

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

## Données

5 fichiers :

![image](https://user-images.githubusercontent.com/129098391/228335146-7aa71007-6428-44d7-9016-0133a29f6c70.png)

## Réduction du dataset

Selections des indicateurs (via pertinence, taux de remplissage) :

![image](https://user-images.githubusercontent.com/129098391/229604328-695ee6a9-d9ca-4a47-9910-1dc92882f446.png)

Réduction du nombre de pays (via groupe de revenus, population 15-24ans...) :

![image](https://user-images.githubusercontent.com/129098391/229604475-a9d04118-951b-47a0-81ae-c5313a988cbb.png)

## Analyse et scoring

Indicateurs en fonction des groupes (région géographique et revenus) : 

![image](https://user-images.githubusercontent.com/129098391/229588112-7c67070b-dd1e-4327-9c2f-2886c39ed8a8.png)

Indicateurs et score pour les pays avec un meilleur score que la France :

![image](https://user-images.githubusercontent.com/129098391/229588820-099fc56b-360a-4850-9b7d-8ed98191d101.png)

Score actuel et anticipé pour les pays avec un meilleur score que la France : 

![image](https://user-images.githubusercontent.com/129098391/229597557-59147f9c-553b-46cd-8f12-6210346a9ace.png)
