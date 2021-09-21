# ToDoApp
A todo app made as a school in class project (Date 2018) following along to the CS Dojo youtube video. This app uses Django and Python while operating in Sublime and Terminal


# Walk through of Code and Project


## Idea:

A website /app for managing tasks that are needed to be done


## Django:

Web framework based on pyython.

## Homebrew Install:

a. brew install python 3     (to download python)

b. Install pipenv : (pip3) - package manager    (python only)

  - a virutal environment for python

c. use pipenv to install django

  - pipenv install django
  - creates a virtual envionment for django

      - virtual environment specifies which version of django wanted

## Creating Django Environment:

a. got to virtual environment --> pipenv shell

b. start project --> django-admin start project "" .     (. represents current directory)

c. start django server --> python manage.py runserver

d. given url for django project


## Creating Hello World

a. create new app within project

  - app --> focuses on particular aspect of website
  - project --> single project powers website, can contain multiple apps

b. create new app hello

  - python manage.py startapp hello

c. let django know about the app   (hello)

  - open project in IDE
  - go to settings.py
      - add 'hello' in INSTALLED_APPS
  - create a view for the target URL    (view = shown to user for certain URL)
      - go to hello directory for views.py   (browser sends HTTP request to server, server responds with HTTP response)
      - open views.py
            
           add "from django.http import HttpResponse"
           
      - create view

            def myView(request):
          
             return HttpResponse('Hello')
              
          run server --> python manage.py runserver
          
      - connect django server with URL
     

"Still need to provide rest of walk through"
