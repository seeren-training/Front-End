# User interface

*  🔖 **Server page**
*  🔖 **Client page**
*  🔖 **3-Tier et SOA**

La construction des interfaces utilisateurs peut se faire en utilisant la charge du serveur ou celle du client. L'objectif de cette introduction est de d'estimer l'impact de cette responsabilité.

___

## 📑 Server side

Un serveur pour produire à la volée des interfaces utilisateur. 

Le projet prend en charge manipulation de données et affichage: les actions de l'utilisateur ont un impacte directe sur le systèmes de stockage.

![image](./resources/svg/User-Interface!Server-Side!Server-Side_1.svg) 

L'effort de calcul des interfaces utilisateur effectué par le serveur une fois les entitées acquises. Le serveur utilise souvent des mécanismes demandant de conserver l'état de l'utilisateur comme les sessions, ce sont des applications avec état et il est difficile de mettre en cache le résultat d'un affichage propre à l'utilisateur en cours.

___

## 📑 Client side

Un script fourni par un server s'exécute chez le client pour produire des interfaces utilisateur. 

L'affichage est découplé du système de donnée. Le serveur effectue moins de traitement, n'ayant pas a générer du formattage de données il peut se consacrer à l'essentiel et être interopérable. Les flux de données peuvent être mis en cache contre l'adoption d'une représentation de la données par adresse descriptive.

![image](./resources/svg/User-Interface!Client-Side!Client-Side_0.svg) 

Pour un projet responsable de l'affichage et du traitement de données, cela représente un double projet avec soucent deux langages et patterns différents.

___

## 📑 3-Tier et SOA

Donner la responsabilité de l'affichage au server ou au client est un choix architectural.

L'architecture 3-Tier fournissant un calcul de page à un acteur, effectuant ce calcul sur un second acteur, grace à des données stockées par un troisième acteur forme un projet monolitique. Un problème de mise à l'echelle et donc d'évolutivité se présente rapidement au fur et à mesure que le projet grandi.

![image](./resources/svg/User-Interface!SOA!SOA_2.svg) 

L'architecture orientée service permet de mettre à l'echelle la couche serveur en créant des fournisseurs de service qui peuvent être différents de par leur détail d'implémentation. Chaque serveur utilisera un protocol de communication et une standardisation de l'interaction pour que le client ne soit pas dépendant de leur détails.

___

> Après avoir différencé les responsabilités posible de production d'interface utilisateurs et leur impact, interessons nous aux technologies qui permettent de les mettre en oeuvre.