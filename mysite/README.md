# Crea venv
python -m venv venv
.\venv\Scripts\activate
## En bash:
source ./venv/bin/activate

# Init projecte
pip install django

## Crea projecte
django-admin startproject mysite
## Crea App (tot projecte té n apps)
python manage.py startapp polls

# Run
python manage.py runserver 127.0.0.1:8080

# NO - Install postgreSQL 16.3 (pgAdmin 4)
pip install psycopg2-binary
pip install psycopg2

# Migrations
python manage.py makemigrations ${APP} -- Crea les migracions (ex. polls/migrations/0001_initial.py)
python manage.py migrate -- migra definitivament atacant cap a BD

NOTA: cal registrar tota app dins del projecte manage.py

# Admin user
python manage.py createsuperuser

NOTA: cal registrar els models dins del manage.py de la app per a fer-los visibles

