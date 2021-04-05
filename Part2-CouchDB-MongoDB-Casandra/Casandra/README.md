# Système de gestion de bases de données NoSQL Casandra

Comme pour les deux systèmes NoSQL CouchDB et MongoDB, l'objectif dans ce qui suit est de vous introduire Casandra. Pour répondre aux problamétiques de stockage et de gestion de très gros volumes de données à grande échelle, un groupe d'ingénieur de Facebook (2007) ont proposé Casandra. Avant qu'elle ne soit portée par Incubator, en 2010, Casandra n'a pas eu de succès. Depuis, elle est elle promu au rang de top-level Apache Project. Actuellent, c'est la socièté Datastax qui gère le support et la distribution de Casadra. Elle rest sur un projet Open Source de la fondation Apache.

``Casadra a beaucoup évolué, ce qui explique une terminologie assez différentes et qui portent à confusion.  Son point de départ est le système BigTable de Google.`` 

Je vais commencer dans la section suivante par vous montrer comment l'installer et l'utiliser.

``Attention, en cas où vous utilisez une autre vesrion de Casadra  que celle que j'ai utilisée pour rédigé ce support de cours, je vous renvoie à la documentation officielle. Il peut y avoir des différences d'installation d'une vesrion à une autre``. 

# Installation 
Pour installer sur votre machine, on peut soit : (i) l'utiliser comme une image Docker ou (ii) télécharger les binaires de Casandra. Je vais vous montrer les deux méthodes dans ce qui suit. 

### Installation du serveur Casandra via Docker
Casadra peut être utilisé dans un système virtualisé de manière très simple (si on n'est pas bien avancé sur la partie ``conteneurisation``, je vous invite à passer directement à la section suivante).  Vous pouvez soit utiliser l'interface graphique ``Kitematic`` ou la ligne de commande suivante : 

``docker run --name cmcassandra -p 8686:9042  -d cassandra:latest``. Le port d'écoute par défaut de Casandra 9042 est donc renvoyé vers le port 8686 du système hôte.  Vous pouvez à présent vous connecter à Casandra et commencer à l'utiliser.  Pour cela, on aura besoin d'un client, à l'image de phpMyAdmin qui est une application web  (client graphique) pour les systèmes de gestion de base de données MySQL et MariaDB, écrite principalement en PHP et distribuée sous licence GNU GPL.  
 
 ### Installation des binaires du serveur Casandra
 La deuxième façon consiste à télécharger les binaires que vous pouvez trouvé à l'adresse suivante http://www.google.fr . 
 
 ``Pour ce qui souhaitent, et c'est ce que je vous conseille dans un premier temps, utiliser la même vesrion que moi, vous pouvez à la télécharger à l'adresse suivante http://www.google.fr``

## Installation d'un client pour Casandra



