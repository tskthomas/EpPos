EpPos fully supports Docker for deployments.
We ship with docker-compose files ready to deploy and serve requests (no proxy necessary)
More details for geeks underneath the instructions.

## Setup
Make sure you have Docker and Docker-compose installed.
For quick and easy deployment on port 80, we have a management script, this needs Make.
You can simply run `make setup` and it will ask you for a superuser username, email and password and run EpPos as a daemon (service) in the background. Run `make down` to stop it.

If you don't want to run my script, are not on Linux or Mac OS, or want to run the production config (on port 80, no SSL), you can run `docker-compose -f docker-compose-prod.yml up -d --build` to build the images and run them.
`docker-compose -f docker-compose-prod.yml down` shuts them down. You can create a superuser by running `docker-compose -f docker-compose-prod.yml run web python manage.py createsuperuser`, this will prompt for username, email and password.

## Info for geeks
EpPos runs two containers, one "web" that runs `gunicorn` to serve our app, and one "nginx" that runs `nginx` to proxy in front of `gunicorn` and serve our static files. The prod config simply binds to port 80 rather than 8001.