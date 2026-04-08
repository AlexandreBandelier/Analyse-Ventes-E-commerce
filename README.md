# Analyse-Ventes-E-commerce
Analyse exploratoire du chiffre d'affaires (EDA) : Segmentation de gamme, analyse de concentration (Pareto) et insights stratégiques sur les mots-clés de conversion.


## Présentation du Projet
Ce projet consiste en une analyse approfondie des performances de ventes d'une boutique en ligne spécialisée dans l'équipement technique de niche. Il s'agit d'une entreprise réelle du milieu du sport, ce projet ayant été réalisé début mars 2026. L'étude porte sur un volume de 1 080 transactions s'étalant du 1er Janvier 2025 au 28 Février 2026.

**Objectif stratégique :** Déconstruire la structure du Chiffre d'Affaires (CA) pour identifier les leviers de croissance prioritaires et optimiser l'allocation des ressources marketing.

---

## Stack Technique et Méthodologie
Pour ce projet, j'ai mis en place un workflow hybride optimisant la productivité via l'IA :

* **Extraction :** Données brutes CSV exportées via WooCommerce.
* **Traitement de données :** Google Sheets (Nettoyage, calculs de Pareto, tableaux croisés dynamiques).
* **Intelligence Sémantique :** LLM (Large Language Models) utilisé pour le clustering de mots-clés, la catégorisation des gammes et l'analyse logique des leviers de croissance.

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



# E-commerce Sales Analytics: Segmentation and Pareto Optimization

## Présentation du Projet
Ce projet consiste en une analyse approfondie des performances de ventes d'une boutique en ligne spécialisée dans l'équipement technique de niche. Il s'agit d'une entreprise réelle du milieu du sport, ce projet ayant été réalisé début mars 2026. L'étude porte sur un volume de 1 080 transactions s'étalant du 1er Janvier 2025 au 28 Février 2026.

**Objectif stratégique :** Déconstruire la structure du Chiffre d'Affaires (CA) pour identifier les leviers de croissance prioritaires et optimiser l'allocation des ressources marketing via une approche assistée par intelligence artificielle.

---

## Stack Technique et Méthodologie
Le workflow de ce projet repose sur une utilisation avancée de l'IA pour compenser l'absence de scripts complexes ou de logiciels lourds, tout en garantissant une précision analytique.

* **Extraction et Stockage :** Données brutes au format CSV (WooCommerce).
* **Préparation des données :** Google Sheets (Nettoyage initial et mise en forme).
* **Moteur d'Analyse (LLM) :** Utilisation de l'IA pour l'exécution des calculs de segmentation, la génération des distributions de Pareto et la structuration des tableaux de synthèse.

### Focus : Ingénierie des Données et Workflow IA
Le dataset brut présentait des défis techniques résolus via une synergie entre le traitement manuel sur Google Sheets et l'analyse logique par l'IA :

* **Normalisation et Nettoyage (Google Sheets) :** Correction structurelle des types de données et des séparateurs décimaux. Désagrégation des catégories multiples via la fonction "Scinder le texte" pour isoler les labels produits et garantir la lisibilité du dataset.
* **Analyse de Pareto assistée (LLM) :** Délégation du calcul de concentration (80/20) au modèle de langue pour identifier les segments critiques du catalogue et isoler les 77 références générant l'essentiel du revenu.
* **Segmentation Logique et Analyse métier (LLM) :** Utilisation de l'IA pour définir les périmètres d'étude. L'IA a permis d'identifier que la comparaison inter-catégories (ex: Équipements de base vs Accessoires) était non-pertinente pour l'objectif visé, orientant l'étude vers une analyse granulaire par gamme de produits et par marque (i.e. de la catégorie de produits phare).

---

## Résultats de l'Analyse

### 1. Analyse de Concentration (Loi de Pareto)
L'étude, réalisée par traitement algorithmique des données, révèle une dépendance critique :
> **20% du catalogue (77 modèles clés) génère 84,18% du Chiffre d'Affaires total.**

### 2. Segmentation Détaillée par Gammes de Prix
| Segment de Prix | Nb Modèles | Volume Ventes | CA Généré | Prix Moyen |
| :--- | :--- | :--- | :--- | :--- |
| **Entrée de Gamme (< 60€)** | 97 | 1 321 | 47 353 € | 36 € |
| **Cœur de Marché (60€ – 105€)** | 92 | 2 067 | 170 094 € | 79 € |
| **Volume Premium (105€ – 150€)** | 78 | 859 | 105 223 € | 125 € |
| **Premium Technique (150€ – 200€)** | 48 | 778 | 132 040 € | 171 € |
| **Haute Performance (200€ – 250€)** | 39 | 491 | 114 074 € | 225 € |
| **Niche Exception (> 250€)** | 30 | 375 | 112 123 € | 308 € |

### 3. Cartographie des Partenariats Fournisseurs
L'analyse croisée (fournisseurs vs revenus) montre que 4 acteurs majeurs représentent 75% des revenus, avec une forte spécialisation par segment de valeur pour le Fournisseur D (Luxe) et le Fournisseur B (Volume).

---

## Intelligence Sémantique et Mots-Clés
L'analyse des 30 termes de recherche les plus liés au CA, traitée par LLM, montre que la conformité aux normes techniques est le premier moteur d'achat.

* **Top Mot-clé (Norme de Certification) :** Génère à lui seul 33% du CA global.
* **Insight :** La demande est tirée par la certification technique plutôt que par l'image de marque pure.

---

## Recommandation Actionnable
**Découvertes de l'analyse exploratoire :**
- La concentration de 33% du chiffre d'affaires sur un seul mot-clé, presque deux fois plus que le deuxième, n'avais pas été identifiée. Il s'agit du mot-clé correspondant à une certification de qualité.
- La répartition relativement uniforme de l'activité au-delà de la gamme d'entrée n'avait pas été identifiée. Le sentiment interne était que l'entreprise proposait principalement du haut-de-gamme, alors que la contraposée est vraie : l'entreprise est peu présente sur le bas-de-gamme, mais présente uniformémment sur toutes les autres gammes au-delà du bas-de-gamme.
- La concentration de 84€ du chiffre d'affaires sur 20% des produits, eux-mêmes presque exclusivement concentrés sur 4 marques, n'avait pas été identifiée.

**Recommendations :**
L'entreprise est concentrée sur 20% des produits, eux-mêmes composés de 4 marques pourtant distinctes dans leur segment de marché. Il s'agit donc d'un avantage et d'un inconvénient : l'entreprise a l'avantage d'opérer sur des segments diversifier, mais cela dilue également les efforts marketing et de communication. Le mot-clé majeur étant un dénominateur commun aux quatre segments, il faut centrer les efforts dans un premier temps sur ce segment commun.

---

## Structure du Dépôt
* **/data** : Dataset échantillon (Anonymisé).
* **/prompts** : Méthodologie et instructions utilisées pour faire calculer les Paretos et les segments par le LLM.
* **/viz** : Captures des synthèses générées par l'IA.

---
*Projet réalisé via une approche "AI-First" pour l'analyse de données e-commerce.*
