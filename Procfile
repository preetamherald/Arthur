release: python manage.py migrate
web: daphne justchat.asgi:channel_layer --port $PORT --bind 0.0.0.0 -v2
worker: python manage.py runworker -v2