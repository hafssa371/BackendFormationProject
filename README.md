🗂️ Système de Gestion des Produits et des Fournisseurs

Ce projet correspond au développement d’une application backend réalisée dans le cadre d’un travail pratique en programmation backend.
L’objectif principal est de concevoir une application permettant de gérer des produits et des fournisseurs, tout en mettant en œuvre une relation plusieurs-à-plusieurs entre ces deux entités.

Le projet s’appuie sur Spring Boot (Java) et une base de données MySQL via XAMPP, avec une organisation claire du code et une séparation des responsabilités.

Contexte du projet : 

=> Cette application a été développée afin de renforcer la compréhension des concepts suivants :

=> Développement backend avec Java et Spring Boot

=> Conception d’une architecture MVC

=> Gestion des relations entre entités avec JPA

=> Interaction avec une base de données relationnelle (MySQL)

=> Structuration professionnelle d’un projet backend

Organisation générale du projet : 

Le projet est structuré selon une architecture MVC :

=> Couche Controller : gestion des requêtes HTTP et affichage des pages

=> Couche Service : traitement de la logique métier

=> Couche Repository : communication avec la base de données

=> Couche Entity : modélisation des tables Produit et Fournisseur

Technologies et outils utilisés : 

=> Java 21

=> Spring Boot

=> Spring Web

=> Spring Data JPA

=> Thymeleaf

=> MySQL (via XAMPP)

=> Maven

=> Git

 Modélisation des entités : 
 
=> Entité Produit :(nom,description,prix,stock)

=> Entité Fournisseur :(nom,adresse,produits fournis)

🔗 Les entités sont liées par une relation Many-to-Many, implémentée avec une table de jointure.

Interfaces Web prévues : 

Liste des Produits : Cette page permet de consulter l’ensemble des produits disponibles avec :

=> leur nom

=> leur description

=> leur prix

=> la quantité en stock

Détail d’un Fournisseur : Cette page affiche :

=> les informations d’un fournisseur

=> la liste des produits qu’il met à disposition

 Mise en œuvre du backend avec Spring Boot: 
 
Création du projet

Le projet a été initialisé à l’aide de Spring Initializr, en sélectionnant les dépendances nécessaires au développement web et à la persistance des données.

Configuration de la base de données (MySQL – XAMPP)

Installation de XAMPP

=> Démarrage des services Apache et MySQL

=> Création de la base de données via phpMyAdmin

=> Connexion à MySQL depuis Spring Boot via application.properties

=> Développement des entités JPA

Définition des classes Produit et Fournisseur

=> Utilisation des annotations JPA (@Entity, @Id, @ManyToMany)

=> Création automatique des tables via Hibernate

=> Gestion de la relation entre produits et fournisseurs

Accès aux données

=> Mise en place de repositories basés sur JpaRepository

=> Gestion des opérations CRUD sans requêtes SQL explicites

Logique métier

=> Les services centralisent les traitements

=> Séparation claire entre la logique métier et les contrôleurs

=> Meilleure maintenabilité du code

Gestion des contrôleurs

=> Récupération des données depuis la base MySQL

=> Transmission des données aux pages Thymeleaf

=> Gestion de la navigation entre les pages

 Suivi du projet avec Git

=> Initialisation du dépôt Git

=> Utilisation de la branche principale main

=> Développement progressif avec commits explicites

=> Historique clair et lisible du projet

Bilan du projet : 

Ce projet m’a permis d’approfondir mes connaissances en Spring Boot, notamment dans la gestion des relations complexes entre entités et l’utilisation d’une base de données MySQL via XAMPP dans un contexte réel.

Axes d’amélioration : 

=> Ajout des formulaires de gestion (CRUD complet)

=> Mise en place de la pagination

=> Validation des données côté serveur

=> Sécurisation de l’application

=> Déploiement sur un serveur distant

