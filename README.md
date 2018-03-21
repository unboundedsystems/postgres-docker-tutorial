# PostgreSQL in Docker Tutorial
Sample setup to run [Postgres](https://www.postgresql.org/) in a [Docker](https://docker.com/) container on your local system
quickly and easily.
This repo is a companion to the
[How to run Postgres in Docker video](https://youtu.be/sNXVP2suMA8) on the
[Unbounded Systems YouTube Channel](https://www.youtube.com/channel/UC4GplIMxZZOkeB_Zlbe7Z1g).

## Starting Postgres
This compose file will download the [official Postgres Docker container](https://hub.docker.com/_/postgres/) and run
it on your local system, listening on the default port of 5432.

```shell
docker-compose -f postgres.yaml up
```
Type Control-C to stop the running container.

## Initial database contents
Any files in the `initdb` directory will be used to initialize the database
when the Postgres container is first started. The sample `init.sql` file
shows how to create a database called `sampledb`.

## Starting pgAdmin
This compose file can be used to run [pgAdmin](https://www.pgadmin.org/) to monitor and manage a
Postgres database. It will listen on your local system's port 8080.

```shell
docker-compose -f pgadmin.yaml up
```
Type Control-C to stop the running container.
