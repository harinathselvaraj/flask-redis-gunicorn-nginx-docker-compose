# Boilerplate code for Flask application which uses the below technologies.
The code uses all the below technologies
- Flask
- Redis
- Unit testing
- Gunicorn
- Nginx - Load Balancing & Reverse Proxy
- Docker Compose to create seperate docker containers for Flask app, Redis & Nginx.

## Flask Folder
<code>app.ini</code> contains the parameters for WSGI Gunicorn settings
<code>Dockerfile</code> contains settings for building the flask container
<code>test.py</code> test cases for flask app

## Nginx Folder
<code>app.ini</code> contains the parameters for WSGI Gunicorn settings
<code>Dockerfile</code> Removes the default configuration for Nginx and uses nginx.conf

## Other Code
<code>dev.env</code> environmental file to store the variables
<code>docker-compose.yml</code> builds docker container for flask, Nginx & Redis

## How to run?
<code>
docker-compose --version
sudo docker-compose up
sudo docker-compose up --build       //use this command to build again and then run.
</code>

## How to deploy in AWS ECS and ECR?
https://www.youtube.com/watch?v=54U5L44K2es&feature=youtu.be
