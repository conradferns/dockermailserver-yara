To delete all containers including its volumes use,

docker rm -vf $(docker ps -aq)
To delete all the images,

docker rmi -f $(docker images -aq)

Check Docker Logs

Docker logs {Container_Name}


docker-compose -f docker-compose.yml config. or docker-compose config


docker start -a -i `docker ps -q -l`
Explanation:

docker start start a container (requires name or ID)
-a attach to container
-i interactive mode
docker ps List containers
-q list only container IDs
-l list only last created container



^P^Q does work, BUT only when -t and -i is used to launch the container:
