## Short overview
A repository that collects useful stacks for debugging and deploying changes to database instances and open source applications locally. Each docker-compose contains the other applications described here in the README.md

## Run specific docker-compose file 
```
docker-compose -f docker-compose1.yml
```
Description of the individual docker-compose
##### docker-compose-1.yaml mysql:latest with php_my_admin
##### docker-compose-2.yaml nginx proxy manager with gui panel hosted on port 81 with mariadb:latest
##### docker-compose-3.yaml xwiki for collection of documentation
##### docker-compose-4.yaml prometheus, grafana, cadvisor for monitoring
##### docker-compose-5.yaml not yet. 
# Stop services only
```
docker-compose stop docker-compose1.yml
```
# Stop and remove containers, networks..
docker-compose down docker-compose1.yml

# Down and remove volumes
```
docker-compose down --volumes docker-compose1.yml
```

# Down and remove images
```
docker-compose down --rmi <all|local> 
```


