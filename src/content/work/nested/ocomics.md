---
title: O'Comics
publishDate: 2020-03-04 00:00:00
img: /assets/ocomics.jpg
img_alt: Pearls of silky soft white cotton, bubble up under vibrant lighting
description: |
  Création d'une platerforme d'échange de comics US.
tags:
  - Dev
  - User Testing
  - Prod
---

## Concept

> Le projet O’Comics a pour objectif de mettre à disposition une plateforme en ligne dédiée aux
passionnés de l’univers des comics, où ils pourront découvrir de nouveaux comics et en échanger avec
d’autres membres afin de compléter leurs collections respectives.

Étant moi-même féru de comics dans mes jeunes années et possédant des collections incomplètes, je me suis mis à la recherche de sites ou plateformes sur lesquelles je pourrais chercher les numéros manquants de mes collections. Il existe effectivement des sites où il est possible d’ acheter des comics et d’autres où il est possible de troquer des bandes dessinées classiques. J’ai donc eu l’idée de créer le projet O’Comics.

Les utilisateurs auront la possibilité de créer deux listes de favoris lorsqu'ils sont connectés en tant qu'utilisateurs enregistrés : l'une pour les comics qu'ils recherchent et l'autre pour les comics qu'ils possèdent déjà.

À terme, la plateforme vise à faciliter les échanges de comics entre les utilisateurs, en favorisant les transactions et les interactions au sein de la communauté. Le public cible de ce projet est principalement composé d'hommes âgés de 25 à 55 ans, partageant une passion pour l'univers riche et diversifié des comics.


### Team

##### 2 dev Front et 2 dev back

### Technologies

#### Front end

##### Framework React, Tailwind, Typescript, React Dom Router, Axios

La partie front-end de notre application à été réalisée avec React, framework utilisant Javascript et un DOM virtuel bien plus rapide que le DOM original, la possibilité de réutiliser
les composants de React permet de gagner du temps, le flux de données unidirectionel fournit un
code stable, de plus la librairie est open-source ce qui facilite la recherche d’informations et de
résolution de problème.
React permettant de faire ce que l’on appela une SPA (Single Page Application), nous avons utilisé
React Router afin d’avoir des routes virtuelles (seuls les composants présents sur la route sont placés
dans le DOM virtuel, le résultat est direct. L’utilisateur n’a pas l’impression d’avoir subi un
chargement de page).

Tailwind CSS intervient dans la gestion des styles de notre application. Il s'agit d'un framework CSS "utility-first" qui facilite la conception des éléments visuels de notre site. Au lieu de définir des styles personnalisés à partir de zéro, Tailwind CSS nous offre un ensemble complet de classes CSS préconçues que nous pouvons appliquer directement dans notre code HTML. Cela accélère le processus de développement en évitant la nécessité de créer des feuilles de style CSS distinctes. De plus, la normalisation des noms de classes avec Tailwind facilite la collaboration et garantit une cohérence dans l'apparence de notre application.

Nous avons suivi une approche "mobile-first" avec Tailwind CSS. Cela signifie que nous avons commencé par concevoir la version mobile de notre site (pour des largeurs inférieures à 425px). Avec Tailwind CSS, les classes de style sont appliquées directement dans le code HTML, ce qui simplifie la gestion des styles pour chaque composant ou page.

#### Back end

##### Framework Symfony, Doctrine, Twig, Bootstrap, MySQL, JWT, PhpMyAdmin, Insomnia

La partie back-end a été réalisée à l’aide du framework PHP Symfony dont l’approche se base sur des
composants et et du modèle MVC (Model-View-Controller).
MakerBundle a été utilisé pour permettre de générer rapidement des commandes vides, contrôleurs,
classes de formulaire, etc. en une ligne de commande.
L’ORM Doctrine a été utilisé pour la gestion de base de données, en tant qu’ORM son rôle est de
transformer les objets PHP en écriture SQL, et récupérer les écritures SQL et les transformer en objet
PHP

Le bundle Lexik JWT Authentication pour l’utilisation de token JWT, ce jeton sera envoyé envoyer à
chaque requête que l’on souhaite effectuer auprès d’une API afin de s’authentifier. Il contient toutes
les informations nécessaires à notre identification.
Notre serveur Symfony est lié à une base de données MySQL, administré via le gestionnaire de base
de données Adminer ou PHPMyAdmin selon les goûts de chacun.
