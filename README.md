# PostgreSQL in Docker Tutorial
Sample setup to run Postgres in a Docker container on your local system
quickly and easily.

## Starting Postgres
This compose file will download the official Postgres Docker container and run
it on your local system, listening on the default port of 5432.

```shell
docker-compose -f postgres.yaml up
```
Type Control-C to stop the running container.

## Starting pgadmin4
This compose file can be used to run pgadmin4 to monitor and manage a
Postgres database. It will listen on your local system's port 8080.

```shell
docker-compose -f pgadmin.yaml up
```
Type Control-C to stop the running container.
