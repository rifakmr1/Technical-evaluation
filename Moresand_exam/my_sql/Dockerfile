FROM ubuntu:22.04

ENV MYSQL_ROOT_PASSWORD=root
ENV MYSQL_DATABASE=mydb
ENV MYSQL_USER=myuser
ENV MYSQL_PASSWORD=mypassword

RUN apt-get update && apt-get install -y mysql-server

COPY sql-scripts/ /docker-entrypoint-initdb.d/

EXPOSE 3306

CMD ["mysqld"]
