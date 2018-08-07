# Docker Machine containing PHP/FPM,  Nginx and MariaDB

Generated with PHPDocker.io

Don't forget to stop every other machine running in the background before running this one
```
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
```

To start the machine simply use docker-compose
```
docker-compose up
```

All web files goes into the `public` directory.
Web server is accessible at http://localhost:8040

# Editing php.ini values

Edit the file located in `phpdocker/php-fpm/php-ini-overrides.ini`