# World Population Evolution Project

<br>

<p align="center">
<img width="594px" src='https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/Presentation/World_Population_Evolution_Snapshot.gif' />
</p>

<br>

Projet final de la formation Data analyst à [JEDHA BOOTCAMP](https://www.jedha.co/formations/data-analysis-fullstack).

Présentation (canva) : Vous pouvez accéder à la présentation [via ce lien](https://www.canva.com/design/DAGAp643_7U/81JnTZ1dDN2NLBIFqvu_mQ/edit?utm_content=DAGAp643_7U&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton).

<br>

## World Population Evolution

Préparer le monde de demain avec les tendences démographiques d'aujourd'hui.

<br>

### Introduction

Ce projet examine l'évolution démographique mondiale de 2000 à 2021, en mettant l'accent sur les variations des taux de natalité et de mortalité. L'importance de ces données réside dans leur capacité à éclairer les tendances sociétales et à guider la planification à long terme. L'objectif de l'analyse approfondie est d'identifier les facteurs clés sous-jacents à ces changements, fournissant ainsi des perspectives utiles pour les décideurs et les acteurs de la santé publique. En anticipant les défis liés à une population en mutation, l'étude vise à contribuer à des décisions stratégiques éclairées, favorisant un avenir plus équitable et durable sur le plan social, économique et environnemental.

<br>

### Données Utilisées

Les données utilisées proviennent de la World Bank Data, une source fiable de données socio-économiques mondiales. Dix-sept bases de données distinctes, couvrant divers aspects de la démographie mondiale, ont été collectées et soigneusement consolidées pour former une base exhaustive. Cette approche garantit une analyse robuste et de qualité de l'évolution de la population mondiale de 2000 à 2021.
Voici le lien vers la source des données: https://databank.worldbank.org/source/world-development-indicators#

Le tableau ci-dessous montre la significationde chaque colonne de notre dataset:

|     Colonnes                                  |     Significations                                                                                                                                                                                                                                                                                                                                                                                                              |
|-----------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|     Country Name                              |     Indique le   nom du pays auquel les données démographiques se rapportent. Chaque entrée   dans cette colonne identifie de manière unique le pays associé aux données de   population.                                                                                                                                                                                                                                       |
|     Country Code                              |     Codes géographiques alphabétiques ou numériques courts développés pour   représenter les pays et les zones dépendantes, utilisés dans le traitement   des données et les communications.                                                                                                                                                                                                                                    |
|     Year                                      |     Fait   référence à l'année correspondante pour laquelle les données démographiques   ont été enregistrées.                                                                                                                                                                                                                                                                                                                  |
|     Birth Rate                                |     Le taux brut   de natalité indique le nombre de naissances vivantes survenues au cours de   l'année, pour 1 000 habitants estimés à la mi-année.                                                                                                                                                                                                                                                                            |
|     Population_male                           |     La   population masculine est basée sur la définition de facto de la population,   qui compte tous les résidents masculins indépendamment de leur statut   juridique ou de leur citoyenneté.                                                                                                                                                                                                                                |
|     Population_female                         |     La   population féminine est basée sur la définition de facto de la population,   qui compte toutes les femmes résidentes indépendamment de leur statut   juridique ou de leur citoyenneté.                                                                                                                                                                                                                                 |
|     Population_total                          |     La   population totale est basée sur la définition de facto de la population, qui   compte tous les résidents indépendamment de leur statut juridique ou de leur   citoyenneté. Les valeurs indiquées sont des estimations en milieu d'année.                                                                                                                                                                               |
|     Median_age                                |     Correspond à   l'âge qui divise une population en deux groupes numériquement égaux,   c'est-à-dire que la moitié des personnes sont plus jeunes que cet âge et   l'autre moitié plus âgées. Il s'agit d'un indice unique qui résume la   répartition par âge d'une population.                                                                                                                                              |
|     Human   Development Index                 |     L'indice de   développement humain (IDH) est une mesure synthétique des dimensions clés du   développement humain : une vie longue et saine, une bonne éducation et un   niveau de vie décent. Des valeurs plus élevées indiquent un développement   humain plus important.                                                                                                                                                 |
|     PM2.5_pollution                           |     Représente   le niveau moyen d'exposition de la population d'un pays aux particules en   suspension d'un diamètre aérodynamique inférieur à 2,5 microns. Ces   particules, capables de pénétrer profondément dans les voies respiratoires,   peuvent causer des dommages importants à la santé.                                                                                                                             |
|     Urban   population rate                   |     La   population urbaine se réfère aux personnes vivant dans les zones urbaines   telles que définies par les bureaux nationaux de statistiques. Les données   sont collectées et lissées par la Division de la population des Nations   unies.                                                                                                                                                                              |
|     Death_Rate                                |     Le taux de mortalité est le rapport entre le nombre annuel de décès et la   population totale moyenne sur une période et dans un territoire donné. Cette   mesure statistique est notamment utilisée en démographie humaine,                                                                                                                                                                                                |
|     Population_15_64_rate                     |     Population   âgée de 15 à 64 ans en pourcentage de la population totale.                                                                                                                                                                                                                                                                                                                                                    |
|     Population_65_above                       |     Population   âgée de 65 ans et plus en pourcentage de la population totale.                                                                                                                                                                                                                                                                                                                                                 |
|     Cotisation   sociale                      |     Souvent   appelées charges sociales, sont des prélèvements assis sur les salaires. Les   cotisations font partie de la répartition opérée sur la richesse nationale   marchande créée au cours de l'année, ou PIB. Elles sont calculées sur la base   des salaires super-brut.                                                                                                                                              |
|     Life_expectancy_in_years                  |     L'espérance   de vie à la naissance indique le nombre d'années que vivrait un nouveau-né si   les taux de mortalité prévalant au moment de sa naissance restaient les mêmes   tout au long de sa vie.                                                                                                                                                                                                                       |
|     gov_health_exp_as_perc_of_gdp             |     Niveau des   dépenses courantes de santé exprimé en pourcentage du PIB. Les estimations   des dépenses courantes de santé comprennent les biens et services de santé   consommés chaque année. Cet indicateur n'inclut pas les dépenses de santé en   capital telles que les bâtiments, les machines, les technologies de   l'information et les stocks de vaccins pour les urgences ou les épidémies.                      |
|     undernourished_population_rate            |     La   prévalence de la sous-alimentation est le pourcentage de la population dont   la consommation alimentaire habituelle est insuffisante pour fournir les   niveaux d'énergie alimentaire nécessaires au maintien d'une vie normale,   active et saine.                                                                                                                                                                   |
|     population_rate_with_water_access         |     Représente   le pourcentage de personnes utilisant des services d'eau de base, y compris   ceux gérés en toute sécurité. Les services d'eau potable de base incluent   l'accès à une source améliorée, avec une limite de temps de collecte de 30   minutes pour un aller-retour.                                                                                                                                           |
|     mortality_cvd_crd_cancer_diabete_30_70    |     Représente   le pourcentage de personnes âgées de 30 ans qui décéderaient avant leur 70e   anniversaire en raison de maladies cardiovasculaires, de cancer, de diabète   ou de maladies respiratoires chroniques. Cette estimation se base sur les   taux de mortalité actuels à tous les âges et suppose que ces personnes ne   décéderaient pas d'autres causes de décès telles que les traumatismes ou le   VIH/sida.    |
|     uhc_service_coverage                      |     Couverture   des services de santé essentiels (définie comme la couverture moyenne des   services essentiels sur la base d'interventions traceurs comprenant la santé   reproductive, maternelle, néonatale et infantile, les maladies infectieuses,   les maladies non transmissibles et la capacité et l'accès aux services, parmi   la population générale et la population la plus défavorisée).                        |
|     population_growth_rate                    |     Le taux de   croissance de la population compare la variation annuelle moyenne en   pourcentage des populations, résultant d'un excédent (ou d'un déficit) des   naissances par rapport aux décès et du solde des migrants entrant et sortant   d'un pays. Le taux peut être positif ou négatif.                                                                                                                            |
|     Female_employment_rate                    |     Le taux d'emploi des femmes est la proportion de femmes   disposant d'un emploi parmi   celles en âge de travailler (15 à 64 ans).                                                                                                                                                                                                                                                                                          |
|     GDP per   Capita                          |     Le PIB par   habitant est le produit intérieur brut divisé par la population en milieu   d'année. Le PIB est la somme de la valeur brute ajoutée par tous les   producteurs résidents de l'économie, augmentée des taxes sur les produits et   diminuée des subventions non incluses dans la valeur des produits.                                                                                                           |
|     female_population_rate_15to44             |     Population   féminine âgée de 15 à 44 ans en pourcentage de la population féminine totale.                                                                                                                                                                                                                                                                                                                                  |
|     Continent   Name                          |     Spécifie le   continent auquel chaque pays appartient. Elle permet de regrouper les données   par continent, facilitant ainsi des analyses régionales.                                                                                                                                                                                                                                                                      |
<br>

### Méthodologie & Outils utilisés

| Etape | Outils utilisés |
|-------|-----------------|
| Data Cleaning & EDA | <img style="padding:2px" src="https://img.shields.io/badge/python-3776AB.svg?style=for-the-badge&logo=python&logoColor=black"/> <img style="padding:2px" src="https://img.shields.io/badge/pandas-150458.svg?style=for-the-badge&logo=pandas&logoColor=black"/> |
| Feature Importance Determination | <img style="padding:2px" src="https://img.shields.io/badge/dataiku-2AB1AC.svg?style=for-the-badge&logo=dataiku&logoColor=black"/> |
| Visualizations | <img style="padding:2px" src="https://img.shields.io/badge/Power%20BI-F2C811.svg?style=for-the-badge&logo=powerbi&logoColor=black"/> |

Les ensembles de données de la World Bank ont été importés dans Python via Pandas, puis traités individuellement pour uniformiser le format en vue d'une fusion. Le processus de fusion a créé une base de données complète pour notre analyse. Nous avons nettoyé la base en supprimant les colonnes superflues, remplaçant les valeurs manquantes par des données provenant d'Internet avec Pandas, et optimisé les types de données pour assurer une précision maximale. Cette approche méthodique garantit la qualité et la cohérence de notre ensemble de données final, formant une base solide pour une analyse approfondie de l'évolution de la population mondiale de 2000 à 2021.

<br>

### Analyse et Modélisation avec Dataiku

Pour approfondir notre compréhension des données, nous avons utilisé la plateforme d'analyse avancée Dataiku. Nous avons créé deux matrices de corrélation pour identifier les caractéristiques les plus influentes sur les taux de natalité et de mortalité. L'analyse de ces matrices a révélé des tendances significatives et des corrélations pertinentes entre les indicateurs. Ensuite, nous avons construit des modèles de régression linéaire pour le taux de natalité et de mortalité, fournissant des informations cruciales sur l'impact des caractéristiques. Cette approche a permis d'identifier les features les plus importantes, affinant notre compréhension des facteurs influençant la démographie mondiale de 2000 à 2021. Cette méthodologie, combinant analyse exploratoire et modélisation, renforce notre capacité à extraire des informations pertinentes et à éclairer les dynamiques complexes liées à la natalité et à la mortalité à l'échelle mondiale.

![Alt text](https://github.com/DimitriKneur/Demoday/blob/main/Presentation/dataiku_flow.png)

<br>

### Visualisations PowerBI

Un tableau de bord interactif construit dans PowerBI, visant à visualiser et analyser l'évolution de la population mondiale au fil des années, avec un focus particulier sur les données par continent. Le tableau de bord est conçu pour offrir une compréhension approfondie des tendances démographiques en relation avec différents indicateurs. [Visualizations_for_final_presentation.pbix](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/4_Data_Viz/Visualizations_for_final_presentation.pbix)

<br>

### Contenu du Tableau de Bord

### 1. Évolution de la Population par Année

La première page du tableau de bord présente une vue d'ensemble de l'évolution de la population mondiale au cours des années. Des graphiques temporels clairs permettent de suivre les variations démographiques et de repérer les tendances significatives.

<br>

### 2. Répartition de la Population par Continent

Les pages suivantes fournissent des analyses détaillées par continent, permettant aux utilisateurs d'explorer les différences et similitudes dans l'évolution démographique. Des filtres interactifs facilitent la sélection de plages temporelles spécifiques.

<br>

### 3. Analyse du Taux de Natalité et de Mortalité

Le tableau de bord propose des graphiques spécifiques mettant en évidence le lien entre le taux de natalité et de mortalité, en corrélation avec divers indicateurs. Ces visualisations permettent une compréhension approfondie des facteurs qui influent sur la dynamique démographique.

<br>

### 4. Recommandations et Insights

En plus des analyses des données, le tableau de bord inclut des graphiques interactifs visant à fournir des recommandations basées sur les tendances observées. Ces recommandations peuvent aider à orienter les prises de décision et les actions futures.

<br>

### Comment Comprendre le Code et les Répertoires

<br>

Après toutes les étapes de cleaning et de traitement, les 2 fichiers de données que nous avons utilisé pour faire nos visualisations dans Power BI sont [217_countries_population.csv](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/217_countries_population.csv) et [df_post_cleaning_4_force.csv](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/df_post_cleaning_4_force.csv). Ils ont été obtenus respectivement à l'issue de l'exécution des 2 scripts [217_countries_population.ipynb](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/217_countries_population.ipynb) et [merged_dataset_cleaning.ipynb](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/merged_dataset_cleaning.ipynb).

En effet, dans notre travail de groupe, nous avons rencontré une situation où nous disposions de deux jeux de données distincts, présentant certains chevauchements de colonnes, mais chacun couvrant un nombre différent de pays. Le premier jeu de données offrait des informations complètes sur 217 pays, mais avec un ensemble de colonnes moins étendu. En revanche, le deuxième jeu de données fournissait des données exhaustives sur seulement 157 pays, mais avec une variété de colonnes plus large. Cette configuration découle du fait que chaque membre du groupe étudiait parallèlement différents aspects des jeux de données, ce qui nous a amenés à adopter une approche d'alternance entre les jeux de données pour répondre aux besoins spécifiques de nos analyses. Bien que cette méthode ne soit pas optimale, elle nous a permis de tirer le meilleur parti des données disponibles malgré les contraintes.

Dans le détail, voici comment nous sommes arrivés à nos 2 fichiers finaux :

<br>

#### Etape 1 - Récupération des données des différentes sources et transformation de ces sources de données du wide format à un long format, dossier [1_Create_and_unpivot_datasets](https://github.com/DimitriKneur/World-Population-Evolution-Project/tree/main/1_Create_and_unpivot_datasets)

La plupart des fichiers ipynb correspondent à des fichiers de traitement (le nom de ces fichiers ipynb commence par "Prepare dataset") d'une ou plusieurs sources de données de 217 pays au mieux, sous format csv, de leur lecture grâce à pandas, jusqu'à l'export de chacune de ces sources données unpivotées dans de nouveaux fichiers csv séparés (le nom de ces nouveaux fichiers cvs commence par "Dataset"). Les autres fichiers ipynb sont des fichiers de lecture de ces sources de données pour de l'exploration préliminaire.

<br>

#### Etape 2 - Merge de toutes les sources de données unpivotées, dossier [2_Merge_datasets](https://github.com/DimitriKneur/World-Population-Evolution-Project/tree/main/2_Merge_datasets)

Dans le fichier [Merge_datasets.ipynb](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/2_Merge_datasets/Merge_datasets.ipynb), on importe tous les datasets créés, puis on les merge ensemble. On exporte ensuite le dataset mergé, contenant les informations de 157 pays (contre 217 dans certaines des sources de données initiales), dans un fichier nommé [joined_merged_final_dataset.csv](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/2_Merge_datasets/joined_merged_final_dataset.csv).

<br>

#### Etape 3 - Cleaning du dataset, dossier [3_Data_cleaning_on_merged_dataset](https://github.com/DimitriKneur/World-Population-Evolution-Project/tree/main/3_Data_cleaning_on_merged_dataset)

Le cleaning a été nécessaire sur 2 colonnes : le GDP et le female employment rate. Nous avons créé 2 fichiers de cleaning séparés, [Cleaning_GDP.ipynb](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/Cleaning_GDP.ipynb) et [female_employment_clean.ipynb](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/female_employment_clean.ipynb) pour effectuer le cleaning de ces 2 indicateurs, puis exporter les données cleanées de ces indicateurs respectivement dans les fichiers [df_GDP_cleaned.csv](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/df_GDP_cleaned.csv) et [female_employment_clean.csv](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/female_employment_clean.csv). 

Puis, dans le fichier [merged_dataset_cleaning.ipynb](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/merged_dataset_cleaning.ipynb), nous avons modifié les valeurs des colonnes correspondant à ces deux indicateurs pour les remplacer par les données cleanées des deux fichiers csv précédemment créés. L'aboutissement de tout ce process nous a permis d'obtenir le fichier [df_post_cleaning_4_force.csv](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/df_post_cleaning_4_force.csv).

En parallèle, nous nous sommes rendus compte que nous avions perdu les données démographiques de certains pays à cause des merges successifs entre les différentes sources de données lors de l'étape 2. Nous avons donc voulu rerécupérer ces données démographiques. Nous avons donc créé le fichier ipynb [217_countries_population.ipynb](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/217_countries_population.ipynb) dans ce but, afin d'avoir les données démographiques les plus exhaustives possibles pour certains indicateurs uniquement: il s'agit du taux de natalité, du taux de mortalité, population totale, population de 65 ans et plus, espérance de vie et taux de croissance de la population. Les données pour ces indicateurs ont été exportées vers le fichier [217_countries_population.csv](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/217_countries_population.csv).

Nous nous donc retrouvés avec deux fichiers de données finaux, [217_countries_population.csv](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/217_countries_population.csv) et [df_post_cleaning_4_force.csv](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/3_Data_cleaning_on_merged_dataset/df_post_cleaning_4_force.csv), le premier fichier étant plus exhaustif pour les indicateurs précédemment cités, et le second ayant tous les autres indicateurs pour compléter notre analyse. Ainsi, pour faire les visualisations, nous avons alterné entre ces 2 fichiers selon les données que nous souhaitions modéliser.

<br>

#### Etape 4 - Visualisation des données sur Power BI, dossier [4_Data_Viz](https://github.com/DimitriKneur/World-Population-Evolution-Project/tree/main/4_Data_Viz)

Dans ce sous-dossier figure un fichier pbix (Power BI) [Visualizations_for_final_presentation.pbix](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/4_Data_Viz/Visualizations_for_final_presentation.pbix) dans lequel figurent de nombreuses visualisations faites en exploitant les 2 fichiers finaux.

<br>

#### Présentation finale

Nous avons créé une [présentation](https://www.canva.com/design/DAGAp643_7U/81JnTZ1dDN2NLBIFqvu_mQ/edit?utm_content=DAGAp643_7U&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton) pour synthétiser tout le travail effectué. Vous trouverez [une version MP4 de cette présentation](https://github.com/DimitriKneur/World-Population-Evolution-Project/blob/main/Presentation/Data%20Analysis%20Fullstack%20Certification%20Project%20-%20Prepare%20the%20World%20of%20Tomorrow.mp4) à la racine du dossier [Presentation](https://github.com/DimitriKneur/World-Population-Evolution-Project/tree/main/Presentation). Dans le sous-dossier [Elements](https://github.com/DimitriKneur/World-Population-Evolution-Project/tree/main/Presentation/Elements), il y a des images, des icônes et différents contenus multimédia que nous avons utilisés pour alimenter cette présentation.

<br>

### Auteurs

*  [Nabil LALLAOUI](https://github.com/Nabil-LALLAOUI)
*  [Célia-Sijing XU](https://github.com/Celia-Siijing)
*  [Dimitri KNEUR](https://github.com/DimitriKneur)
*  [Nigel ZANNOU](https://github.com/Nigel95)
