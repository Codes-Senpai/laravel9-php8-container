# Laravel9 + PHP8

Docker Compose Up ready for developement.

## Installation

Make sure to have correct Docker environment setup as [here](https://docs.docker.com/engine/install/ubuntu/) then run the following cmd in directory 

```bash
$ docker compose up -d --build
# Attach Shell
$ docker compose exec php-apache /bin/bash
#init laravel
composer create-project laravel/laravel .
chown -R www-data:www-data /var/www/laravel_docker/
a2dissite 000-default.conf 
service apache2 reload


Visit http://localhost:8080/

```

## Usage

```python
# Attach Shell php-apache 
$ docker compose exec php-apache /bin/bash
# Attach Shell database 
$ docker compose exec database /bin/bash
# Shutdown
$ docker compose down

```



## Inspired from [here](https://www.twilio.com/blog/get-started-docker-laravel)


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)