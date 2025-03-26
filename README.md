
# Drupal setup for a Docker container

Features linked folders for database and file system

## Setup

**Add directories**

Create empty folders:

    mkdir ./drupal-files ./mariadb-data
Start up Docker containers

    docker compose up -d
As configured in supplied docker-compose.yml file, local environment will be available at http://localhost:8180/



## References

StackEdit https://stackedit.io/app

Drupal Installation with Docker https://www.youtube.com/watch?v=kztDsxyesqM