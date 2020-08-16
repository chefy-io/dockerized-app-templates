# Dockerized application template

## Tech stack

- Frontend:
  - React
    - Node: 8
  - Typescript: 3.7.5
- Backend:
  - Python: 3.7
  - Django: 3.1
- Storage:
  - MySQL: 8.0

## Install

- Spin up apps using Docker compose

> docker-compose up -d

- Start frontend

> docker exec -ti <frontend-app-container> bash
> npm start

You can access the starter React app on `localhost:3000`

- Start backend

> docker exec -ti <backend-app-container> bash

You should see a project directory like below:
```
backend/
  migrations/
  __init__.py
  asgi.py
  urls.py
  views.py
  wsgi.py
Dockerfile
manage.py
requirements.txt
```

Start Django app:

> python3 manage.py runserver 0.0.0.0:5000

