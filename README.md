# Cours SQL
Doc SQL (liste des fonctions existantes pour chaque langage SQL) : https://sqlpro.developpez.com/cours/sqlaz/fonctions/ 

## Les différentes jointures

### Cross Join

Un cross join, également appelé produit cartésien, est une opération dans les bases de données relationnelles qui combine chaque ligne d'une table avec chaque ligne d'une autre table. En d'autres termes, pour deux tables, A et B, un cross join va générer un ensemble de résultats qui contient toutes les combinaisons possibles des lignes de A et B.

Un cross join ne nécessite pas de clé primaire ou de condition de jointure entre les tables. 

Un cross join est utile lorsque vous souhaitez obtenir toutes les combinaisons possibles de deux ensembles de données. Par exemple, si vous avez une liste de produits et une liste de magasins, un cross join peut vous aider à créer un rapport de toutes les combinaisons de produits par magasin.

Étant donné que les cross joins peuvent générer un nombre de résultats très élevé (le nombre de lignes dans A multiplié par le nombre de lignes dans B), il est préférable de les utiliser avec des ensembles de données relativement petits pour éviter des performances médiocres.

### Inner Join

Un inner join renvoie les lignes qui ont des correspondances dans les deux tables. Seules les lignes ayant une condition de jointure vraie dans les deux tables sont incluses dans le résultat.

Utilisé pour récupérer les enregistrements qui ont des relations dans les deux tables, comme obtenir les clients et leurs commandes.

### Left Join (Left Outer Join)

Un left join renvoie toutes les lignes de la table de gauche et les lignes correspondantes de la table de droite. Si aucune correspondance n'est trouvée, les résultats de la table de droite contiendront NULL.

Utilisé lorsque vous souhaitez toutes les lignes d'une table (la table de gauche), même si elles n'ont pas de correspondance dans l'autre table.

### Right Join (Right Outer Join)

Un right join est l'inverse d'un left join. Il renvoie toutes les lignes de la table de droite et les lignes correspondantes de la table de gauche. Si aucune correspondance n'est trouvée, les résultats de la table de gauche contiendront NULL.

Utilisé lorsque vous souhaitez toutes les lignes d'une table de droite, même si elles n'ont pas de correspondance dans l'autre table.

### Full Join (Full Outer Join)

Un full join renvoie toutes les lignes lorsque des correspondances se produisent dans une ou les deux tables. Si aucune correspondance n'est trouvée, les résultats contiendront NULL pour les colonnes de la table sans correspondance.

Utilisé lorsque vous voulez combiner toutes les lignes des deux tables, que les correspondances existent ou non.

### Self Join

Un self join est une jointure d'une table à elle-même. Il permet de comparer des lignes dans la même table.

Utilisé pour des hiérarchies, comme dans un tableau d'employés où chaque employé a un manager également présent dans le même tableau.