# DjangoCommand

## CREATE PROJECT 

django-admin startproject project_name

## RUN SERVER

python manage.py runserver

## CREATE FEATURES

python manage.py startapp app_name

## SETUP POSTGRESQL URL
import dj_database_url

DATABASES = {'default': dj_database_url.config(default='url')}

## RUN MIGRATE

python manage.py migrate

## CREATE MODELS

python manage.py makemigrations model_name

## START THE SHELL

python manage.py shell

## insert data in shell

from music.models import Album, Song
album1 = Album.objects.get(pk=1)
Album.objects.all()
Album.objects.filter(id=?)
Album.objects.filter(artist__startwith='Taylor)


a = Album(artist="Taylor ", ....)
a.save()

a.artist to access

## Adding Song to our db

album1 = Album.objects.get(pk=1)

song=Song()
song.album = album1

song.file_type = 'mp3'

song.save()

album1.song_set.all()

album1.song_set.create(song_title:'Hi', ....)

## Admin interface

python manage.py createsuperuser

## REST API

