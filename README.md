# udacity-linux-server-config

What this is about?
-------------------

This is a configurations summary as part of the Udacity Linux Configurations course. The objective was to setup a python flask application to be served using an Apache webserver. Additinally all the data is being served using PostgreSQL.

* IP address: 35.160.19.90
* URL: http://35.160.19.90/restaurants/


## Summary of Packages installed


### via apt-get install
apache 2.4.7
psql (PostgreSQL) 9.3.16
postgresql-server-dev-9.3
postgresql-contrib
tree
git
python-pip
python-dev
build-essential


### via pip install
Flask (0.12)
psycopg2 (2.6.2)
SQLAlchemy==1.1.4
Werkzeug==0.11.15
oauth2client==4.0.0


## Summary of configurations made
1. User grader created wth sudo privileges enabled.
2. ssh key pair for grader created
3. Local time configured to UTC
4. SSH port change to 2200 from 22
5. ufw modified to only allow connections for SSH (port 2200), HTTP (port 80), and NTP (port 123)
6. Key-based SSH authentication is enforced.


### Third Party Resources
https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
http://blog.trackets.com/2013/08/19/postgresql-basics-by-example.html
http://docs.sqlalchemy.org/en/latest/dialects/postgresql.html

