# tutor
Tutorial hosting web application with django 

# Requirement
- Python3.7
- Django2.2.7
- Docker 19.03.2

# Development 
## Project Setup 

1. Building a docker image 
```bash
$ docker-compose build
```

2. Install Django library
```bash
docker-compose run --rm app pipenv install
```

3. start docker container
```bash
$ docker-compose up 
```

4. Execute migration to create a database
```bash
$ docker-compose run --rm app pipenv run python manage.py migrate
```

5. Create a Super User
```bash
$ docker-compose run --rm app pipenv run python manage.py createsuperuser
```

