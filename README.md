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

Run the Django development server:

    cd backend
    python3 -m venv venv && source venv/bin/activate && pip install django
    python manage.py migrate
    python manage.py runserver
