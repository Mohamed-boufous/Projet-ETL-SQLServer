Projet ETL - Intégration et Analyse de Données (SQL Server / SSIS / Power BI)

Ce projet implémente un pipeline ETL (Extract, Transform, Load) complet pour centraliser et analyser des données liées aux étudiants, à leurs activités et à leurs performances académiques.

📋 Présentation du Projet

L'objectif est d'extraire des données provenant de fichiers sources CSV, de les transformer pour garantir leur intégrité et leur cohérence, puis de les charger dans une base de données SQL Server. Enfin, une couche de visualisation est ajoutée via Power BI pour faciliter la prise de décision.

Architecture du projet :

Sources : Fichiers plats (CSV) contenant des informations sur les activités, les étudiants, les parents et les performances.

ETL : Utilisation de SQL Server Integration Services (SSIS) pour le nettoyage et le chargement des données.

Stockage : Base de données relationnelle SQL Server.

Visualisation : Rapport interactif Power BI.

🛠️ Technologies Utilisées

Base de données : SQL Server (T-SQL)

ETL : SQL Server Integration Services (SSIS) / Visual Studio

BI & DataViz : Power BI

Langages : SQL

📁 Structure du Répertoire

Data_set_files/ : Contient les fichiers sources au format CSV.

source_activites.csv

source_etudiants.csv

source_parents.csv

source_performances_CORRIGE.csv

separated_files/ : Contient la solution SSIS (.sln, .dtproj) et le package de flux de données (Package.dtsx).

script.sql : Script SQL de création des tables et de la structure de la base de données.

Visualisation.pbix : Fichier Power BI pour l'analyse visuelle des données.

🚀 Installation et Utilisation

1. Préparation de la Base de Données

Ouvrez SQL Server Management Studio (SSMS).

Exécutez le fichier script.sql pour créer les tables nécessaires (etudiant, parents, activite, performance, etc.).

2. Exécution de l'ETL (SSIS)

Ouvrez le projet separated_files.sln avec Visual Studio (avec l'extension SQL Server Data Tools installée).

Configurez les gestionnaires de connexion pour pointer vers vos fichiers CSV locaux et votre instance SQL Server.

Lancez le package Package.dtsx pour charger les données.

3. Visualisation

Ouvrez le fichier Visualisation.pbix avec Power BI Desktop.

Actualisez les données pour qu'elles se connectent à votre instance SQL Server locale.

📊 Analyse des Données

Le rapport Power BI permet de suivre :

Le taux de réussite des étudiants par activité.

L'influence de l'implication des parents sur les résultats.

L'évolution temporelle des performances académiques.

