# PipelineDB - Postgresql-11 / for ARM64 
PostgreSQL + PipelineDB docker image for **Arm64** architecture

## Important Note!
Forked from 

[https://github.com/binakot/PostgreSQL-TimescaleDB-PipelineDB](https://github.com/binakot/PostgreSQL-TimescaleDB-PipelineDB)

--- 

Based on [Alpine Linux](https://alpinelinux.org).

Docker image with:
* [PostgreSQL](https://www.postgresql.org/)
* [PipelineDB](https://www.pipelinedb.com/)

Current versions of components:
* PostgreSQL: **11.9** ([Source docker image](https://store.docker.com/images/postgres))
* PipelineDB: **1.0.0-13** ([Release archive](https://github.com/pipelinedb/pipelinedb/releases/tag/1.0.0-13))

How to build:

```bash
$ docker build -t fsonmezay/pipelinedb-postgresql-11 .
```

How to run:

```bash
$ docker run -d --name postgres -e POSTGRES_PASSWORD=postgres fsonmezay/pipelinedb-postgresql-11
```

You can also build and run the docker image using `docker-compose`

```bash
# Building Image
docker-compose build
# Running the postgres image
docker-compose up
```

## IMPORTANT

PipelineDB has joined Confluent. 
PipelineDB will not have new releases beyond 1.0.0, although critical bugs will still be fixed.
PipelineDB currently supports PostgreSQL versions 10.1, 10.2, 10.3, 10.4, 10.5, and 11.0 on 64-bit architectures.
PipelineDB is under maintenance and will not support PostgreSQL after version 11.
