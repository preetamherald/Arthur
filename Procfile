release: python manage.py migrate
web: gunicorn justchat.wsgi --log-file -
worker: python manage.py runworker -v2