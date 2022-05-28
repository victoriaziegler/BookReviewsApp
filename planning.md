# Planning

* [ ] Make and activate virtual environment
        - in terminal type:
            - 'python -m venv ./.venv'
            - 'source ./.venv/bin/activate'
* [ ] Install Django
        - 'pip install django'
* [ ] Create a Django project
        - 'django-admin startproject project_name .'
* [ ] Add a Django app to the project
        - 'python manage.py startapp app_name'
* [ ] Make migrations
        - 'python manage.py makemigrations'
* [ ] Migrate
        - 'python manage.py migrate'
* [ ] Add config to settings.py
        - 'INSTALLED_APPS = [
                'reviews.apps.ReviewsConfig'
                'django.contrib.admin',
                'django.contrib.auth',
                'django.contrib.contenttypes',
                'django.contrib.sessions',
                'django.contrib.messages',
                'django.contrib.staticfiles',
            ]'
* [ ] Make reviews/urls.py
        -and new file called 'urls.py' under reviews directory
        - add 
            - 'from django.urls import path
            urlpatters = [

            ]'
* [ ] Migrate
        - 'python manage.py migrate'
* [ ] Start Django server
        - 'python manage.py runserver'

# App

* [ ] Urls (urls.py)
        * [ ] Define a path so that based ont he path in the url bar, a request will be routed to a specific view
        * [ ] add a path to 'book_review/urls.py'
                * [ ] 'from reviews import views'
                * [ ] 'path('', views.home, name='home)'
                * [ ] What should the view be called? 'list_reviews'
* [ ] View
        * [ ] make a function called 'list_reviews'
                * [ ] takes a request
                * [ ] uses a render function, return result
                        * [ ] with reiews/main.html
* [ ] Model to query the database
        * [ ] Make a class
                - './reviews/models.py'
                - Class Review:
                        - include rating, image, title, summary, etc.
        * [ ] Has a list of books?
* [ ] Template to hold the new info
        * [ ] filepath:
                - 'mkdir reviews/templates'
                - 'mkdir reviews/templates/reviews'
                - 'touch reviews/templates/reviews/list.html'


        