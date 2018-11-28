# application-Conversion
# Rapport:

# Binome :
# Tahraoui Randa
# Abboudi Raian



## 1.Architecture globale de l'application : on choisi les web services:
![webbb](https://user-images.githubusercontent.com/44061285/49148186-f759a200-f306-11e8-82fc-070e47047271.png)
(diagramme de classe)  
https://user-images.githubusercontent.com/44061285/48780543-754ff480-ecda-11e8-9c69-aa43b9012bd0.png


Pour créer cette application il faut :
Coté Serveur :
1. Service d'email
2. Service pour choisir la conversion 
3. Service de téléchargement en 5 mn
https://user-images.githubusercontent.com/44061285/49147636-7e0d7f80-f305-11e8-92bf-ccf877fc78cd.png


## 2.Architecture de la couche donnée:
On choisi L'architecture trois tiers parce que C'est une architecture basée sur l'environnement client-serveur: 
modèle plus général est le multi-tiers.


L'architecture logique du système est divisée en trois niveaux ou couches:

1.Couche de présentation (premier niveau) : On parle De L’interface homme-machine
2.Couche de traitement (deuxième niveau : Elle correspond à la partie fonctionnelle de l’application (c.-à-d. les opérations de chaque serveur)
3.Couche d’accès aux données (troisième niveau) : Elle correspond à la partie gérant l’accès aux données de l’application ( 
Un serveur SQL comme Xamp ou Wamp pour gérer les donnes)


## 3.La manière de gestion des demandes des clients :


Le client choisi la conversion voulu à travers l’application en envoyant un email (une tache facultatif)
La demande sera enregistrée dans une base 
Un message sera envoyé lors de l’enregistrement de la demande    accompagné d’un lien qui mène vers une page de statut là ou il trouvera sa demande s’il elle est en attente ou en cours ou bien terminé 
L’application ne supporte que deux clients en 5mn. En utilisant Les threads qui permettent la synchronisation entre les clients en concurrence 

## 4.les technologies:
1.OPENSHIFT :
#Appication image
OpenShift Container Platform fournit un processus S2I (source à image) pour créer et exécuter des applications permettant de joindre le code source d’une application au-dessus d’une image de constructeur (une image technologique telle que JBoss EAP).Il permet aux utilisateurs de créer et d'exécuter des applications Java simples
#Base de Donnée
OpenShift Container Platform fournit une image de conteneur pour l'exécution de MySQL. Cette image peut fournir des services de base de données basés sur les paramètres de nom d'utilisateur, mot de passe et nom de base de données fournis via la configuration.
#QuikStart apllication template 
Il s'agit d'un exemple de référentiel d'applications très basique qui peut être créé et déployé sur OpenShift à l'aide de l'image du générateur Serveur HTTP Apache
2.JAVA EE :
Java Platform, Enterprise Edition, Java EE ou Jakarta EE est une spécification pour la plate-forme Java d'Oracle, destinée aux applications d'entreprise2. La plate-forme étend Java Platform, Standard Edition (Java SE) en fournissant une API de mapping objet-relationnel, des architectures distribuées et multitiers, et des services web3. La plate-forme se fonde principalement sur des composants modulaires exécutés sur un serveur d'applications









