# Power-BI-project-Comptoir-DataBase
Mise en Place d'un Écosystème BI &amp; Data Mining : Cas ComptoirDB Ce projet présente une architecture décisionnelle complète,de la modélisation de données opérationnelles à l'analyse prédictive et la visualisation interactive, afin de transformer les données brutes de la base en indicateurs stratégiques pour le pilotage commercial et logistique.

🛠️ Stack Technique 
L'originalité de ce projet réside dans l'intégration de technologies leaders du marché pour couvrir l'ensemble de la chaîne de valeur de la donnée :

Talend Open Studio (ETL) : Pivot central du projet, utilisé pour concevoir des flux de traitement robustes. Il a permis l'extraction, la transformation complexe (via le composant tMap) et le chargement des données vers l'entrepôt.


SQL Server & SSAS : Hébergement de l'entrepôt de données modélisé en étoile (R-OLAP). La création d'un cube OLAP via Analysis Services permet des analyses multidimensionnelles ultra-rapides sur des volumes importants.

Power BI : Transformation des données en intelligence visuelle. Création de tableaux de bord dynamiques connectés en temps réel au cube SSAS pour une aide à la décision intuitive.

Weka (Data Mining) : Application de l'algorithme K-Means pour segmenter la clientèle. Cette étape apporte une valeur prédictive en identifiant, par exemple, les clusters de clients subissant des retards de livraison critiques.

🏗️ Architecture du Projet
Le projet suit une méthodologie rigoureuse en trois grandes phases :

1. Modélisation Décisionnelle
Passage d'un schéma relationnel complexe à un schéma en étoile optimisé.

Définition de dimensions clés : Temps (granularité jour/mois/année), Client, et Produit.

Centralisation des métriques dans une Table de Faits (Ventes).

2. Pipeline ETL avec Talend
Développement de jobs spécifiques pour chaque dimension.

Nettoyage et mapping des sources de données pour garantir l'intégrité de l'entrepôt.

Calcul d'indicateurs avancés : Chiffre d'Affaires Net, Taux de service, et retards de livraison.

3. Analyse & Visualisation

Pilotage Commercial : Analyse du CA par catégorie de produits et impact des remises.


Optimisation Logistique : Suivi du "Danger de Rupture" et analyse géographique des délais de livraison.


Segmentation Clients : Utilisation du clustering pour différencier les zones performantes (ex: Occitanie) des zones critiques (ex: Île-de-France).

📈 Indicateurs Clés de Performance (KPIs) implémentés

CA Brut vs CA Net : Mesure de la performance financière réelle après remises.


Taux de Service : Indicateur de satisfaction client et d'efficacité logistique.


Délai Moyen de Livraison : Identification des goulots d'étranglement dans la chaîne d'approvisionnement
