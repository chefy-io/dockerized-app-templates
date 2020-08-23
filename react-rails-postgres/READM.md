# Dockerized application template

## Tech stack

- Frontend:
  - React
    - Node: latest
  - Typescript: latest
- Backend:
  - Ruby: 2.7
  - Rails: 6.0
- Storage:
  - Postgres: 12.0

## Install

- Spin up apps using Docker compose

> docker-compose up -d

- Start frontend

> docker exec -ti <frontend-app-container> bash
> yarn start

- Start backend

> docker exec -ti <backend-app-container> bash

Start Rails app:

> rake db:create db:migrate
> rails s -b 0.0.0.0
