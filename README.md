# PHP App Example

## Requirements To Run Test
1. Docker


## How To Run Tests
#### Overview

1. Assurez vous que Docker soit en marche
2. Ouvrez un terminal
3. Rendez-vous dans le répertoire dans lequel se trouve le projet en utilisant la commande ci-dessous. Remplacez "chemin_vers_projet" par le chemin vers le répertoire du projet (php-app). 
```
cd chemin_vers_projet
```
4. Tapez la commande suivante : 
```
docker-compose up
```
Cela va permettre de construire et lancer les différents conteneurs nécessaires. Aussi, vous pourrez voir les logs de tous les conteneurs en cours d'exécution.

5. Une fois que cela est fait, ouvrez un nouveau terminal (sans fermer le précédent) dans le même dossier tel que décrit ci-dessus
Vérifiez le nom du conteneur docker associé à l'image 'rabbitmq:latest' grâce à la commande : 
```
docker ps
```
Si le nom est différent de 'php-app-rabbitmq-1' copiez le et rendez vous dans le fichier client.php, à la ligne 8, et remplacez le nom 'php-app-rabbitmq-1' par celui que vous venez de copier.

6. Enfin, rendez vous à l'adresse http://localhost:8080/client.php . Vous devriez voir s'afficher le message 'Sent Video To Server!'.

## Source
<https://github.com/ProdigyView-Toolkit/Microservices-Examples-PHP>