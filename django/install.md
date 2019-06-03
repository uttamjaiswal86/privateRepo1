# How to install Django Framework

###### Firstly install python with latest version. Let's Assume > 3.0. Once you done with installlation then check it from python.
**To install django we can use PIP package manager to install it. pip install Django**
###### If You are planing to work with database then please follow specifice package to install database API funtinality with django. 
###### In addition to a database backend, you’ll need to make sure your Python database bindings are installed.
* If you’re using PostgreSQL, you’ll need the psycopg2 package. Refer to the PostgreSQL notes for further details.
* If you’re using MySQL, you’ll need a DB API driver like mysqlclient. See notes for the MySQL backend
for details.
* If you’re using SQLite you might want to read the SQLite backend notes.
* If you’re using Oracle, you’ll need a copy of cx_Oracle, but please read the notes for the Oracle backend for
details regarding supported versions of both Oracle and cx_Oracle.
* If you’re using an unofficial 3rd party backend, please consult the documentation provided for any additional
requirements.
---

#### To create a project using django CLI
###### django-admin startproject mysite
* mysite/
  * manage.py
  * mysite/
    * __init__.py
    * settings.py
    * urls.py
    * wsgi.py
###### These files are:
* The outer mysite/ root directory is just a container for your project. Its name doesn’t matter to Django; you can rename it to anything you like.
* manage.py: A command-line utility that lets you interact with this Django project in various ways. You can read all the details about manage.py in django-admin and manage.py.
* The inner mysite/ directory is the actual Python package for your project. Its name is the Python package name you’ll need to use to import anything inside it (e.g. mysite.urls).
* mysite/__init__.py: An empty file that tells Python that this directory should be considered a Python package. If you’re a Python beginner, read more about packages in the official Python docs.
* mysite/settings.py: Settings/configuration for this Django project. Django settings will tell you all about how settings work.
* mysite/urls.py: The URL declarations for this Django project; a “table of contents” of your Djangopowered site. You can read more about URLs in URL dispatcher.
* mysite/wsgi.py: An entry-point for WSGI-compatible web servers to serve your project. See How to deploy with WSGI for more details.

###### To create a new app under mysite project. *$ python manage.py startapp polls*
