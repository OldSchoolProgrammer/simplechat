web: gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker
worker: celery -A skale.taskapp worker -P gevent -l info
beat: celery -A skale.taskapp beat -l info -S django