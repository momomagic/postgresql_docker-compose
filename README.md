## Install postgreSQL with docker and docker-compose

* Make sure you have docker and docker-compose in your local machine 

```
    docker ps 
    docker-compose ps 
```


## Run environment 

```
cd $directory_of_docker-compose 
docker-compose up -d 
docker-compose logs 
```


## connect to your postgreSQL 


```
docker-compose exec -it db /bin/bash
psql --username postgres --password
SELECT * FROM pg_catalog.pg_tables;
```