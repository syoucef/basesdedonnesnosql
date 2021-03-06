# Système de gestion de bases de données NoSQL Casandra

Comme pour les deux systèmes NoSQL CouchDB et MongoDB, l'objectif dans ce qui suit est de vous introduire Casandra. Pour répondre aux problamétiques de stockage et de gestion de très gros volumes de données à grande échelle, un groupe d'ingénieur de Facebook (2007) ont proposé Casandra. Avant qu'elle ne soit portée par Incubator, en 2010, Casandra n'a pas eu de succès. Depuis, elle est elle promu au rang de top-level Apache Project. Actuellent, c'est la socièté Datastax qui gère le support et la distribution de Casadra. Elle rest sur un projet Open Source de la fondation Apache.

``Casandra a beaucoup évolué, ce qui explique une terminologie assez différentes et qui portent à confusion.  Son point de départ est le système BigTable de Google.`` 

Je vais commencer dans la section suivante par vous montrer comment l'installer et l'utiliser.

``Attention, en cas où vous utilisez une autre vesrion de Casadra  que celle que j'ai utilisée pour rédigé ce support de cours, je vous renvoie à la documentation officielle. Il peut y avoir des différences d'installation d'une vesrion à une autre``. 

# Installation 
Pour installer sur votre machine, on peut soit : (i) l'utiliser comme une image Docker ou (ii) télécharger les binaires de Casandra. Je vais vous montrer les deux méthodes dans ce qui suit. 

### Installation du serveur Casandra via Docker
Casadra peut être utilisé dans un système virtualisé de manière très simple (si on n'est pas bien avancé sur la partie ``conteneurisation``, je vous invite à passer directement à la section suivante).  Vous pouvez soit utiliser l'interface graphique ``Kitematic`` ou la ligne de commande suivante : 

``docker run --name cmcassandra -p 8686:9042  -d cassandra:latest``. Le port d'écoute par défaut de Casandra 9042 est donc renvoyé vers le port 8686 du système hôte.  Vous pouvez à présent vous connecter à Casandra et commencer à l'utiliser.  Pour cela, on aura besoin d'un client, à l'image de phpMyAdmin qui est une application web  (client graphique) pour les systèmes de gestion de base de données MySQL et MariaDB, écrite principalement en PHP et distribuée sous licence GNU GPL.  
 
 ### Installation des binaires du serveur Casandra
 La deuxième façon consiste à télécharger les binaires que vous pouvez trouvé à l'adresse suivante http://www.google.fr. 
 
 ``Pour ce qui souhaitent, et c'est ce que je vous conseille dans un premier temps, utiliser la même vesrion que moi, vous pouvez à la télécharger à l'adresse suivante``  http://www.google.fr. 
 
 Une fois le dossier décompressé, il suffit de lancer suivant votre système d'exploitation casandra.sh pour Linux et Mac et casandra.bat pour windows. Le port d'écoute par défaut de Casandra est 9042. Pour arrêtre Casandra, il vous suffira d'appuyer simultanément sur ``ctrl+c``. 

## Installation d'un client pour Casandra

Il existe plusieurs clients Casadra, au moment où je rédige ce cours, il me semble que le plus complet est le Datastax DevCenter. C'est ce client que j'utilise. Je vous invite à tester d'autres clients si vous le souhaitez. Vous pouvez télécharger la derbière version, en utilisant ce lien https://downloads.datastax.com/#devcenter. Sinon, je mets à votre disposition les binaires que j'utilise à l'adresse suivante http://www.google.fr.   


La figure suivante vous montre l'interface graphique de Datastax, avec ses différentes fenêtres pour explorer le shéma d'une base, de l'interroger, en utilisant le langage CQL, que je vais vous présenter ultérieurement. 

<center>
<img src="images/datastax.png" alt="drawing" WIDTH=600 HEIGHT=400"/>
</center>



# Les modèles de données
Au début Casandra était un système de gestion de bases de données permissif. Autrement dit, on peut insérer des données qui n'ont rien avoir les unes des autres (à l'image de CouchDB et MongoDB). Par la suit, il s'est orinté vers un modèle dit relationnel étendu, avec un typage fort et un shéma.  ET c'est là justement la différence principale par rapport à tous (à ma connaisance .... si ce n'est le cas, n'hésitez pas à me l'apprendre SVP) les systèmes de gestion de bases de données NoSQL. Une base de données Casandra est constitué, comme pour un modèle relationnel, de tables. Chaque table est constituée d'un ensemble de colonnes

## Paires clé/valeur (columns) et documents (rows)

## Les tables (column families)

## Les bases (Keyspaces)

####  Utilisation de cqlsh

 pip install cqlsh``

## La langage de requête CQL (Cassandra Query Language) de Casandra 

Pour plus d'information sur CQL, je vous encourage à consulter sa documentation officielle que vous pouvez trouver à l'adresse suivante https://cassandra.apache.org/doc/latest/cql/. 




