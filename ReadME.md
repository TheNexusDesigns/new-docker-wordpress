# Run this to make docker wordpress working
     
> 1. build containers
   
    docker-compose up -d

> 2. make container volume files on host system readable by apache and linux user. (change path to container location).


    sudo chown -R ubuntu:ubuntu ~/containers/wordpress-env
    sudo chown -R www-data:www-data ~/containers/wordpress-env



# Rebuild Containers Commands
  >needs to be run where docker-compose.yaml is.

## 1. kill docker-containers without deleting or affecting site edits
    docker-compose kill

## 2. Now rebuild docker containers without affecting site edits
    docker-compose up -d --build

#

## Some useful Docker Commands
    #To Tear Down
    docker-compose down --volumes

    #stop all containers
    docker stop $(docker ps -q)

    #remove all containers
    docker rm $(docker ps -a -q)

    #remove all docker images
    docker rmi $(docker images -q)

This Preset was proudly presented by www.nexusdesigns.net, your place for designs or websites.