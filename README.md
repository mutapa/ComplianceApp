# The Compliance App
A Django web framework API for Compliance within the organization.

Install the project using commmand:
```django-admin startproject backendsite```

Install the apps for this project using the following commands:
```
    django-admin startapp consultants
    django-admin startapp locations
    django-admin startapp questions
    django-admin startapp solutions
    django-admin startapp surveys
```

Install a PostgresSQL and within the psql command prompt create a complianceappdb:
```CREATE DATABASE complianceappdb;```

To run the project website, issue the command below from inside the top-level backendsite folder:
```python manage.py runserver```

Change the database to use PostgresSQL by editing the settings.py file connection string
```
    DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'complianceappdb',
        'USER': 'postgres',
        'PASSWORD': 'django1234',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}

```