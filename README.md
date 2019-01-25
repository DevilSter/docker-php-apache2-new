# Common
Apache 2
PHP

# PHP Additional Modules
memcached<br />
pgsql<br />
redis<br />
xdebug

# XDebug
At the current time - XDebug is in beta for 7.3 and can be unstable

# docker-compose example
 ```dockerfile
version: '3'
services:
  web:
    build: .
    ports:
      - "80:80"
      - "443:443"
    volumes:
      - "./test:/var/www"
    environment:
      XDEBUG_CONFIG: ${XDEBUG_CONFIG}
```

# .env Example 

For Linux
```dotenv
COMPOSE_PROJECT_NAME=devilster_php_apache2
XDEBUG_CONFIG=remote_host=172.17.0.1
```

For MacOs
```dotenv
COMPOSE_PROJECT_NAME=devilster_php_apache2
XDEBUG_CONFIG=remote_host=docker.for.mac.localhost
```

For Windows
```dotenv
COMPOSE_PROJECT_NAME=devilster_php_apache2
XDEBUG_CONFIG=remote_host=docker.for.win.localhost
```
