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
- interrogation sur les données manquantes (comment les trouver et solution apportée : morphologie ? gradient ?)
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
- choix de la taille des données (pixels), réflexion sur le nombre de variables que cela induit
- machine learning : régression logistique sur données en noir et blanc
- deep learning : ResNet (50 ? moins performant ? -> le plus adapté) sur données à 3 niveaux

Délimitation des avancées concrètes qui pourront être mises en oeuvres pour battre la baseline :
- redimensionnement des données : suite de la recherche d'une méthode pour faire un "crop circle" sur les images
- data augmentation, modèles avancés

#### Travail à faire :
- Finition des 2 baselines
- Décisions finales sur les problèmes relatifs : garder la baseline avec ce choix de nombre de pixels ? quelles avancées dans ce domaine ?

### Lundi 7 mars
- bilan des travaux effectués
- mise en place d'une stratégie pour la suite du projet
- définition de la fonction resize
- définition de la fonction permettant d'enlever les parties non informatives d'une image (parties noires)
- mise au propre du notebook Kaggle
- création de la baseline avec régression logistique
- problème rencontré : la régression logistique ne fonctionne pas (probablement car trop de variables)

Modèles de machine learning à tester :
- k-nearest neighbors (KNN)
- random forest
- support vector machines (SVM)
- linear discriminant analysis (LDA) et quadratic discriminant analysis (QDA)
- naive bayes
- AdaBoost, gradient tree boosting
- stacking

### Mardi 15 mars
- répartition du travail pour la journée
- recherche sur l'ACP et implémentation
- entraînement des modèles de machine learning et résultats
- recherche sur un filtre (bruitage gaussien)

### Mardi 29 mars

|          Modèle          | KNN (32) avec partie noire | KNN (32) sans partie noire | KNN (64) avec partie noire | KNN (64) sans partie noire |
|:------------------------:|:-:|:-:|:-:|:-:|
|         Accuracy         | 0.724  |  0.708 |  0.709 | 0.701  |
| Quadratic weighted Kappa |  0.583 |  0.570 |  0.575 | 0.567  |

|          Modèle          | LDA (32) avec partie noire | LDA (32) sans partie noire | LDA (64) avec partie noire | LDA (64) sans partie noire | LDA (128) sans partie noire
|:------------------------:|:-:|:-:|:-:|:-:|:-:|
|         Accuracy         | 0.686  |  0.656 |  0.492 | 0.502  | 0.654  | 
| Quadratic weighted Kappa |  0.617 |  0.598 |  0.378 | 0.463  | 0.672  |

|          Modèle          | QDA (32) avec partie noire | QDA (64) avec partie noire | SVM (32) avec partie noire | SVM(64) avec partie noire |
|:------------------------:|:-:|:-:|:-:|:-:|
|         Accuracy         | 0.532  |  0.086 |  0.724 | 0.502  |
| Quadratic weighted Kappa |  0.110 |  -0.019 |  0.619 | 0.463  |

- mise en place d'une stratégie pour la suite du projet
- entraînement des modèles de machine learning et résultats
- implémentation et entraînement d'un MLP
- implémentation d'un réseau CNN
- rédaction du rapport

### Vendredi 15 avril
- énumération des travaux à effectuer avant la soutenance
- rédaction du rapport
- mise au propre du notebook Kaggle et correction des éventuelles erreurs
