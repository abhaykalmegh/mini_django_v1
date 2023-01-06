### To create django project


```shell
# linux command
django-admin startproject velocity

# windows command
django-admin.exe startproject velocity
```

### project structure

```markdown

mini_django_v1 (project-directory)

    - README.md
    - requirements.txt
    - venv
    - velocity  (project)
        - manage.py
        - velocity  (project-settings)
            - __init__.py
            - asgi.py
            - wsgi.py
            - settings.py
            - urls.py

```



### django files 

- `manage.py` :: this script helps us with management of site. It helps us to 
to start web server.

- `settings.py` :: contains configuration for the website
- `urls.py` :: this is a file for URL management
- `wsgi.py` :: deployment purpose
- `asgi.py` :: deployment purpose



## default database with django 

- sqlite

## how to create tables associated with sub-applications?

- Django has pre-built sub-applications available in itself.
- We can create database tables using those apps by using following command 

```shell
cd <project-directory>   # cd velocity
python manage.py migrate
```
- To run the application

```shell
python manage.py runserver
```

## Synopsis to start with django

Step 1: create directory `mkdir <project-root>`
Step 2: `cd` to directory in step 1
Step 3: `django-admin.exe startproject velocity`
Step 4: `cd velocity`
Step 5: create DB tables  `python manage.py migrate`
Step 6: run project `python manage.py runserver`