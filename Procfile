web: SENTRY_CONF=sentry.conf.py twistd -n web --port=$PORT --wsgi=sentry.wsgi.application
worker: sentry --config=sentry.conf.py celery worker --loglevel=INFO
beat: sentry --config=sentry.conf.py celery beat --loglevel=INFO
