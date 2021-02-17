# SAMPLE VERSION OF TODO APP
This app is written in Python with Flask and SQLAlchemy.

## A. Dependency
In order to run this app, the following dependencies must have been already installed:
1. Postgres. 
 * Start manually: `pg_ctl -D /usr/local/var/postgres start`
 * Stop manually: `pg_ctl -D /usr/local/var/postgres stop`
 
2. Flask

## B. Database 
* `createdb todoapp -p 5432` 
* Open the database prompt - `psql -p 5432`
* Connect to the database - `\c todoapp` 
* Displays the tables in the database `\dt` 
* Displays the schema of the 'todos' table `\d todos` 
* Displays the schema of the 'todolists' table `\d todolists` 

You can insert a few rows in both the tables. Insert first in the `todolists` relation. 


## C. Steps to Run the App:
* Open up the Terminal(for Mac users and Linux/UNIX users) and if you are a Windows user Download GitBash and open it.
* `pip3 install -r requirements.txt` to install dependencies. For Mac users, if you face difficulty in installing the `psycopg2`, you may consider intalling the `sudo brew install libpq` before running the `requirement.txt`.
* `flask db init && flask db migrate && flask db upgrade` initializing the migration files and upgrading the migration files. 
* `FLASK_APP=app.py flask run` to run the app (http://127.0.0.1:5000/ or http://localhost:5000).
