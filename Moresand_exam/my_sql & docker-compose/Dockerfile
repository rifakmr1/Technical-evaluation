FROM mysql:latest

# Set the environment variables for the root user
ENV MYSQL_ROOT_PASSWORD=my-secret-pw
ENV MYSQL_DATABASE=mydb

# Copy the SQL files to the container
COPY mydb.sql /docker-entrypoint-initdb.d/

EXPOSE 3306
CMD ["mysqld"]
