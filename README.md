# django-recipe-app-api

## Necessary Commands
```sh
docker build .
docker-compose build
docker-compose run --rm app sh -c "flake8"
docker-compose run --rm app sh -c "django-admin startproject app ."
docker-compose up
docker-compose down
docker-compose run --rm app sh -c "python manage.py startapp core"
docker-compose run --rm app sh -c "python manage.py test"
docker-compose run --rm app sh -c "python manage.py test && flake8"
docker-compose run --rm app sh -c "python manage.py wait_for_db"
docker-compose run --rm app sh -c "python manage.py wait_for_db && flake8"
docker-compose run --rm app sh -c "python manage.py makemigrations"
docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"
docker volume ls
docker volume rm django-recipe-app-api_dev-db-data
docker-compose down
docker volume rm django-recipe-app-api_dev-db-data
docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"
docker-compose run --rm app sh -c "python manage.py test"
docker-compose run --rm app sh -c "python manage.py createsuperuser" #127.0.0.1:8000/admin admin@example.com password
```
-----------------------
Kawshik Kumar Paul\
kawshikbuet17@gmail.com