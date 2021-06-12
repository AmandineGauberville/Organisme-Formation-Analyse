
# Project 2 : Analyse d'une offre de formation
Amandine GAUBERVILLE

*[Le 12/06/2021]*

## Content
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Workflow](#workflow)
- [Links](#links)

<a name="project-description"></a>

## Project Description
Nous tenterons dans ce projet d'analyser un organisme de formation au niveau régional sur une période de 6 ans à compter de 2014.

Le Cnam en région Centre-Val de Loire déploie une offre de formation très diversifiée de type enseignement supérieur (Bac+1 à Bac+5).

L'offre de formation est principalement dédiée aux adultes dans le cadre de la formation continue tout au long de la vie.

Le Cnam propose également de la formation en alternance.

Une telle offre est possible grâce aux partenariats que le Cnam entretient avec d'autres organismes.

Pour explication, l'offre de formation se découpe par l'organisation des formations en UE (Unités d’Enseignement) obligatoires, optionnelles ou libres. Ces UE comprennent des cours magistraux, des travaux dirigés et pratiques, des stages et/ou mémoires.

Les enseignements sont dispensés par semestre.

<a name="hypotheses-/-questions"></a>


## 1 Datasets

Le Dataset principal est issu de diverses requêtes SQL émanant d'un logiciel interne de scolarité.

Ce dataset est complété avec les compétences d'expertise attendues par le Cnam national sur chaque unité d'enseignement.

Ce premier dataset est composé de 7234 lignes pour 20 colonnes où une ligne correspond à une unité d'enseignement dispensée par un enseignant particulier.

Les réponses à un questionnaire d'autoévaluation complète un second dataset consacré aux compétences transversales des enseignants. Il s'agit d'un échantillon de 54 enseignants du Cnam Centre-Val de Loire.

<a name="workflow"></a>


## Workflow
Les étapes de cette analyse de données ont été :

1. La constitution des datasets sur Python
    - Requêtes SQL sur le logiciel interne pour extraction en fichiers csv.
    - Extraction de l'étude d'autoévaluation en fichiers csv.
    
2. Datacleaning sur Python
    - Suppression des valeurs nulles
    - Ajout du volume horaire par ligne
    - Anonymisation des enseignants
    
3. Analyse exploratoire des données sur Python
    - Dans un premier temps, l'analyse est effectuée de manière univariée
    - Dans un second temps, nous avons tenté de croiser les données par analyse bi-variée puis multivariée.

4. Datavisualisation sur Tableau public
    - Traduction des éléments d'analyse sur des graphiques plus complets
    - Storytelling


## Links

[Repository](https://github.com/AmandineGauberville/CnamCVDL_EDA)  

[Slides](https://drive.google.com/file/d/160RZuoULHFtDaafYZACtCP8Dfks2YGf9/view?usp=sharing)

[Storytelling](https://public.tableau.com/app/profile/gauberville.amandine/viz/AnalyseCnam/Analysedeloffredeformation)

