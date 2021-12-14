#Use Python 3.6 as a base image
FROM python:3.7
# Copy contents into image
WORKDIR /dcfrontend
# Copying files to new directory
COPY . .
# install pip dependencies from requirements file
RUN pip install -r "requirements.txt"
# Set environment variables
ENV MYSQL_USER "jackc"
ENV MYSQL_PWD "Admin00#"
ENV MYSQL_IP "jacksdbs.mysql.database.azure.com"
ENV MYSQL_DB "jacksdbs"
ENV MYSQL_SK "sofdnbshelvosgul"

# Expose correct port
EXPOSE 5000
# Create an entrypoint
ENTRYPOINT [ "python", "app.py" ]