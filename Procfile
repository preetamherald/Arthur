release: python manage.py migrate
web: gunicorn justchat.wsgi --log-file -
web: daphne justchat.settings:channel_layer --port $PORT --bind 0.0.0.0 -v2
worker: python manage.py runworker -v2