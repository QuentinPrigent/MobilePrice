# Notebooks d’expérimentation en IA quantique

## Présentation
Ce dépôt contient une série de notebooks Python réalisés dans un cadre **expérimental et pédagogique**.  
L’objectif est de mettre en place un flux de travail complet allant de l’analyse des données jusqu’à la comparaison de modèles classiques et quantiques, en appliquant un cas réel d’intelligence artificielle sur un **QPU (Quantum Processing Unit)**.

## Objectifs
- Illustrer un pipeline de machine learning standard appliqué à un jeu de données réel.  
- Fournir un cadre d’optimisation pour l’exécution sur un processeur quantique.  
- Comparer les performances des approches **classiques** et **quantiques**.  
- Sensibiliser aux opportunités et aux limites actuelles de l’IA quantique.  

## Contenu des notebooks
1. **Analyse des données**  
   - Exploration du jeu de données.  
   - Visualisation et mise en évidence des caractéristiques principales.  

2. **Préparation des données**  
   - Nettoyage et transformation des données.

3. **Modèles classiques**  
   - Implémentation de modèles de classification classiques.  
   - Mesure des performances.  

4. **Modèle quantique (QSVC)**  
   - Construction et entraînement d’un **Quantum Support Vector Classifier (QSVC)**.  
   - Comparaison avec les modèles classiques.  
   - Réflexion sur l’apport et les contraintes du quantique.  

## Remarques
- Le travail est **exploratoire** et ne prétend pas fournir de solution industrielle.  
- Les résultats peuvent varier selon la disponibilité et la qualité des ressources quantiques (simulateurs ou QPU).  
- L’objectif principal est de donner une **vision pédagogique** des enjeux et de la méthodologie.  

## Accès au QPU pour le notebook quantique

Le notebook `4 - Modèle quantique.ipynb` nécessite l'utilisation des **QPU d'IBM**. Pour cela, deux variables d'environnement doivent être configurées, et sont stockées dans un fichier `local.env` à créer à la racine du projet.  

### Étapes pour configurer l'accès :

1. Créer un compte sur la plateforme IBM Quantum : [https://quantum.cloud.ibm.com/](https://quantum.cloud.ibm.com/).  
2. Créer une instance sur la plateforme pour obtenir l'accès aux QPU.  
3. Récupérer le **token IBM** et l'**identifiant de l'instance**.  
4. Créer un fichier `local.env` à la racine du projet et y ajouter les variables d'environnement suivantes :

```
IBM_TOKEN=<votre token IBM>
IBM_INSTANCE=<votre identifiant d'instance>
```

Une fois ces variables configurées, le notebook pourra être exécuté en entier.
