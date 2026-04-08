# Analyse-Ventes-E-commerce
Analyse exploratoire du chiffre d'affaires (EDA) : Segmentation de gamme, analyse de concentration (Pareto) et insights stratégiques sur les mots-clés de conversion.


## Présentation du Projet
Ce projet consiste en une analyse approfondie des performances de ventes d'une boutique en ligne spécialisée dans l'équipement technique de niche. Il s'agit d'une entreprise réelle du milieu du sport, ce projet ayant été réalisé début mars 2026. L'étude porte sur un volume de 1 080 transactions s'étalant du 1er Janvier 2025 au 28 Février 2026.

**Objectif stratégique :** Déconstruire la structure du Chiffre d'Affaires (CA) pour identifier les leviers de croissance prioritaires et optimiser l'allocation des ressources marketing.

---

## Stack Technique et Méthodologie
Pour ce projet, j'ai privilégié une approche agile combinant des outils de calcul robustes et l'assistance de l'Intelligence Artificielle pour le traitement sémantique.

* **Extraction et Stockage :** Données brutes au format CSV (WooCommerce).
* **Moteur ETL et Nettoyage :** Google Sheets.
* **Analyse Prédictive et Clustering :** LLM (Large Language Models) pour la catégorisation des mots-clés et l'analyse de sensibilité.

### Focus : Ingénierie des Données (Data Cleaning)
Le dataset brut présentait des défis techniques majeurs résolus pour garantir l'intégrité de l'analyse :
* **Normalisation Numérique :** Correction des séparateurs décimaux erronés via des formules imbriquées `=VALUE(SUBSTITUTE(cell;".";","))`.
* **Désagrégation Sémantique :** Utilisation de l'IA pour scinder et nettoyer les métadonnées produits fusionnées.
* **Audit de Validité :** Correction des erreurs de typage (données numériques interprétées comme du texte) qui faussaient les classements par valeur.

---

## Résultats de l'Analyse

### 1. Analyse de Concentration (Loi de Pareto)
L'étude révèle une dépendance critique à une minorité de références :
> **20% du catalogue (77 modèles clés) génère 84,18% du Chiffre d'Affaires total.**

### 2. Segmentation par Gammes de Prix
| Segment | Tranche de Prix | Nb Modèles | CA Généré | Prix Moyen |
| :--- | :--- | :--- | :--- | :--- |
| **Volume Technique** | 60€ – 150€ | 170 | 275 317 € | 100 € |
| **Premium Technique**| 150€ – 250€ | 87 | 246 114 € | 195 € |
| **Niche Haute Valeur**| > 250€ | 30 | 112 123 € | 308 € |
| **Entrée de Gamme** | < 60€ | 97 | 47 353 € | 36 € |

### 3. Cartographie des Partenariats Fournisseurs
Le marché est porté par 4 acteurs majeurs représentant 75% des revenus. 
* **Fournisseur A (Leader Polyvalent) :** 27,8% des parts de marché.
* **Fournisseur B (Spécialiste Volume) :** 22,6% des parts de marché.
* **Fournisseur D (Spécialiste Luxe/Niche) :** 10,2% des parts de marché.

---

## Intelligence Sémantique et Mots-Clés
L'analyse des 30 termes de recherche les plus liés au CA montre que la conformité aux normes techniques est le premier moteur d'achat, devant la notoriété de marque.

* **Top Mot-clé (Norme de Certification) :** Génère à lui seul 33% du CA global.
* **Insight :** Les clients achètent une garantie de performance plutôt qu'un design.

---

## Recommandations Actionnables
1. **Optimisation Publicitaire :** Réorienter les campagnes vers les mots-clés liés aux certifications techniques.
2. **Gestion de Catalogue :** Consolider les relations avec les fournisseurs A et B pour sécuriser 50% du volume critique.
3. **Stratégie de Gamme :** Prioriser le développement du segment 105€-150€, identifié comme le point d'équilibre optimal entre marge et volume.

---

## Structure du Dépôt
* **/data** : Dataset échantillon (Anonymisé, proportions conservées).
* **/prompts** : Log des méthodologies utilisées pour le nettoyage via IA.
* **/viz** : Visualisations graphiques des segments et courbes de Pareto.

---
*Projet réalisé dans le cadre d'une étude d'optimisation de structure de données e-commerce.*
