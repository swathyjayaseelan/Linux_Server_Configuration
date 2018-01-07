# Linux Server Configuration

## About
A content management system using Python's flask framework. Authentication is provided via OAuth and all data is stored within a PostgreSQL database. A Linux server(Amazon Light Sail) is configured to host it securely. 

## Server Details

IP Address : 35.165.225.152

SSH Port : 2200

URL: http://ec2-35-165-225-152.us-west-2.compute.amazonaws.com

## Configuration changes made

1. Updated all installed packages
2. Changed the SSH port from 22 to 2200
3. Configured FireWall to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123)
4. Created a new user "grader" with sudo permission
5. Timezone set to UTC
6. Permission to login as root is disabled
7. Keybased authentication is enforced i.e) password authentication is disabled

## Packages installed for this project

1. apache2
2. libapache2-mod-wsgi
3. postgresql
4. postgresql-contrib
5. python-psycopg2
6. python-flask
7. python-sqlalchemy
8. python-pip
9. oauth2client
10. requests
11. httplib2
12. git
13. virtualenv

## SSH key for user 'grader'

ssh key can be found at '/home/grader/.ssh/authorized_keys'

The Items Catalog app can be accessed at : 'http://35.165.225.152/' or 'http://ec2-35-165-225-152.us-west-2.compute.amazonaws.com/'

