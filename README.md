# Django-Docker
Core files for starting a Django project in Docker

**Development**
* Start the Django server `docker-compose up -d --build`
* Create an admin user `docker-compose exec web python manage.py createsuperuser`
* Access the development app at `localhost:8000`

**Production**
* Start the WSGI server with Nginx proxy `docker-compose up -f docker-compose.prod.yml up -d --build`
* Access the production app at `0.0.0.0:80`
