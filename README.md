# django-ssl-nginx-gunicorn


This is a simple set up document for using ssl with nginx and gunicorn


### you need to add following things to your settings.py


SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')
SECURE_SSL_REDIRECT = True
SESSION_COOKIE_SECURE = True
CSRF_COOKIE_SECURE = True

we are done
