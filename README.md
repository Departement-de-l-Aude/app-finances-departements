# Application d'Analyse Financière Départementale

<img width="1918" height="1028" alt="gif_site_clement" src="https://github.com/user-attachments/assets/f7f4ac1d-ee02-431d-b5d0-016281f334bb" />

---

Ce dépôt contient le code source d'un tableau de bord interactif conçu pour analyser et comparer la santé financière des départements français, en exploitant les données publiques de l'OFGL.

## Fonctionnalités

L'application propose 5 modules d'analyse principaux :

### 1. Comparaison d'indicateurs d'un même département
* Affiche un seul graphique contenant tous les indicateurs du département choisi.
* Utile pour comparer deux dépenses ou observer un effet ciseaux.
* Possibilité de choisir l’intervalle des années.

### 2. Recherche de départements de même strate
* Renvoie un tableau contenant la liste des départements de même strate (avec leur numéro, nom et région).
* Seule fonction pour laquelle les indicateurs financiers ne sont pas pris en compte.
* Possibilité de restreindre la recherche aux départements provenant uniquement de la même région.

### 3. Comparaison d'indicateurs financiers entre plusieurs départements
* Renvoie un graphique par indicateur, dans lequel chaque courbe correspond à un département.
* Possibilité de choisir autant de départements que souhaité.
* Possibilité de choisir l’intervalle des années.

### 4. Département comparé à la moyenne de sa strate
* Renvoie un graphique par indicateur, dans lequel on trace une courbe pour le département et une courbe pour la moyenne des départements de même strate (moyenne dans laquelle le département analysé est exclu pour ne pas la fausser).
* Possibilité d’afficher la moyenne de la strate de la France métropolitaine (hors outre-mer) ET/OU de la même région.
* Possibilité de choisir l’intervalle des années.

### 5. Département comparé à la moyenne de sa strate et à la moyenne de la métropole
* Renvoie un graphique par indicateur comparant le département, la moyenne des départements de même strate, et la moyenne de tous les départements de la métropole.
* Possibilité de restreindre la moyenne des départements de même strate à ceux de la même région.
* Possibilité de choisir l’intervalle des années.
* *Note : Fonction similaire à la précédente, mais offrant une vue macroscopique plus large.*

## Stack Technique
* Python
* Streamlit (Interface Web)
* Pandas & NumPy (Traitement des données massives)
* Matplotlib & Seaborn (Data Visualisation)
