Bonjour et bienvenue dans la partie 1 du cours Big Data. L'objectif de cette partie est de vous présenter les bases de données NoSQL (Not only SQL). Je vais commencer par quelques définitions et l'introductiosn d'un ensemble de vocabulaires. A la fin de cette première partie, vous serez capable d'installer et d'utiliser quelques systèmes de gestion de bases de données NoSQL, de mettre en place une architecture distribuées tolérante aux pannes. 

# Introduction générale  


De plus en plus le besoin de sauvegarder de très gros volumes de données se fait ressentir au sein des entreprises (même les plus petites). Les systèmes de gestion de bases données relationnelles ont certainement permis de sauvegerader et de gérer de manière efficace des données mais de quantité limitée. Les systèmes qui gèrent ce type de donnée ne passent pas l'échelle. 

# Qu'est ce que le passage à l'échelle ? 

# Brève introduction à XML 


# Brève introduction à JSON

Pour savoir si un document JSON est est correct, vous pouvez utiliser ce lien http://jsonlint.com/. 



# Théorème de CAP 

1. Consistency (Cohérence) : une donnée sauvegardé dans une base de données ne peut avoir plus d'un état visible quelque soit le nombre de replicas. 
2. Availability (Disponibilité) : une donnée est disponible 
3. Partition Tolerance (Distribution)


``Le théorème de CAP stipule que l'on ne peut pas respecter plus de deux propriètés parmi la cohérence, la disponibilité et la distribution.``

Il est évident qu'un système de gestion de base de données relationnel, que vous avez déjà étudiés, gèrent la cohérence et la disponibilité mais par la distribution. En effet, étudions les trois combinaisons possibles de ces caractéristiques : 

- CA (Consistency & Availability)
- B
- C


# Classement des systèmes de gestion de bases de données grâce au triangle de CAP

Ce triangle (donc trois critères), vous permet de choisir le système de gestion de bases de données qui répond au mieux à votre application. 

# Organisation de la suite de ce cours
La suite de ce cours est organisé comme suit.  Elle est décomposée en 9 parties. 

1. la partie 1 est consacrée la pérsentation de trois types de bases de données NoSQL (CouchDB, MongoDB et Casandra). 
2. la partie 2 présente  
