# Cours SQL

## Les différentes jointures

### Cross Join

Un cross join, également appelé produit cartésien, est une opération dans les bases de données relationnelles qui combine chaque ligne d'une table avec chaque ligne d'une autre table. En d'autres termes, pour deux tables, A et B, un cross join va générer un ensemble de résultats qui contient toutes les combinaisons possibles des lignes de A et B.

Un cross join ne nécessite pas de clé primaire ou de condition de jointure entre les tables. 

Quand utiliser un Cross Join ?
Combinaison exhaustive : Un cross join est utile lorsque vous souhaitez obtenir toutes les combinaisons possibles de deux ensembles de données. Par exemple, si vous avez une liste de produits et une liste de magasins, un cross join peut vous aider à créer un rapport de toutes les combinaisons de produits par magasin.

Ensembles de données de petite taille : Étant donné que les cross joins peuvent générer un nombre de résultats très élevé (le nombre de lignes dans A multiplié par le nombre de lignes dans B), il est préférable de les utiliser avec des ensembles de données relativement petits pour éviter des performances médiocres.