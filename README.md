# DockerAMP
Serveur Docker léger Php / Mysql 

Machine docker Apache/ php
Base de donnée MySql

### Prérequis
Docker installé ( perso en Version 18.03.1-ce-mac65 (24312))
 

### Config
Ajouter le fichier .env contenant :

```
MYSQL_ROOT_PASSWORD=[mot de passe root sql]
MYSQL_DATABASE=[nom de la base]     
MYSQL_USER=[nom du user par default]
MYSQL_PASSWORD=[et son mot de passe]
```

### Initialisation
Dans un terminal :
```
docker-compose up -d
```
à la fin de la récuperation , executer :

```
docker ps
```

Vous devriez obtenir un truc dans le genre  :
```
CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS              PORTS                NAMES
f3c7b5eeb7f5        mysql               "docker-entrypoint.s…"   11 hours ago        Up 24 seconds       3306/tcp             dockeramp_db_1
13602429972c        php:7.1-apache      "docker-php-entrypoi…"   11 hours ago        Up 24 seconds       0.
```
