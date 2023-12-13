# learn_django_v5

In this project I set up the development enviroment for django projects with the help of django-cookiecutter.
and build some very basic app for functional testing.

The setup of this development enviroment is as following:

- django docker container
- postgresql docker container
- docs docker container

It is convenient to have development enviroment as docker-based.
It runs pre-commit hooks and pytest. All was set up successfully.

The steps to create development enviroment are as following:

### create some folder for the project:
- mkdir projectdir
- cd projectdir
### install conda -> create and activate conda enviroment
- conda create --name env311_django42 python=3.11
- conda activate env311_django42
### install git
### install git-hooks
### install docker and docker-compose (see digitalocean tutorials)

### create project with django-cookiecutter, choose docker:yes, whitenoise:yes

- TO BE CONTINUED

[![Built with Cookiecutter Django](https://img.shields.io/badge/built%20with-Cookiecutter%20Django-ff69b4.svg?logo=cookiecutter)](https://github.com/cookiecutter/cookiecutter-django/)
[![Black code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)

License: MIT

## Settings

Moved to [settings](http://cookiecutter-django.readthedocs.io/en/latest/settings.html).

## Basic Commands

### Setting Up Your Users

- To create a **normal user account**, just go to Sign Up and fill out the form. Once you submit it, you'll see a "Verify Your E-mail Address" page. Go to your console to see a simulated email verification message. Copy the link into your browser. Now the user's email should be verified and ready to go.

- To create a **superuser account**, use this command:

      $ python manage.py createsuperuser

For convenience, you can keep your normal user logged in on Chrome and your superuser logged in on Firefox (or similar), so that you can see how the site behaves for both kinds of users.

### Type checks

Running type checks with mypy:

    $ mypy learn_django_v5

### Test coverage

To run the tests, check your test coverage, and generate an HTML coverage report:

    $ coverage run -m pytest
    $ coverage html
    $ open htmlcov/index.html

#### Running tests with pytest

    $ pytest

### Live reloading and Sass CSS compilation

Moved to [Live reloading and SASS compilation](https://cookiecutter-django.readthedocs.io/en/latest/developing-locally.html#sass-compilation-live-reloading).

## Deployment

The following details how to deploy this application.

### Docker

See detailed [cookiecutter-django Docker documentation](http://cookiecutter-django.readthedocs.io/en/latest/deployment-with-docker.html).
