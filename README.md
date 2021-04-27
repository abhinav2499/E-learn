## E-learn
### A content management system made using Django
![Alt Text](https://github.com/abhinav2499/E-learn/blob/master/courses/static/Animation3.gif)
## Overview
<p>
E-learn is a Django based web application where instructors can create different courses having multiple modules. Each module can have different types of content such
as image, text, video and file. Instructors can also edit and delete their courses. Students can sign up and enroll in different courses and can also chat with the
instructor as well as students of the respective enrolled courses.
</p>

## Installation
Make sure you have **Python** and **memcached** installed in your system.

Clone the repository

    https://github.com/abhinav2499/E-learn.git

Install all required dependencies in an isolated environment

    cd E-learn
    pipenv install django
    pipenv shell
    pipenv install -r requirements.txt
    
 ## Running on local server
 By default, the database for development server in **E-learn/db.sqlite3** is already filled with some data for ease of development.
 
 If you want to start clean then **delete db.sqlite3** and follow this step:
 
 ### Create migrations
 
    python manage.py makemigrations
    python manage.py migrate
    
### Create superuser

    python manage.py createsuperuser
    
### Run the server

    python manage.py runserver
