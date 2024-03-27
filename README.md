## Planetarium API

API service for planetarium management written on DRF

## Features

* JWT authenticated
* Admin panel /admin/
* Documentation is located at /api/doc/swagger/
* Managing Reservations and Tickets
* Creating Astronomy Shows with Themes
* Creating Planetarium Domes
* Adding Show Sessions
* Filtering Astronomy Shows and Show Sessions

## Used Technologies
* Python 3.12
* Django 5.0.3
* Postgres 16.0
* DRF 3.15.1

## Installation

- Python 3.12 must be already installed
- Install PostgresSQL 16 and create db

```shell
git clone https://github.com/Toltecos/planetarium-api.git
cd planetarium_api
python -m venv venv
venv\Scripts\activate (on Windows)
source venv/bin/activate (on macOS)
pip install -r requirements.txt
set DB_HOST=<your db hostname>
set DB_NAME=<your db name>
set DB_USER=<your db username>
set DB_PASSWORD=<your db user password>
set SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver # start Django Server
```

## Run with Docker

Docker must be already installed

```shell
docker-compose build
docker-compose up
```

## Getting access
* Create user via /api/user/register/
* Get access token via /api/user/token/
* Refresh access token via /api/user/token/refresh/
* User info via /api/user/me/

## DB Structure

![DB Structure](DB_structure.png)

## Demo

![Website Interface](demo.png)
