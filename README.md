# python-test

### install command line

1. Make sure python version is 3.11.5
```bash
# switch to 3.11.5 
$ pyenv local 3.11.5

# or install
$ pyenv install 3.11.5
```

2. Install python virtual environment
```bash
$ python -m venv .venv
```

3. Active the python virtual environment
```bash
$ source .venv/bin/activate
```

4. Install python libraries.
```bash
$ python -m pip install -r requirements.txt
```

5. If you want to update library list
```bash
$ python -m pip freeze > requirements.txt
```

### start-up command line

1. create project
```bash
$ django-admin startproject [project_name]
```

2. start project
```bash
$ python manage.py runserver
```

3. create app
```bash
$ python manage.py startapp [app_name]
```

### adjust database command line

1. Edit models.py in specific app file.
e.g. polls/models.py

2. Add app config to settings.py.
e.g. line 34 in testsite/settings.py

3. Make migrations
```bash
$ python manage.py makemigrations [app_name]
```

4. Apply those changes to the database.
```bash
$ python manage.py migrate
```
