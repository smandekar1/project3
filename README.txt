Udacity Project 3 - Restaurant Menu App 

This application allows the user to add their favorite restaurants to a database of restaurants.  They can then add menu items with details about those menu items.  

Files/Folders 

README.txt - information on the running the Restaurant Menu App
project.py - python file containing functions that implement the restaurant database system.
database_setup.py - python file that creates the restaurant database 
static - folder containing images and stylesheet used for the application
templates - folder containing html temlplates used for the application
.vagrant - folder that syncs host machine  
pg_config - file retrieves information about the install version of Postgresql
restaurantwithusers - database for restaurant menu app information
vagrantfile - file that describes the type of machine required for a project
client_secrets - file containing login credentials
fb_client_secrets - file containing facebook login credentials 


Requirments

Python 2.7
flask 0.9
flask login 0.1.3
sqlalchemy
postgresql
psycopg2
pip
requests 
htplib2

Installing the Restaurant Menu App

1.  Clone the github repository using the command git clone https://github.com/smandekar1/project3
2.  navigate to the repository directory within shell 
3.  Run vagrant up and vagrant ssh commnads to run the vagrant virtual machine 

(sudo su command may be needed for the folllowing installations)

4.  apt-get -qqy update
5.  apt-get -qqy install postgresql python-psycopg2
6.  apt-get -qqy install python-flask python-sqlalchemy
7.  apt-get -qqy install python-pip
8.  pip install oauth2client
9.  pip install werkzeug==0.8.3
10. pip install flask==0.9
11. pip install Flask-Login==0.1.3
12. pip install requests
13. pip install httplib2
14. Run the database_setup.py command to setup the database at the vagrant virtual machine prompt
15. Run the project.py command to start the program
16. Navigate in your browser to http://localhost:5000

Operating the Restaurant Menu App

From the open browser, user is able to add,edit, and delete restaurants and their menus.
open API endpoints include:

/restaurant/<int:restaurant_id>/menu/JSON - retrieves menu information for a restaurant
/restaurant/<int:restaurant_id>/menu/<int:menu_id>/JSON - retrieves menu item information
/restaurant/JSON - retrieves list of restaurants
	





