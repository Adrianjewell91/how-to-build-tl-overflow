#How we Built Translate Overflow

##This tutorial is a guide to building Translate Overflow (https://github.com/Adrianjewell91/tl_overflow).

If you have any suggestions for clarity, please write me.

##Preface
Preface: Understand that you always must activate a virtual environment when you work with a Django project. Install python3 and install the package for virtualenv, and always activate it before working with your project in python. File structure should look something like:

/project
   /env 
   /project_name
      //all the actual files. 

##Start 
Do the Getting Started with Django on the Django Documentation. Use the newest version of python (probably 3.6.2), and create your app like this: 1. “cd your_project” 2. “virtualenv env”. #creates the virtual environment. 3. “source env/bin/activate”. 4. Then do the instructions for creating a Django app.

1 Do the “Getting Started with Django” Tutorial on Heroku. https://devcenter.heroku.com/articles/getting-started-with-python#introduction

Download and start your Django App with the Heroic Django Template.
(https://github.com/heroku/heroku-django-template

Follow tutorials 1-5 in the Django REST Framework tutorial.
http://www.django-rest-framework.org/

Build a React App on top of your app using this tutorial: https://www.techiediaries.com/create-react-app-django/.  Personall I now recommend using webpack, a tutorial that I wrote myself can be found here: (https://github.com/Adrianjewell91/madscience-django-react-webpack)

Pay attention to the settings.py configuration (change the “try:” line in your view to this line: with open(os.path.join('frontend', 'build', 'index.html')).

Build User auth using this tutorial (one of many ways it seems): https://iheanyi.com/journal/user-registration-authentication-with-django-django-rest-framework-react-and-redux/. Then read our auth code to see how we changed it.

You may want to look at this one too:https://simpleisbetterthancomplex.com/tutorial/2017/02/18/how-to-create-user-sign-up-view.html Then read our code.

Build nested routes with this tutorial: https://github.com/alanjds/drf-nested-routers

When you decide to push to heroku, disable COLLECTSTATIC using “heroku config:set DISABLE_COLLECTSTATIC=1”, and un-ignore your build file in the create-react-app build settings by deleting the line in the .gitignore. Or just do the webpack tutorial that I wrote after the fact.

Basically, you need to make sure that your app, when uploaded on Heroku, uses your build files instead of the static files that python creates using collect static. This is really important.

Build out redux cycles.