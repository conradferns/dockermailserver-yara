# My Docker Cheat Sheet

- **To delete all containers including its volumes use,**
``` bash
docker rm -vf $(docker ps -aq)
```
- **To delete all the images,**
``` bash
docker rmi -f $(docker images -aq)
```

- **Check Docker Logs**
``` bash
Docker logs {Container_Name}
```
- **To check your docker config**
``` bash
docker-compose -f docker-compose.yml config. or docker-compose config
```

- **Attach to container shell**
``` bash
docker exec -it {Container_Name} bash OR docker exec -it {Container_Name} sh 
```
- **Run a command on a container**
``` bash
docker exec -it {Container_Name} {Command} i.e. docker exec -it runny_runt ls
```
- **Detach from a Docker container's process or terminal and returns you to the host machine's command prompt (Only works when -t and -i is used to launch the container)** 
``` bash
Ctrl+P+Q 
```

  156  docker-compose up --remove-orphans
docker-compose up and -d and down

  255  docker container ls / volume network image
