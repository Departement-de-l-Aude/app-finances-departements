# Application d'Analyse Financière Départementale

_**Apperçu du site :**_
<img width="1918" height="1028" alt="gif_site_clement" src="https://github.com/user-attachments/assets/a6dc0fd9-64e9-445d-9f19-b48aca32c089" />

---

**Accéder à l'application en ligne : [lien](https://departement-de-l-aude-app-finances-departements-app.streamlit.app/)**  
**Consulter le tutoriel d'utilisation (PDF) : [pdf](https://github.com/user-attachments/files/30582839/tuto.utilisation.pdf)**

---

Ce dépôt contient le code source d'un tableau de bord interactif conçu pour analyser et comparer la santé financière des départements français, en exploitant les données publiques de l'OFGL.

## Fonctionnalités

Fonction 1 « Comparaison d'indicateurs d'un même département » 
- Affiche un seul graphe contenant tous les indicateurs du département choisi 
- Utile pour comparer deux dépenses ou observer un effet ciseaux 
- Possibilité de choisir l’intervalle des années 

Fonction 2 « Recherche de départements de même strate » 
- Renvoie un tableau contenant la liste des départements de même strate (avec leur numéro, nom et région) 
- Seule fonction pour laquelle les indicateurs ne sont pas pris en compte 
- Possibilité de restreindre la recherche aux départements provenant uniquement de la même région 

Fonction 3 « Comparaison d'indicateurs financiers entre plusieurs départements » 
- Renvoie un graphique par indicateur, dans lequel chaque courbe correspond à un département 
- Possibilité de choisir autant de départements que souhaité 
- Possibilité de choisir l’intervalle des années 

Fonction 4 « Département comparé à la moyenne de sa strate » 
- Renvoie un graphique par indicateur, dans lequel on trace une courbe pour le département et une courbe pour la moyenne des départements de même strate (moyenne dans laquelle on ne compte pas notre département pour ne pas la « fausser ») 
- Possibilité d’afficher la moyenne de la strate de la France métropolitaine (on appellera tout le temps métropole quand on sélectionne tous les départements français mais qu’on enlève les outre-mer) ET/OU de la même région 
- Possibilité de choisir l’intervalle des années 

Fonction 5 « Département comparé à la moyenne de sa strate et à la moyenne de la métropole » 
- Renvoie un graphique par indicateur, dans lequel on trace une courbe pour le département, une courbe pour la moyenne des départements de même strate et une dernière courbe pour la moyenne de tous les départements de la métropole 
- Possibilité de restreindre la moyenne des départements de même strate de la métropole à ceux de même strate ET de même région 
- Possibilité de choisir l’intervalle des années

> *Note : fonction assez similaire à la 4ème, offre une vue plus large*

## Stack Technique
* Python
* Streamlit (Interface Web)
* Pandas & NumPy (Traitement des données massives)
* Matplotlib & Seaborn (Data Visualisation)
