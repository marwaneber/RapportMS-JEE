# Rapport MS-JEE

## Introduction

L’objectif est de créer un système distribué basé sur les micro-services permettant de gérer les factures des clients en utilisant la même architecture que vous avez déjà développé auparavant en y intégrant un système de sécurité basé sur Keycloak, Un Bus de messagerie avec KAFKA, un service de Stream processing avec Kafka Streams et un service de Batch Processing avec Spring Batch.

## 1 - Architecture du Projet

### Conception

Pour construire ce projet on va suivre l'architecture des MicroServices suivant:

![](Screens/Architecture.jpg)

1. Customer-Service
2. Inventory-Service
3. Billing-Service
4. Eureka Discovery Service
5. Spring Cloud Gateway

### Implementation

Chaqu'un de ces Microservices a sa propre base de données.
Et par la suite en va voir en details les structure de chaque microservice:

`1. Customer-Service`

![](Screens/Customer.png)

`2. Inventory-Service`

![](Screens/Inv.png)

`3. Billing-Service`

![](Screens/Bill.png)

`4. Eureka Discovery Service`

![](Screens/Eureka.png)

`5. Spring Cloud Gateway`

![](Screens/GateWay.png)

## 2 - Test du Partie Backend

Pour garantie le bon fonctionnement des API qu'on a developer, on a utiliser Insomnia, une outil de RESTClient :

#### Dans cet partie on va essayé d'accées au les MicroServices, et obtenir les donnnées.


`A-1. GET Bills`

![](Screens/back_GetBills.png)

`A-2. GET Customers`

![](Screens/back_GetCustomers.png)

`A-3. GET Products`

![](Screens/back_GetProducts.png)


#### Dans cet partie on va essayé d'accées au les MicroServices, et obtenir les donnnées.

`B-1. POST Bills`

![](Screens/back_PostBills.png)

`B-2. POST Customers`

![](Screens/back_PostCustomers.png)

`B-3. POST Products`

![](Screens/back_PostProducts.png)


## 3 - Test du Partie Frontend

Pour cet partie on va voir l'implimentation du Frontend utilison la technologie `REACT.js` avec `Tailwind CSS`.

![](Screens/Front.png)

Et par la suite on va voir les parties réaliser :

`1. Produits`

![](Screens/front_Products.png)

`2. Clients`

![](Screens/front_Customers.png)

`3-a. Factures`

![](Screens/front_Bills.png)

`3-b. Détail de facture`

![](Screens/front_DetailBill.png)


## 4 - Quelle est la prochaine étape ?

Mon prochain objectif est d'intégrer KAFKA dans un nouveau MicroService qui va générer des factures du maniere aléatoire. Et d'ajouter ce MicroService dans mon systéme complet.

Ainsi que d'ajouter des couches de sécurité au `Frontend` et `Backend` utilisons Keycloak, j'ai déja commencer de l'integrer mais je rencontre des problèmes dans la partie du Bearer-Only.

## Conclusion

Je tiens de merci Mr. Youssfi pour cet formation qui m'a motivé de continuer mes autoformations dans ce sense là, et de réaliser plus des projets.

