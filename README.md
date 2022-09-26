# apache-php-7.1-mysql-5.7-mongo-4.4

## Requirements in this is as follows in the docker:
>apache2

>php-7.1

>mysql-5.7

>mongo-4.4

mongo 5 requires minimum of i3 processor for proper functioning

### To connect php container with mysql container we have to install mysql-client in the php container by writing the command in the Dockerfile of the php

>RUN apt-get update \
    && apt-get install -y default-mysql-client
    
 ### TO connect with mysql container run the command in the php container

> mysql -u root -p -h mysql
