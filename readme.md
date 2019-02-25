# Docker Symfony
> Docker Compose for Symfony

## Installation
1 - Create the symfony project:
```bash
composer create-project symfony/website-skeleton app
``` 

2 - Change your .env mysql credentials on `app/.env`
```dotenv
DATABASE_URL=mysql://user:password@127.0.0.1:3306/app
```

2 - Start the docker compose:
```bash
docker-compose up -d
```
**Note:** First time will take a few minutes to download all the containers.

## Run the application
The application is listening the por :8888.
You can see the application running in **[http://localhost:8888](http://localhost:8888)**

## Commands
Check all the containers:
```bash
docker-compose ps
```

Entering the container:
```bash
docker exec -it docker-symfony_php_1 /bin/sh
```
