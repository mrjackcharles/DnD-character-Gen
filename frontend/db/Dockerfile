# Derived from official mysql image (our base image)

# Use mysql 5.7 as the flask-app is not set up to work with later versions

FROM mysql:5.7

# Add a database and root password

ENV MYSQL_ROOT_PASSWORD = Admin00#

ENV MYSQL_DB=jacksdbs

# Add the content of the .sql file to your image

COPY CreateTable.sql docker-entrypoint-initdb.d/

# All scripts copied to docker-entrypoint-initdb.d/ are automatically executed during container startup.

# get SQL database