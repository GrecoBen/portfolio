---
title: Oflix
publishDate: 2020-03-02 00:00:00
img: /assets/oflix.JPG
img_alt: Image de fond Oflix
description: |
  Plateforme de streaming
tags: 
  - Dev
  - User Testing
  - Prod
---

## Concept

> Le projet Oflix à été réalisé pendant ma spécialisation Symfony au cours de ma formation.

 Il a pour objectif de mettre à disposition une plateforme en ligne dédiée aux
aux films, où les utilisateurs une fois enregistrés et connectés peuvent créer une liste de films favoris.
Les administrateurs ont accès au CRUD des films afin de créer, editer, modifier ou supprimer des films.
Les administrateurs peuvent également ajouter ou supprimer des utilisateurs. Il n'a été réalisé uniquement en back end
en utilisant le générateur de template Twig pour rendre les vues.
J'ai travaillé seul sur ce projet.


### Technologies

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
