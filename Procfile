release: python manage.py migrate
web: gunicorn config.wsgi:applicationworker: celery worker --app=config.celery_app --loglevel=info
beat: celery beat --app=config.celery_app --loglevel=info
