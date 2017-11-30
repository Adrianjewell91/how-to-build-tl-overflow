How we Built Translate Overflow

How We Built Translate Overflow.

Understand that you always must activate a virtual environment when you work with a Django project.. Install the package(I forgot how), and always start before working with your project in python

Do the Getting Started with Django on the Django Documentation. User the newest version of python (probably 3.6.2), and create your app like this: 1. “cd your_file” 2. “virtualenv env”. #creates the virtual environment. 3. “source env/bin/activate” #activate virtual env. 4. Then do the Django create app instructions.

1.5. Do the “Getting Started with Django” Tutorial on Heroku.

Download and start your Django App with the Heroic Django Template.

Follow tutorials 1-5 in the Django REST Framework tutorial.

Build a React App on top of your app using this tutorial: https://www.techiediaries.com/create-react-app-django/

Pay attention to the settings.py configuration (change the “try:” line in your view to this line: with open(os.path.join('frontend', 'build', 'index.html')).

Build User auth using this tutorial: https://iheanyi.com/journal/user-registration-authentication-with-django-django-rest-framework-react-and-redux/. Then read our auth code to see how we changed it.

You may want to look at this one too:https://simpleisbetterthancomplex.com/tutorial/2017/02/18/how-to-create-user-sign-up-view.html Then read our code.

Build nested routes with this tutorial: https://github.com/alanjds/drf-nested-routers

When you decide to push to heroku, disable COLLECTSTATIC using “heroku config:set DISABLE_COLLECTSTATIC=1”, and un-ignore your build file in the create-react-app build settings by deleting the line in the .gitignore.

You need to make sure that your app, when uploaded on Heroku, uses your build files instead of the static files that python creates using collect static. This is really important.

Build out redux cycles.