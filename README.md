# django-react-jwt-auth-test
Trying out JWT authentication for a website with a React frontend and Django REST backend

Based on [this](https://medium.com/@dakota.lillie/django-react-jwt-authentication-5015ee00ef9a) tutorial.

## Installation

### Backend 

1. Open a terminal and navigate into the backend folder - make sure you stay in this directory
2. Create a virtual python environment for the project (note steps 2 and 3 may differ if you're not using linux):
    `python -m venv venv`
    (the first venv is the name of a command, the second venv is that name of the folder that will be created - this 
    could be named anything you like but I like to use 'venv')
3. Activate the virtual environment: `source venv/bin/activate`
4. Install requirements: `pip install -r requirements.txt`
5. Apply django migrations: `python manage.py migrate`. This will create a sqlite database which is essentially a file 
named db.sqlite3 that will mimic the functionality of a full blown SQL database. Note do NOT commit this file to git.
6. Create a superuser (admin) in the database by running: `python manage.py createsuperuser`
7. Run the django development server to test it's working: `python manage.py runserver`
