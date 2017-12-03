# docker-symfony-development
[![Build Status](https://travis-ci.org/umbonia/docker-symfony-development.svg?branch=master)](https://travis-ci.org/umbonia/docker-symfony-development)
Setup a Docker environment and a 1..n Symfony project(s).
```
curl -L https://git.io/vbLSV | bash
```
## Requirements
- [Docker](https://docs.docker.com/engine/installation/)
- [Docker compose](https://docs.docker.com/compose/install/)

## Commands
```
make
```
```
up         docker-compose up
down       docker-compose down
restart    down & up
```
with a project name argument (eg. make install project=myproject)
> **Note:**
> Assuming that the <project> argument is the root name of the project.
> eg. /home/john/Desktop/myproject
```
install    make up and composer install.
require    Composer require.
new        make up, create a new Symfony project, install and edit hosts.
db-create  Create database
db-update  Update database (force)
clean      Remove the hosts entry.
```
