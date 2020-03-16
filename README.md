# DjangoCommand

## CREATE PROJECT 

django-admin startproject project_name

## RUN SERVER

python manage.py runserver

## CREATE FEATURES

python manage.py startapp app_name

## RUN MIGRATE

python manage.py migrate

## CREATE MODELS

python manage.py makemigrations model_name

## START THE SHELL

python manage.py shell

## insert data in shell

from music.models import Album, Song
Album.objects.all()
Album.objects.filter(id=?)
Album.objects.filter(artist__startwith='Taylor)


a = Album(artist="Taylor ", ....)
a.save()

a.artist to access

## Admin interface

python manage.py createsuperuser
