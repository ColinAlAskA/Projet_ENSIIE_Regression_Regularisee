# Projet de régression régularisée

Projet réalisé dans le cadre de l'UE **Régression Régularisée**, en deuxième année
à l'ENSIIE.

## Auteurs

- Colin Coërchon
- Léos Coutrot

**Chargé de projet :** Kylliann De Santiago  
**Responsable de l'UE :** Mathilde Mougeo

## Présentation du projet

Nous disposons d'un jeu de données comprenant **37 variables et 4 424
observations**, recueillies auprès d'élèves de l'Institut polytechnique de
Portalegre, au Portugal, entre 2009 et 2019. Le jeu de données est complet et
ne présente aucune donnée manquante.

Les variables décrivent notamment le genre, l'âge et le niveau d'études des
parents, ce qui permet d'étudier différents aspects de l'environnement familial
des élèves.

La question centrale du projet est la suivante :

> Quelles sont les variables ayant un impact significatif sur la performance
> scolaire des étudiants ?

La variable cible est binaire :

- `1` si l'élève a obtenu son diplôme ;
- `0` sinon.

## Méthodes

Pour répondre à cette question, nous avons utilisé plusieurs modèles de
régression logistique :

1. Des modèles de régression logistique simples
2. Une régression Ridge ($\ell_2$)
3. Une régression Lasso ($\ell_1$)
4. Une régression Elastic net.

Ces méthodes permettent d'identifier les variables les plus pertinentes pour
la réussite académique et de construire un modèle prédictif capable d'identifier
les étudiants susceptibles d'être en difficulté.

Le meilleur résultat obtenu atteint une précision de **0.86**.

## Contenu du dépôt

- `Projet_Rapport_Coerchon_Coutrot.Rmd` : rapport et analyses réalisés en R Markdown ;
- `data.csv` : jeu de données utilisé pour les analyses ;
- `preambule.tex` : préambule LaTeX contenant des commandes et réglages utilisés
  pour améliorer la mise en forme du rapport PDF ;
- `Projet_Rapport_Coerchon_Coutrot.pdf` : rapport PDF compilé ;
- `Diapo_MERR_Coerchon_Coutrot.pdf` : supports de la présentation orale du
  18 décembre 2023.

## Compilation du rapport

Le rapport est conçu pour être compilé au format **PDF**. La compilation au
format HTML est possible, mais le fichier `preambule.tex` n'y est pas pris en
compte et le rendu est donc moins fidèle à la version finale.

Pour reproduire les résultats, ouvrir `Projet_Rapport_Coerchon_Coutrot.Rmd`
dans RStudio, puis sélectionner **Knit > Knit to PDF**.
