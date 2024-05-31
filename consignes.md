## Installer l'application Symfony

modifie éventuellement les ports utilisés par les containers docker dans le fichier .env
 ```
DOCKER_MYSQL_PORT_3306=10308
DOCKER_APACHE_PORT_80=10290
 ```
Puis utilise les commandes suivantes pour installer le dépendances et mettre en place la base de données.

 ```bash
composer install
php bin/console d:m:m
php bin/console d:f:l
```


Si docker est installé localement: http://localhost:10290 devrait lancer l'application

## Consignes de l'exercice:

Voici une application qui présente la liste des membres de la fédération.

Le staff fédéral, client de cette application, ne trouve pas ça très pratique et formule la demande suivante:

> Pourrait-on avoir plutôt une vue sur le nombre de participants par groupes d'unité? Que pouvez-vous nous proposer de plus intéressant visuellement qu'un tableau?

Libre à toi d'installer les librairies que tu souhaites et de modifier le code existant pour répondre à cette demande.

Laisse parler ta créativité ;)

