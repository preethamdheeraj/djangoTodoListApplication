# djangoToDolistApplication
ToDo list project using Django REST framework
add the instructions to run the project later

asgiref==3.5.2 Django==3.2.9 pytz==2022.1 sqlparse==0.4.2 uWSGI>=2.0.18,<2.1

this text document will contain all the list of the versions that is used in the development of this project

http://localhost:8000/ this will contain the django public user interface with a level of abstraction that will not allow the django admin API to be changed in its classes for more security each user created will only be able to see his lists added and created. User 1 will not be able to access User 2 lists.

http://127.0.0.1:8000/admin/ this will contain the admin page that only the developer will have access to add delete and perform CRUD operations

venv\Scripts\activate.bat to activate the virtual environment

python manage.py runserver run this command in the terminal of windows or any choice to run the development and public server of the todo list django application
