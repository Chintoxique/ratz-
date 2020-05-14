# Ratz-

Une intelligence artificielle pour s'occuper de nos gerbilles

## Introduction

Afin de surveillez et de répondre aux besoin primaire de nos gerbilles, nous avons mis au point une intelligence artificielle capable de s'occupez sans intéruption.

### Caractéristiques du programmes

* Detection des Gerbilles dans leur cage
* Detection des objets de leur quotidien (ex boites en carton, assiette à nourriture, lit,...)
* Système de notification WLAN pour l'approvisionnement des gerbilles

### But du projet

Nos gerbilles sont le terrain d'essaie parfait pour l'expérimentation de programme de gestion et de surveillance d'être vivant, permettant de répondre aux besoins de ceux-ci tout en les surveillant afin de les garders en vie dans un espace restreint.

Cette procédure de surveillance s'apparante fort aux programmes installé dans les maisons connectés et met en lumière les dérives d'un écosytème omnipotent et autonomme qui prends en charge toutes les actions d'autogestion d'un humain. 
Une intelligence artificielle serait donc capable de transformer notre maison en une usine régulant nos besoin primaire aux point de nous réguler nous même à un état de dépendance de la machine !

## Detection

On utilise [YOLO](https://pjreddie.com/darknet/yolo/) pour la detection d'object et d'animaux

### Nourriture et Carton

La camera garde toujours en vue la quantité de nourritures présente et notifie au moment de renouveller celle-ci

IMG

Le programme permet aussi de détecter quand les gerbilles manquent de carton afin qu'elles puissent constament avoir de quoi ronger

IMG

### Gerbilles

Le programme garde constament un oeil sur la postition des gerbilles, les moments où elles dorment ainsi que les tentatives d'évasion afin de notifier toutes leurs actions

IMG

## Application
Utilise notre réseau Wifi afin de nous notifier 

IMG

Elle affiche en temps réel le pourcentage des ressources présente dans la cage 

IMG


## Built With

* [YOLO]() - Object Detection
* [TailwindCss]() - Style, Postcss


## Authors

Envy
Leo

