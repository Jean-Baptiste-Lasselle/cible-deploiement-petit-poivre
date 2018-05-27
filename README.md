# Cuisine

Ce repository versionne le code source d'une rectte de provision d'une cible de déploiement.

Cette recette est l'un des composants d'une expérimentation mettant en jeu:
* une application jee web, avec client angular 5, et base de données mongodb:
  * la partie Java de l'application est versionnée par le repository [petit-poivre-jee](https://github.com/Jean-Baptiste-Lasselle/petit-poivre-jee)
  * la partie Java de l'application est versionnée par le repository [petit-poivre-angular5](https://github.com/Jean-Baptiste-Lasselle/petit-poivre-angular5)
* un plugin maven à la vue perçante [petit-duc-mvn-plugin](https://github.com/Jean-Baptiste-Lasselle/petit-duc-mvn-plugin)
* une recette de provision d'une cible de déploiement tomcat / mongodb "dockerisée",  versionnée par le repository [petit-poivre-cible-deploiement](https://github.com/Jean-Baptiste-Lasselle/cible-deploiement-petit-poivre)


Le but de l'expérimentation est de proposer un processus de développement, et les outils qui permettent de le mettre en oeuvre, pour deux 
équipes séparées géographiquement et/ou technologiquement, et travaillant sur la même application.

L'intention est de chercher comment une équipe technique peut faire du pilote de projet 
un homme aux 5 sens augmentés.


# Ingrédients


Cette recette de déploiement permet de monter une cible de déploiement:
* conteneur docker Tomcat
* conteneur docker mongodb

Les conteneurs peuvent:
* être démarrés individuellement, avec support du CHECK_HEALTH
* être démarré et orchestrés par docker-compose (cf. fichier docker-compose.yml)
<!-- * À venir: être démarrés et orchestrés par Kubernetes -->


# TODOs


## TODO: plan de travail

Garder les mêmes varibles d'environment, les mêmes noms de scripts, essayant de ne faire que remplacer le mot "mariaDB", par le mot "mongoDB".
[référence 1](https://www.mongodb.com/blog/post/getting-started-with-mongodb-and-java-part-i)]

La recette de base est prévue pour ubuntu, la transposer pour un hôte DOcker CentOS.





