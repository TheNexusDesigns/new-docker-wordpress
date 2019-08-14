# Run this to make docker wordpress working

if other path change command below


    sudo chown -R ubuntu:ubuntu ~/containers/wordpress-env
    sudo chown -R www-data:www-data ~/containers/wordpress-env



Some useful Docker Commands
----------------------
    #Run Docker background
    docker-compose up -d

    #To Tear Down
    docker-compose down --volumes

    #stop all containers
    docker stop $(docker ps -q)

    #remove all containers
    docker rm $(docker ps -a -q)

    #remove all docker images
    docker rmi $(docker images -q)