# Corpus web : une cartographie Web de l'écosystème IA en France - médialab Sciences Po - 2019

Ce dépot héberge les données au format GEXF ([Gephi](https://gephi.org)) de la cartographie du web réalisée dans le cadre de l'analyse exposée à l'adresse suivante : https://medialab.sciencespo.fr/actu/une-cartographie-web-de-lecosysteme-ia-en-france/
Vous pouvez les télécharger en [cliquant sur ce lien](https://raw.githubusercontent.com/medialab/AI-ecosystem-carto-data/master/Carto_Web_ecosysteme_IA_FR_2019_LO_medialab_SciencesPo.gexf). 

## Présentation 

Qui sont les acteurs de l’écosystème IA français ? Quelles relations entretiennent-ils sur le Web ?
Cette cartographie, sans prétendre à l’exhaustivité, tente de rendre compte de la composition et de la structure relationnelle des différents acteurs de l’IA en France sur le Web. Elle laisse apercevoir une segmentation entre plusieurs communautés d’acteurs majeures que sont les acteurs économiques (startups, incubateurs, etc.), les laboratoires et équipes de recherche en intelligence artificielle, ainsi que les communautés de développeurs qui se retrouvent autour d'événements (meetup) et les repository (Github) qui dessinent un réseau socio-technique d’acteurs variés (code logiciel, page de développeurs, de projet, d’équipe ou d’entreprise) interconnectés entre eux. 


## Méthodologie

Cette cartographie du web a été réalisée en en Septembre 2019 à partir de données extraites du Web au printemps 2019 à partir du logiciel de crawl Hyphe. Le corpus a été principalement constitué par quatre sites de départ (https://www.hub-franceia.fr ; https://franceisai.com/ ; https://cartographie-ia.enseignementsup-recherche.pro/acteurs.php# ; https://aiparis.fr/2019/) qui agrègent des listes d'acteurs français (recherche, startup) autour de l'IA dans divers domaines. A ces principaux sites ont été ajoutés 15 sites web (articles de presse, incubateurs, communauté de développeurs) recensant également des acteurs dans le domaine de l'intelligence artificielle.Ce corpus de départ a permis de récupérer une première série de web entités (Jacomy et al, 2016) en effectuant un crawl de profondeur n+1. De manière itérative un travail de nettoyage a consisté à crawler les nouvelles entités découvertes en lien avec la thématique (startup, incubateur, recherche, communauté) et à supprimer les entités non associées à la France, hors de la thématique concernée, les sites de presse et les sites inactifs. Afin de clôturer le crawl, il a été décidé de supprimer toutes les entités dont le degré (nombre de liens hypertextes) était inférieur à 3 avec le corpus constitué. Par conséquent, certains acteurs de l'IA ayant peu d'interconnexions sur le web ne figurent pas dans la cartographie. Un travail de catégorisation à la main de toutes les entités a été effectué avant d’identifier les types d'acteurs qui composent le réseau. Le graphe final visualisé à partir du logiciel d'exploration de réseaux Gephi est composé de 1562 entités web reliées entre elles par un ensemble de 5313 liens hypertextes. La taille de nœuds est relative au degré des entités web (le nombre de liens hypertextes qui les connecte au reste du graphe). Les couleurs sont relatives à la modularité qui détecte et catégorise automatiquement les sous-ensembles qui forment des zones plus denses dans le réseau. On observe 4 clusters principaux (modularité avec une résolution de 1.5 en aléatoire) de taille assez inégale, et dont la structure est assez stable (plusieurs itérations de l'algorithme de modularité), seul deux clusters d'environ une dizaine d'entités web ont été associés à un cluster proche plus important pour faciliter la lecture de l'ensemble.

_NB :_ Ce réseau ne prétend pas être exhaustif, du fait de contraintes techniques liées aux outils de crawl ou du ciblage du sourcing certains acteurs de l'écosystème liés à l’intelligence artificielle peuvent ne pas y être présents. Par ailleurs, le terme d'intelligence artificielle est à prendre ici dans une acceptation large, tout acteur qui présente ou déclare avoir tout ou partie de ses activités liées à l'IA est ainsi considéré comme dans la thématique.


## Caractéristiques du corpus

Nombre d’entités web : 1562 
Nombre de liens : 5313
Graphe dirigé : Oui 


## Description des métadonnées

- `ID` : identifiant hyphe de l’entité web 
- `Label` : nom de l’entité web
- `Cluster` : Catégories interprétées des classes de modularité produites dans Gephi 
- `Homepage` : URL de l’entité web 
- `Indegree` : nombre de liens entrants de l’entité web
- `Outdegree` : nombre de liens sortants de l’entité web 
- `Degree` : nombre de liens de l’entité web
- `Type_acteur` : Catégories manuelle des entités (voir détail ci-dessous)

Détail de la catégorie `Type_acteur` :
- `research` : école, université, projet ou laboratoire de recherche public et privé, logiciels techniques issus de la recherche, site de communication recherche 
- `institution` : niveau Européen et national, ministères, collectivités territoriales, soutien au développement économique
- `incubator` : incubateurs territoriaux, incubateurs liés à des écoles ou privés 
- `startup` : sociétés spécialisées mettant en avant une partie de leur activité en lien avec l’IA 
- `company` : grands groupes et sociétés françaises ou internationales avec une activité en France (domaines variés : technologie, télécom, transport, énergie, santé, etc.)
- `finance` : banques, assureurs, fonds de capital risque 
- `community` : page de groupes et de rencontre autour de l’IA meetup 
- `repository` : pages github (personnes, équipe, projets, entreprise, recherche) 
- `event` : colloque, , conférences, compétitions


## Crédits

- Maxime Crépel, médialab SciencesPo
- Jean-Marie John-Mathews, médialab SciencesPo
- Dominique Cardon, médialab SciencesPo
- [médialab Sciences Po](https://medialab.sciencespo.fr)

_Contact :_ maxime.crepel [ AT ] sciencespo [ DOT ] fr


## Licence
Ces données sont publiées en Open Data sous les conditions de la [Licence Ouverte](https://www.etalab.gouv.fr/licence-ouverte-open-licence), vous pouvez les réutiliser librement en citant les auteurs et en pointant l'url de ce site comme source.
