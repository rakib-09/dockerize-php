# Dockerize-php

## Process: 
***
* First clone this project into your desired folder.

```
https://github.com/rakib-09/dockerize-php.git
```

* Change your *.env* information as you want.

* Inside the `Workstation` directory put your all *php* code. 
*important: Your index.php file must inside the public directory*

* Build the *app* image with the following command:

```
docker-compose build app
```

* When the build is finished, you can run the environment in background mode with:

```
docker-compose up -d
```

* This will run your containers in the background. To show information about the state of your active services, run:

```
docker-compose ps
```

* Now run *composer install* to install the application dependencies:

```
docker-compose exec app composer install
```

* Now go to the browser and access your server’s domain name or IP address on port 8000:

```
http://server_domain_or_IP:8000
```

* For Mysql connection you have to write this in your settings file:

```
DB_HOST=mysqldb
DB_PORT=3306
DB_DATABASE=app_db
DB_USERNAME=admin
DB_PASSWORD=secret
```

