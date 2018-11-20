# application-Conversion

Binome :
tahraoui randa
abboudi raian
Rapport :

1.architecture globale de l'application : on choisit les web services:
figure.1

pour créer cette application il faut :
1 service d'email
2 un service pour choisir la conversion 
3.un service de téléchargement en 5 mn
 

2.architecture de la couche donnée: on choisit L'architecture trois tiers parce que C'est une architecture basée sur l'environnement client-serveur.: 
figure.2

modèle plus général qu'est le multi-tiers. L'architecture logique du système est divisée en trois niveaux ou couches:
1.Couche de présentation (premier niveau): On parle d'interface homme-machine(ici les interfaces pour choisir la conversion et..)
2.Couche de traitement (deuxième niveau: Elle correspond ‡ la partie fonctionnelle de l'application(dans notre application 
le code de l’application c.-à-d. les opérations de chaque serveur)
3.Couche d’accès aux données (troisième niveau):Elle correspond ‡ la partie gérant l’accès aux données de l'application(nous 
dans cette application on installe un serveur SQL comme xamp ou wamp pour gérer les donnes).

3.La manière de gestion des demandes des clients :
(diagramme de classe)  
https://user-images.githubusercontent.com/44061285/48780543-754ff480-ecda-11e8-9c69-aa43b9012bd0.png


4.les technologies:
#Appication image
OpenShift Container Platform fournit un processus S2I (source à image) pour créer et exécuter des applications permettant de joindre le code source d’une application au-dessus d’une image de constructeur (une image technologique telle que JBoss EAP).Il permet aux utilisateurs de créer et d'exécuter des applications Java simples
#Base de Donnée
OpenShift Container Platform fournit une image de conteneur pour l'exécution de MySQL. Cette image peut fournir des services de base de données basés sur les paramètres de nom d'utilisateur, mot de passe et nom de base de données fournis via la configuration.
#QuikStart apllication template 
Il s'agit d'un exemple de référentiel d'applications très basique qui peut être créé et déployé sur OpenShift à l'aide de l'image du générateur Serveur HTTP Apache







