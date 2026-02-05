# SytexHub User CRUD API

A simple User CRUD REST API built with Django, Django REST Framework, and PostgreSQL.
This project demonstrates how to build RESTful APIs for Create, Read, Update, and Delete operations.

==================================================

TECH STACK

- Python 3.10
- Django 3.2
- Django REST Framework
- PostgreSQL
- psycopg2-binary

==================================================

PROJECT STRUCTURE

sytexhub_user_crud_api/
├── manage.py
├── sytexhub_user_crud_api/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
├── users/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── serializers.py
│   ├── views.py
│   ├── urls.py
│   └── migrations/
└── README.md

==================================================

FEATURES

- Create user
- Read all users
- Read single user by ID
- Update user
- Delete user
- Django Admin panel for internal management

==================================================

INSTALLATION AND SETUP

1. Clone the repository

git clone https://github.com/your-username/sytexhub-user-crud-api.git
cd sytexhub-user-crud-api

2. Create virtual environment

python -m venv venv
venv\Scripts\activate

3. Install dependencies

pip install django djangorestframework psycopg2-binary

==================================================

DATABASE CONFIGURATION

Edit sytexhub_user_crud_api/settings.py

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'drf_project',
        'USER': 'postgres',
        'PASSWORD': 'your_postgres_password',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}

==================================================

RUN PROJECT

Apply migrations

python manage.py makemigrations
python manage.py migrate

Create superuser

python manage.py createsuperuser

Run server

python manage.py runserver

==================================================

ADMIN PANEL

URL:
http://127.0.0.1:8000/admin/

Use superuser credentials to log in.

==================================================

API ENDPOINTS

Base URL:
http://127.0.0.1:8000/api/users/

GET     /api/users/          -> Get all users
POST    /api/users/          -> Create user
GET     /api/users/{id}/     -> Get user by ID
PUT     /api/users/{id}/     -> Update user
DELETE  /api/users/{id}/     -> Delete user

==================================================

EXAMPLE REQUEST BODY

{
  "username": "john_doe",
  "email": "john@example.com",
  "age": 25
}

==================================================

TESTING

- Django REST Framework Browsable API
- Postman
- Insomnia

==================================================

LICENSE

This project is for educational and learning purposes only.

==================================================

AUTHOR

Ismail Sadykov
Backend Developer (Django)

==================================================
