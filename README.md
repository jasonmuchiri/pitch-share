# Pitch Share

#### An application for viewing and posting pitches

## Author

[Jason Muchiri](https://github.com/jasonmuchiri)

## Description

An application where users will submit their one minute pitches and other users will vote on them and leave comments to give their feedback on them.A user must first register an account, and on registration should receive a welcome email. Once registered and logged in,then he or she can post a pitch and comment on other pitches.

## Project's set up instructions

To start using this news-highlight app, use the following commands:

- `git clone` ~ This will automatically clone the repository to your local machine.

- `sudo apt-get install python3-pip`

- `cd news-highlight`

- `python3.6 -m venv --without-pip virtual` ~ create a virtual environment

- `source virtual/bin/activate` ~ activate the virtual environment

- `sudo curl https://bootstrap.pypa.io/get-pip.py | python` ~ to download pip

- `pip install flask` ~ to install Flask using pip

- `sudo apt-get update`

- `sudo apt-get install postgresql postgresql-contrib libpq-dev` ~ to install Postgres

- `sudo service postgresql start`

- `sudo -u postgres createuser --superuser $USER`

- `sudo -u postgres createdb $USER`

- `touch .psql_history`

- `psql` ~ to connect to the postgres server

- `\q` ~ to exit the server

- `pip install flask-SQLAlchemy` ~ to install Flask-SQLAlchemy

- `pip install psycopg2` ~ to install psycopg2 which is our Postgres driver

- `pip install flask-migrate` ~ to install the flask-migrate extension to create database migrations

- use the following commands to initialize our aplication to use Migrations
  
  - `python3.6 manage.py db init`

  - `python3.6 manage.py db migrate -m "Initial Migration"`

  - `python3.6 manage.py db upgrade`

- `pip install flask-login`

- `pip install flask-uploads`

- `pip install flask-mail`

- `pip install flask-simplemde markdown2`

- `chmod a+x start.sh` ~ to make the file executable

- `./start.sh` ~ to run the application

### Dependancies

- For reference open the requirements.txt file to view all the project's dependancies.

## BDD

|Behaviour|Input Example|Output Example|
|---------|-------------|--------------|
|See Pitches|Open a pitch|View the pitch|
|Create an account|Account details|Account created|
|Log in|Account details|Logged in|
|Comment on a pitch|Write a comment|Comment is posted|
|Submit a pitch|Write a pitch|Pitch is submitted|

## Live link to the application's website in heroku

https://pitch-share.herokuapp.com/

## Contacts

email me here: jasonmkinyua@gmail.com

## License Information

MIT License

Copyright (c) 2019 cooldragon