# Django Chunkator demo app

this demo app is mainly used for running tests, but you may want to install it for manual testing

## Install

* (create and) activate a virtualenv (using your favorite Python version)
* from this virtualenv, install your required Django version. e.g.: ``pip install Django==2.2``
* from this directory, install the demo app: ``pip install -e ./``


### Set up the database

This will create the SQLite database and sync its models:

```sh
django-admin migrate --settings=demo_chunkator.settings
```

### Feed the "bookstore"

We're providing a sample ``book.json`` fixture, to load into your DB like this:

```sh
django-admin loaddata --settings=demo_chunkator.settings book.json
```
