# APTOS 2019 Blindness Detection
## Master 2 Data science - Data camp

https://www.kaggle.com/c/aptos2019-blindness-detection

**Notre équipe** : Cathia Le Hasif, Paul Mazet, Etienne Gaucher

### Lundi 10 janvier

#### Travail effectué :
- création de nos comptes Kaggle
- création d'une team sur Github
- prise en main de Kaggle et création d'un notebook collaboratif
- création de notebooks personnels
- début de visualisation des données
- recherche sur le preprocessing en consultant les travaux accessibles sur Kaggle

#### Travail à faire :
- continuer la recherche sur le preprocessing
- commencer la recherche sur les méthodes de machine learning pour le traitement d'images


### Lundi 24 janvier

#### Travail effectué :
- recherche sur la rétinopathie diabétique
- recherche sur le preprocessing
- mise en commun de nos recherches pour établir le preprocessing
- implémentation dans le notebook Kaggle du preprocessing (partie 1/2)
- énumération des différentes méthodes de machine learning qui seront appliquées
- interrogation sur les données manquantes (comment les trouver et solution apportée : morphologie ? Gradient ?)
- recherche sur le score quadratic weighted kappa et son utilité
- réunion pour faire le plan, faire le bilan des idées

#### Travail à faire :
- implémenter le data augmentation et la fonction resize qui permet de mettre les images à la même taille (rognage/centrage)
- implémenter le filtre gris qui sera utile pour certains modèles

### Lundi 14 février  
- création d'un diagramme de Gantt pour organiser le projet
- recherche d'une méthode pour faire un "crop circle" sur les images
- recherche d'une méthode pour transformer les images en noir et blanc

### Lundi 21 février
Début d'implémentation des 2 baselines : 
- Choix de la taille des données (pixels) 
- ML : Regression logistique sur données en noir et blanc
- DL : ResNet (50 ? moins performant ? -> le plus adapté) sur données à 3 niveaux

Délimitation des avancées concrètes qui pourront être mises en oeuvres pour battre la baseline :
- Redimensionnement des données : suite de la recherche d'une méthode pour faire un "crop circle" sur les images
- Data augmentation, modèles avancés

#### Travail à faire :
- Finition des 2 baselines
- Décisions finale sur les problèmes relatifs : garder la baseline avec ce choix de nb de pixels ? quelles avancées dans ce domaine ?

### Lundi 21 février
- réunion
- fonction resize
- fonction permettant d'enlever les parties non informatives d'une image (parties noires)
