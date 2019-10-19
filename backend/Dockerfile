# Dockerfile obtained from: https://dev.to/englishcraig/creating-an-app-with-docker-compose-django-and-create-react-app-31lf and modified

# Use official Python runtime as parent image
FROM python:3.6

# Adding backend directory to make absolute filepaths consistent across services
WORKDIR /read.me/backend

# Install python dependencies
COPY requirements.txt /read.me/backend
RUN pip3 install --upgrade pip -r requirements.txt

# Adding the rest of the code
COPY . /read.me/backend

# Making port 8000 available for the application
EXPOSE 8000

# Using 0.0.0.0 for the host within the docker container so that the browser
# can find it
CMD python3 manage.py runserver 0.0.0.0:8000


