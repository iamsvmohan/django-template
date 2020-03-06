# django-template

## Feature


## Requirements

- Docker: 19.03.2
    - docker-compose: 3.7.3

## System

- Python: 3.6.7
- Nginx + uWSGI + Django + MySQL

## Usage

```
$ docker-compose up -d

# http://localhost/
```

docker-compose.yml

## Installation for Ubuntu 16.0.4 LTS

## Reference
```
$ cd django-template
$ pip install --upgrade pip
$ pip install --no-cache-dir -r requirements/development.txt
$ python manage.py migrate
$ python manage.py makemigrations app
```

```
$ uwsgi uwsgi.ini --http :3033 --stats 127.0.0.1:9191

# http://localhost:3033/
```

```
$ python manage.py test
```
