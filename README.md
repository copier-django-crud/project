# project
Template for Django project (django-admin startproject).

## Usage

Create `backend` directory and generate Django project `mysite` into it:

    copier gh:copier-django-crud/project backend
    🎤 What is your project name?
    mysite

    Copying from template version 0.0.0.post2.dev0+5a60e17
        create  .
        create  .copier-answers.yml
        create  mysite
        create  mysite/urls.py
        create  mysite/__init__.py
        create  mysite/asgi.py
        create  mysite/wsgi.py
        create  mysite/settings.py
        create  manage.py

Run the Django development server and visit the site `http://127.0.0.1:8000`:

    cd backend
    python3 -m venv venv && source venv/bin/activate && pip install -r requirements.txt
    python manage.py migrate
    python manage.py runserver

Create admin user and log into `http://127.0.0.1:8000/admin`:

    cd backend
    python manage.py createsuperuser
    python manage.py runserver

## Customization

    🎤 What default database do you want to use?
    mysql

Configure the database connection in `my.cnf` file.
