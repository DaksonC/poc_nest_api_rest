version: "3.8"

services:
postgres:
container_name: poc-nest-api-rest-pg
image: postgres
ports: - 5432:5432
environment:
POSTGRES_USER: user
POSTGRES_PASSWORD: password
POSTGRES_DB: poc-nest-api-rest
PGDATA: /data/postgres
volumes: - ./data/pg:/data/postgres
