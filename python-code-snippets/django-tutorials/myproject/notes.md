# Django workflow
```bat
mkdir django-projects
cd django-projects/
django-admin startproject myproject
cd myproject/
python3 manage.py runserver
```
make sure that your in project folder
```bash
django-admin startapp myapp
```

Include your app to your project in settings.py as follow
```python
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    #include your apps
    'myapp'
]
```

[how to create models and register them to admin](http://www.john-player.com/django/how-to-register-a-model-with-django-admin/)

when ever you make changes to your model use these following commands
```
python3 manage.py makemigrations
python3 manage.py migrate
```



