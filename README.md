
  

# Drupal setup for a Docker container

Includes linked folders for database and file system

## Setup

**Add directories**
Create empty folders:

    mkdir ./drupal-files ./mariadb-data

Start up Docker containers

    docker compose up -d

As configured in supplied docker-compose.yml file, local environment will be available at http://localhost:8180/
  
## Drupal management in Docker

Access container command line

    docker compose exec drupal bash

You might find you have permissions issues in your drupal install. Fix it in bash by running

    chown -R www-data:www-data web

## Install Drupal core
From the bash prompt

    composer create-project drupal/recommended-project .

## References

StackEdit https://stackedit.io/app

Drupal Installation with Docker https://www.youtube.com/watch?v=kztDsxyesqM
