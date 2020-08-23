FROM ruby:2.7

RUN apt update && apt -y install lsb-release awscli
RUN wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | apt-key add -
RUN echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" | tee  /etc/apt/sources.list.d/pgdg.list
RUN apt update && apt -y install postgresql-client-12

WORKDIR /app
ADD . /app/
