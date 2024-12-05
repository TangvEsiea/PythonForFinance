# PythonForFinance - Equipe Atlas

## Description
Ce dépôt contient le code source de nos outils d'aides à la décision dans le cadre du projet du cours de python pour la finance.
Le dépôt contient deux fichiers : 
 - Projet_Atlas.ipynb contenant le code source.
 - HistoriqueAchatVente.xlsx contenant l'historique des transaction éfféctuées par Atlas

## Indicateur technique 1 - Model prédictif pré entrainer
Le premier système d'aide à la décision se base sur le model [Prophet](https://facebook.github.io/prophet/). Après plusieurs tests sur des échelles de temps différentes, nous avons décider d'entrainer le model sur les 20 derniers jours d'un asset donnée et projeter la prédiction future (sur une semaine) dans un graph. Cela permet de dégager une tendance court terme pour un asset donnée.

## Indicateur technique 2 - Analyse chartiste avec moyenne mobiles
Le deuxième indicateur technique consiste à projeter sur un même graph le cours d'un asset et trois moyennes mobiles. La plage de calcul des moyennes mobiles peut être modifier par l'analyste à souhait. Par défaut, nous partons sur des plages courtes (3, 5 et 10 jours) pour répondre aux exigences du challenge qui se déroule sur 1 semaine.

## Complétion de l'analyse
Ce dépôt contient uniquement le code pour l'aide à la décision technique. Les prises de décisions se couple avec une analyse macro (au niveau des actualités, de la situation politique, des actualités des entreprises, ...).
