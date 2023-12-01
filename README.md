
# Bug Tracker

## Overview

Bug Tracker is a platform for reporting bugs by documenting them with tickets, as well as their progress with comments posted by users of the same team.  
The application runs in a docker container through docker compose.

## Features

This Docker container consists of three services:  
- Next.js web application.  
- Java Spring REST api.  
- PostgreSQL database.  

## Prerequisites

- [Docker Desktop.](https://www.docker.com/products/docker-desktop/)

## Installation

1. Clone the repository and go to its directory:
```bash
git clone --recursive https://github.com/renan-aquino/bug-tracker-docker
```

**Note**: The `--recursive` tag is responsible for populating the submodule folders in your local copy.   Without it, these directories will be empty. If that happens, run the following commands to update the   submodules:
```bash
git submodule init
git submodule update
```
2. Run the Docker container:
```shell
docker-compose up -d
```

3. Access the web application on `localhost:3000`. The api will be running on port `:8080`, and the database on port `:5432` .

## Alternative Installation (without Docker)

You can also install the services locally without the need of a Docker container. Check the following repositories for more information:

- [Bug Tracker Web App.](https://github.com/renan-aquino/bug-tracker)
- [Bug Tracker API.](https://github.com/renan-aquino/bug-tracker-api)
