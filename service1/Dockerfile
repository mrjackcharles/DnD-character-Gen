#Use Python 3.6 as a base image
FROM python:3.7
# Copy contents into image
WORKDIR /dcservice1
# Copying files to new directory
COPY . .
# install pip dependencies from requirements file
RUN pip install -r "requirements.txt"
# Expose correct port
EXPOSE 5000
# Create an entrypoint
ENTRYPOINT [ "python", "app.py" ]