# Bayes- Birats: a bivariate normal hierarchical model


## Description du Projet
Ce projet implémente le modèle Birats, un modèle hiérarchique bivarié normal, pour analyser les données de croissance de rats. Inspiré par le travail de Gelfand et al. (1990), ce modèle utilise une distribution normale multivariée pour les coefficients de régression des courbes de croissance de chaque rat, permettant d'étudier la corrélation entre le poids initial (intercept) et le taux de croissance (pente).

## Structure du Modèle
* Données: Poids des rats mesurés à différents âges.
* Paramètres du Modèle:
  	- mu_beta: Moyennes des coefficients de régression. \n
    - Sigma_beta: Matrice de précision de la population pour les coefficients.
    - tauC: Précision des mesures.
* Distributions Prior:
	- Coefficients de régression suivent une distribution normale multivariée.
	- Priors non-informatifs pour mu_beta.
	- Prior Wishart pour Sigma_beta.
	- Prior Gamma pour tauC.

## Fichiers dans le Répertoire
- bayes_birats_code.ipynb: Notebook Jupyter contenant le code pour la modélisation et l'analyse.
- projet_birats.Rmd : Une autre version améliorée qu'on a pu le réalisée contenant le code en R.
- WinBUGS_Vol2-23-25.pdf: Document PDF fournissant les détails et les résultats originaux du modèle utilisant WinBUGS. https://mribatet.perso.math.cnrs.fr/CentraleNantes/BAYES/Grading.pdf
- Rapport : https://www.overleaf.com/project/66198a8d696e5baf8f4cd0ad

## Résultats Attendus
Le notebook comprend des analyses des postérieurs, y compris les moyennes, écarts types, et intervalles crédibles pour chaque paramètre. Des visualisations de la convergence des chaînes MCMC et des distributions postérieures sont également fournies.

### Travail réalisé par :
* Lamiae ARIFALLAH
* Rim YOUSFI
* Meryem Cherqi

### Encadré par  : Ribatet Mathieu
