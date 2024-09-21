
# Prévisions des ventes d'une entreprise après différentes campagnes publicitaires

## Overview

L'objectif de ce projet était de créer un modèle de régression linéaire multiple pour prédire les ventes et de déterminer d'éventuels insights qui peuvent aider l'entreprise à améliorer ses ventes. Dans ce projet nous avons utilisé les données des différentes types de campagnes de marketing pratiquées dans une entreprise. Les différentes variables retenues sont les dépenses de publicités pour la 'Radio et la 'Tv'. Cette dernière est classée en niveau 'faible', 'moyenne' et 'élevée'. Le modèle explique 91,12 % des ventea et la moyenne des ventes est inférieure pour les catégories de dépenses moyennes ou faibles par rapport à la catégorie de dépenses élevées; lorsque les dépenses radio sont maintenues constantes.

## Business Understanding

L'entreprise souhaite maximiser ses ventes par le biais de campagnes de marketing efficaces. Il est essentiel de comprendre comment chaque canal contribue aux résultats. Ainsi nous allons identifier les canaux qui permettent d'optimiser les investissements en marketing et des solutions basées sur les résultats de l'analyse.

## Data Understanding

Les données utilisées dans ce projet proviennent de [Dummy Marketing and Sales Data](https://www.kaggle.com/datasets/harrimansaragih/dummy-advertising-and-sales-data). Les données comprenaient environ 4546 campagnes de marketing uniques et 5 caractéristiques. Parmis ces caractéristiques on peut citer les ventes réalisées, les budgets de publicités alloués à la télévision, à la radio, aux réseaux sociaux et aux influenceurs. Le graphique ci-dessous montre la relation entre les ventes effectuées et les variables 'Tv' et 'Réseau Social'.


![image.png](attachment:image.png)

Dans le même ordre d'idées, une ingénieurie des caractéristiques a été mise au point pour indiquer si le budget alloué aux dépenses de télévision est faible ou moyenne ou élevée. Des entrées redondantes ont été supprimées.

## Évaluation de modèles


Un modèle de régression linéaire multiple a été utilisé pour évaluer l'impact des budgets de publicité sur les ventes. La variable 'Tv' est une variable catégorielle et sa variable par défaut est "High". 

$$Sales = 218.5261 - 154.2971 * TV_Low - 75.3120 * TV_Medium + 2.9669 * X_Radio$$

Le modèle affiche un R² de 91,12 % et que toutes les variables retenues sont significatives au seuil de 1%. Le modèle respect toutes les hypothèses nécessaires à sa validitée.



## Conclusion
L'analyse indique que le budget alloué à la télévision est le facteur principal influençant les ventes, suivi par celui dédié à la radio. En revanche, les investissements dans les réseaux sociaux et les influenceurs semblent avoir un impact limité.

Il est recommandé à l'entreprise:

- d'augmenter le budget promotionnel destiné à la télévision;
- d'investir dans des campagnes radio pour stimuler les ventes; 
- de reconsidérer la stratégie concernant les réseaux sociaux.
