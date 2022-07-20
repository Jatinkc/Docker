# Simple Web Application

This is a simple web application using [Python Flask](https://flask.palletsprojects.com/en/2.1.x/) and [MySQL](https://www.mysql.com/downloads/) database. This is used in the demonstration of development of Ansible Playbooks.

Below are the steps required to get this working on a base linux system.

- Install all required dependencies
- Install and Configure Web Server
- Start Web Server

## Installation

Python and its dependencies

```bash
apt-get install -y python python-setuptools python-dev build-essential python-pip python-mysqldb
```

## Install and Configure Web Server

Install Python Flask dependency

```bash
pip install flask
pip install flask-mysql
```
- Copy app.py or download it from source repository
- Configure database credentials and parameters

## Start Web Server
Start web server

```bash
FLASK_APP=app.py flask run --host=0.0.0.0
```
## Run
Open a browser and go to URL
```bash
http://<IP>:5000                            => Welcome
http://<IP>:5000/hello                      => hey, User!
http://<IP>:5000/how are you                => I am good, how about you?
```
