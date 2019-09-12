# Docker
basic development config

# .env configuration for laravel

DB_CONNECTION=mysql
DB_HOST=db
DB_PORT=3306
DB_DATABASE=app
DB_USERNAME=dev
DB_PASSWORD=password


# Run containers 
docker-compose up

# Show all working containers
docker ps

# Stop all working containers 
docker stop $(docker ps -aq)

# Delete all working containers 
docker rm $(docker ps -aq)

# Get inside container
docker-compose exec (NAME_OF_CONTAINER) bash

#NGINX Virtual hosts
root /var/www/site/public - this route use if index.php inside PUBLIC dir.
root /var/www/site/ - if index.php inside root dir of the project
