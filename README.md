Final project

## how to use

- clone the repository
- copy the .env.example file to .env
- update the env file
    - add key APACHE_DOCUMENT_ROOT=/var/www/html/public
    - update the db data:
            DB_CONNECTION=mysql
            DB_HOST=mysql
            DB_PORT=3306
            DB_DATABASE=Picard
            DB_USERNAME=root
            DB_PASSWORD=root
- generate the key with >$ compose artisan key:generate
- create a folder to bind to the db in the project root, with name dbdata
- build and run the container with >$ docker-compose up -d 
