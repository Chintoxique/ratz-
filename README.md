# Ratz-

Une intelligence artificielle pour s'occuper de nos gerbilles

## Introduction

Afin de surveiller et de répondre aux besoins primaires de nos gerbilles, nous avons mis au point une intelligence artificielle capable de s'occuper sans interruption.

### Caractéristiques du programme

* Détection des Gerbilles dans leur cage
* Détection des objets de leur quotidien ( assiette à nourriture, eau, litière, boite en carton,...)
* Système de notification pour l'approvisionnement des gerbilles

### But du projet

Nos gerbilles sont le terrain d'essai parfait pour l'expérimentation de programme de gestion et de surveillance d'êtres vivants, permettant de répondre aux besoins de ceux-ci tout en les surveillant afin de les garder en vie dans un espace restreint.

Cette procédure de surveillance s'apparante fort aux programmes installés dans les maisons connectées et met en lumière les dérives d'un écosytème omnipotent et autonomme qui prends en charge toutes les actions d'autogestion d'un humain. 
Une intelligence artificielle serait donc capable de transformer notre maison en une usine régulant nos besoins primaires aux point de nous réguler nous même à un état de dépendance de la machine !

## Detection

On utilise [YOLO](https://pjreddie.com/darknet/yolo/) pour la détection d'objets et d'animaux

### Nourriture

La caméra garde toujours en vue la quantité de nourriture présente et notifie au moment de renouveller celle-ci

```
(FoodFull-ActiveFood)/FoodFull x 100 = FoodNeeded %
```

### Eau

```
(BoxWater-ContentWater)/BoxWater x 100 = WaterNeeded %
```
![Alt text](assets/RAT13.png?raw=true "Title")

### Carton

Le programme permet aussi de détecter quand les gerbilles manquent de carton afin qu'elles puissent constamment avoir de quoi ronger

```
BoxConsumed/BoxAll x 100 = BoxArea % 
if (BoxArea === 0) {
  Box ++
}
```


### Gerbilles

Le programme garde constament un oeil sur la postition des gerbilles, les moments où elles dorment ainsi que les tentatives d'évasion afin de notifier toutes leurs actions

![Alt text](assets/RAT12.png?raw=true "Title")

## Application
Utilise [OneSignal](https://documentation.onesignal.com/) pour notifier 

![Alt text](assets/notification.png?raw=true "Title")

Elle affiche en temps réel le pourcentage des ressources présente dans la cage 

![Alt text](assets/app.png?raw=true "Title")


## Built With

* [YOLO](https://pjreddie.com/darknet/yolo/) - Object Detection
* [VueJS](https://vuejs.org/v2/guide/) - Monitoring, Framework
* [OneSignal](https://documentation.onesignal.com/) - Notification


## Authors

Envy

### Note :
Plus l'environnement est robotisé/automatisé, plus le scénario peut s'avérer catastrophique à la moindre erreur de l'intelligence articifielle. L'autonomie des êtres vivants dépend alors de la machine.
En cas de dysfonctionnement, la vie des êtres vivants est mise en danger.
Ce qui démontre le risque que peut engendrer la dépendance aux machines. Si celle-ci est programmée pour notre survie.
