# Learned Concepts

A track record of topics and interesting facts that I've learned each week.

## Week 1

1.# CLI (day 2)


 create virus

 #!/bin/bash
 cd ~/Desktop
 vim virus


#Text

vim

create a file : vim newfile.txt

I  insert
wq (newfile.txt if not named yet)

--------

access a server : ssh daniel@72.23.24.34.178       (IP)




Sublime , atom, VS Code: more single file oriented


Jupyter : good for single files  and data science

repl.it : cool for sharing code


# Python exercises

cmd /  for multiple line commentary
cmd b  define the method

\t  add a tab
\n  break line


methods attached to specific objects


ctrl shift R to run in pycharm for first time

\"  special character " not defining a string

type()   defines the class

x = 10   x is an instance of the integer class

comments : # one line , ``` ```, docstring right 
after a function : def fun(a,b):
"""adds 

:param a: 
:param b: 
:return: 
"""

# Friday


iterables : lists strings generators tuples

exercises page 46

in a function :  pass used to complte later

print has an argument to print on same line

list comprehension

read up to page 69 (4-12)


comprehension example : squares = [value**2 for value in range(1,11)]

print on one line
print("hello", "my", "man")
--> hello my man
for i in range(3):
    print(i+1, end=" ")
--> 1 2 3 

# Saturday 1
local variable 'name' referenced before assignment --> when u define in local scope a global scope variable


# Monday2
add a remote repository : git remote add namebranch httpgiithub...
remove : git remote remove testbranch

things we dont wanna commit: add a .gitignore   generelly .idea and venv we dont wanna commit

git workflow:
git init , make changes, git add<filename> , git commit -m "msg" , git push <remote-name> master

Tuples
x = 1, 2   -> give a tuple

def my_funct():
 a =1
 b = 2
 return a, b
 --> returns a tuple

unpack the tuple ->  y,z = my_funct()
                     print(y)   -> 1
                     print (z) -> 2
                     
 aliasing -> new_list = my_list point the same space in memory, if i change one i change the other
 if i wanna make a copy : new_list = my_list.copy
 
 ctrl T rename or right click refactor rename
 
 cache -> how that works? memory management for mutable and immutable object
 
 membership to a list -> in    not in
 
 do exercises all from chapter 5
 
 git log -> check history
 git checkout 512d9dcf3a811654 -> rolls back to that commit    and reset head
 git checkout master returns to latest version
 
 create a branch:
 git checkout -b caden_db_feature
 git branch -a
 git branch -> tells which branch u at
 
 git push salt_remote caden_db_feature  -> where we wanna push, what we wanna push
 
 #Tuesday2
 
 try
 ..
 except ValueError:
 
 dcitonnaries:
 each key must be unique, each key has to be an immutable
 
 start a dictionnary:
 dict_1= dict()
 dict_2 = {}
 not ordered
 object dict keys iterable but no indexable
 .item() method returns tuples
 
 tuple unpacking:
 t = (1,2)
 a, b = t
 
 json files and XML : data structures to communicate info on web
 
while loops usefeul for inputs

function.__call__()  equivalent to function()

a function returns None by default

isintance(variable, type(ex string)  _> equivalent to type(variable) == type (ex string)

# Thursday week 2

if merge conflict, change the file in question  , add and commit again

a = "hello" -> we instantiate a string object

anki flash cards -> good for memory

module -> python file with functions , classes...
import math -> from standard library

when creating instance of a class you call __init__

# Friday week 2

Class attribute : attribut put a the top of the script before the functions (init...)
Instance attribute: in ___init___

aliasing -> for mutable object
shallow copy -> import copy    b = copy.copy(a)  
deep copy  -> use on mutable objects

#Weekend2

https://www.digitalocean.com/community/tutorials/understanding-class-and-instance-variables-in-python-3?fbclid=IwAR2rSFQCT3MpkoQCxGiA4CUAsXTklyi2_GWBHJQTI1lgPWnj7xzKA9MiVJg

if __name__ == "__main__":  -> 

# Monday week 3

with open -> closes the file at the end of the block (just open leaves it open)
fin when read
fout when write

check import logging  -> you can track what happens in the code

successful situation : try -> else -> finally
unsuccesful situation : try -> else ->finally

install a package:
which python -> should tell you venv/bin/python
if not in venv -> project interpreter and choose venv
downloads from pypi.org
project gutemberg _> lots of text

read() returns one long string
readlines() returns a list of lines

# Tuesday3
w+ read and write
raise Exception("custom exc bla bla"")
encode = "utf8"  solves problems sometimes in open
make root folder when prob with num in name

tdd test driven development
1.pseudocode 2.write test 3.write code

.  test pass

unittest

in python console : python -m unittest

import unittest
import text
create class TestNameoffile(unittest.TestCase)
def test superlongname
   self.assertSomething(text.bla)
unittest testing framework

name your test file  test_fun.py

breakpoint()  -> debugg on server    on CLI pdb   commands n,p,q

object = instance

make directory as source root can solve import problems (ex:number in the name)

function dir() -> give info 

# wednesday 3

virtual environment -> we create one for each project, has a py version, pip -> pip install 

in command line
python3 -m venv .env -> creates a python3 in the virtual environment  .env -> whichever name(the . makes it hidden)
source .env/bin/activate _> we get inside the virtual environment  (to exit _> "deactivate" in CLI
then we install the package in the venv:
pip install InstagramAPI
which python
/Users/danielwegmann/Documents/CodingNomads/instagram/.env/bin/python  (shows python we using inside the project)
pip freeze -l  (local) shows all packages installed

so steps:
 make venv , activate , pip install, make .py file, write code
 (alt space does quick preview of pics in pycharm)
 Thleruth/bot_arbitrage
 
# Friday3

Class attribute:
class Chair:
    legs = 4
instance attribute:
def__init__(self, color):
    self.color() = color
 
method is called on an object " object.methos()  eq to  method(self)

d = Dog()   _> calls Dog.__innit()__     instantiation

create custom exception:

def MyException(Exception):
   pass
   
   a = 1
   b = 1
   
   if a!=b:
    raise MyException("not equal")    _> shows traceback and terminate code   (whereas catching continues the process)
    
  create virtual environment (from CLI):
  python3 -m venv .env
  source .env/bin/activate
  
  "deactivate" to get out of the venv
  
  
 generator:
gen = (x+1 for x in my_list)
-> gen is an iterable, takes much less memory space than a comprehension
returns an object

list comprehension, generator , lambdas 

# Monday 4

html
body, P, a , div

eval(input) -> executes the input

# Tuesday4

<a href = "url"> link </a>    --> attirbute in opening tag
create unordered listof 4 elements : ul > li * 4

style -> can write css inside html
<head>
  <meta charse...
  <link rel="stylesheet" href ="style.css">
 </head>
 
 brackets plugin > for  css syntx higlighting
 
 classes:
in css : .top-headin {
             color :blue
           }
  <h1 class = "top-headin..."> blbla</h1>
  example : css zen garden
  viewport adapts to mobile
  
  gor github website display name your file index.html
  setting, master branch
 
# Wednesay 4
file:///  or file://localhost/  access your root folder
URI URL
ftp://  http://  are protocols  www.codingnomads.com domain name
ping www.blabla.com in CLI shows IP
traceroute in CLI shows trought which servers this goes
ports : 80 main one

# Thursday4:
pip install requests-html
history id
fragment -> samepagelink    example ww.blabla#History
xpath to find precise elements

with requests_html : r.html.render() -> opens chromium to render the a return the JS

on github to put the project online : call file index.html then click on settings and go down

use Xpath to get a specific element in requests-html (right click inspect right click copy xpath)

# Friday4:
html requests -> use Session() object to keep pesisting info after login in
get request gets an html response object

# Monday5:
master branch -> working code
branch dev then pull request
commit to different branche : git checkout -b your-new-branch   ,   git add  ,  git commit   (-b = branch)
regular website : html   api : jason or xml response
post : create content  put : change data

keep secret tokens or passwords: 
1. create secrets.py or config.py   -> put in .gitignore  (to do globally **/secrets but better to do for each project)
from secrets import API_Key
2.venvs : export TEST="test" -> we have access to that key  (in bin/activate)
 or dircetly in pycharm -> preferences build execution, python console, environment variables
 import os
 os.environ.get('TEST'))
 -> we get the test variable
 
 slack: api 

crontab -e   crontab -l

# Tuesday 5

relationnal database : relate from table to table, never duplicate data. primary key identify each record
link tables with foreign keys -> point to primary key in other table
use lookup  table (ex:studen courses)
many to many -> lookup table
many to one -> add a column in the many
one to one -> all in same table
interact with sql -> client or statement

query statement : SELECT * FROM students;
returns a result set : table with elements required
when insert : return success or failure

can add sorting:
SELECT * FROM students WHERE age > 20;

INSERT INTO Students (name, age) VALUES ("daniel", 32)
(we'll make the id autoincrement)

JOIN gives temporary joining of 2 tables
example : 
SELECT * FROM Student as s
JOIN Student-Course sc   (thats the lookup table)
ON s.id = sc.student_id
JOIN courses as c
ON sc.course_id = c.id;
(WHERE s.id = 1;)

postgress:

in the CLI
$psql (connects to postgress server)
psql -u postgress 
\? -> commands
\l -> list of databases
\c -> connect to database
\q -> quit
\dt -> shows all tables
can type SQL queries straight in there
CLI pg_restore -> import downloaded database into postgres
Import a database:
pg_restore -U danielwegmann -d dvdrentals /Users/danielwegmann/Downloads/dvdrental 
schemas, tables
tools query tool

pgAdmin4
create server right click create
schemas tables

on postgress start server (opens cli psql)
open pgadmin
create database with connection localhost

make something available anywhere on computer : add the path to .bash_profile 


# Wednesday 5

from root folder : vim .gitignore to add global gitignore

when we create database -> do it within pgadmin
then intereact on python
echo = true -> shows sql statements

pip install SQLAlchemy  
pip install psycopg2       

# Friday 5
ORM is a translator from python to relationnal database    object relation mapper
connection string -  dataURI (unified ressource identifier)
db.select[(actors.columns.name)]

sandman2 package
sandman2ctl connectionstring
example : sandman2ctl 'postgres+psycopg2://danielwegmann:Sunrise2016$@localhost:5432/dvdrentals'

microservices : little apps that can be on diff servers (exemple authentification, posts) that are Rest APIs

put : you have to put the end pint (ex:actor/201)
post: endpoint is actor/   and will create new id automatically

IFTTT connects
psql : create database nameofdatabase

# Monday 6

MVC (MTV in django)
django templating language
sandman2
front end framework -> executed on client side
back end -> happens on the server
SALT stores a hash

create a django project
create file with venv
pip install django
pip freeze > requirements
django-admin startproject name [directory]
make a .gitignore(venv idea secrets) and secrets.py
gitinit
python manage.py migrate
add sqlite database to gitignore
python manage.py runserver
python manage.py createsuperuser (to create an admin)
create a README.md file
git add .    
git commit -m "inital setup"
python manage.py startapp appname  (creates app file on top of management app we have)
in models.py -> put db models as class (singular in django)
class inherits from models.Model
"class Topic(models.Model):                      #id is made automatically
    text = models.CharField(max_length=200)
    date_added = models.DateTimeField(auto_now_add=True)

    def __str__(self):
        return self.text"
add our new app logs in setting.py in our management app (dont forget "," at the end can mess up django) ex: "testapp",
python manage.py makemigrations (creates initial.py in the migrations file of our app)
python manage.py sqlmigrate logs 0001   (show what SQL does with migrate)      
python manage.py migrate (executes the init)
go to admin.py to register the topics model:
"from .models import Topic
admin.site.register(Topic)"
python manage.py runserver

add the other class in models.py
class Entry(models.Model):
    topic = models.ForeignKey(Topic, on_delete=models.CASCADE) # show that it needs sth on delete
    text = models.TextField()
    date_added = models.DateTimeField(auto_now_add=True)

    class Meta:
        verbose_name_plural = 'entries'    #django pluralises so we put this to get entries instead of entrys

    def __str__(self):
        return f"{self.text[:50]}..."   #display a clipped version


python manage.py makemigrations  
python manage.py migrate  
put admin.site.register(Entry) in admin.py


good sqlalchemy tutorial : https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_core_using_conjunctions.html

# Tuesday 6
sqlite is a file postgress run server

scrum master talk


django continued:
for queries in the database we can start a django shell
>>>python manage.py shell    in the cli
>>>from logs.models import Topic, Entry
example:
>>> e = Entry.objects.get(id=1)
>>> e
<Entry: relationnal database : relate from table to table,...>

in our app :
gonna work in templates
view.py for code logic
urls.py for routes

urls.py in management app but we create a new url.py in our own app
in management url:
'''from django.contrib import admin
from django.urls import path, include

urlpatterns = [
    path('admin/', admin.site.urls),
    path('logs/', include('logs.urls')),
]'''

in our app url:
'''from django.urls import path
from logs import views

urlpatterns = [
    path('', views.index),
]'''

then go in our views.py and put:
'''from django.shortcuts import render
from django.htpp import HttpResponse

'Create your views here and put the function:
def index(request):
    return render(request,"base.html")
    ->return HttpResponse("<hhello django!1")'''
 create a templates file in the app
create a base.html 
 go into settings of management app and add DIRS': [os.path.join(BASE_DIR, 'logs/templates')], in TEMPLATES
 
 how it works again:
 1) learning-logs -> urls of management app
 2) redirects to url of the app
 3)redirects to views  
 4) executes function 
 5) sends to template via render


in our app, to be able to pass info of database from views to template we use a context variable in views: (in views.py)
'''def list(request):
    context = {}
    t = Topic.objects.all()
    context["topics"] = t
    return render(request, "list.html",context)'''

we can put logic in html files:
    <ol>
        {% for topic in topics %}
        <li>{{topic}}</li>
        {% endfor %}
    </ol>


we have been following Web Applications project3 from the book(up to p453 pdf)  finish chapter 18

we can define live templates (tab tab)

base.thml helps define a base with :
    {% block content %}

    {% endblock %}

and we call in index with :
{% extends "base.html" %}

    {% block content %}
        <h2>whatsupppp</h2>
    {% endblock content %}
    
can use loops in html templates:
{% for i in blabla %}
  do this
{% endfor %}

# Wednesday 6

forms: in html stuff that we fill up
create froms.py on app level

for namesspaces:
app_name = "logs" 
path('new_topic/', views.new_topic, name="new_topic")

# Java crash course
comiled language, use java virtual machine to run the code

# Friday6
Deployment in Heroku
export SECRET_KEY='blabla'

# Monday 7
operators
"google this"
- blabla
+ blabla

tools ; can change time frame

#decorators
@login_required    (python thing)
function that takes a funct as a an argument and return a function object

# AWS



https://www.digitalocean.com/community/tutorials/how-to-set-up-django-with-postgres-nginx-and-gunicorn-on-ubuntu-18-04#creating-systemd-socket-and-service-files-for-gunicorn

STEP 1. clone - run locally - push to github

1. create folder
2. create a virtual environement: $ python3 -m venv .env
3. activate .env: $ source .env/bin/activate
4. clone from github: $ git clone https://github.com/martin-martin/django-twitter-clone.git
5. $ cd django-twitter-clone
6. $ pip install -r requirements.txt
7. $ python djitter/manage.py migrate
8. $ cd djitter
9. $ python manage.py makemigrations djeet
10. $ python manage.py makemigrations djeeterprofile
11. migrate the DB: $ python manage.py migrate
12. check if it’s running in localhost: $ python manage.py runserver
13. create github repository, and push to github.
$ git add /commit/ add remote <your remote name> “github repository link ”
$ git push ming master

STEP 2.
1. register an account with AWS.
2. login to AWS management console
3. Services -> EC2 -> Instances -> Launch Instance -> Ubuntu -> next until Configure Security Group: set Source=My IP
Add one more type: Custom TCP , port range = 8000, anywhere
Add one more type: HTTP, port range = 80, anywhere
750hour a month for one instance for free for only one year
port: 8080 development 8000; 22 secured shell
4. click: Launch
5. create new key pair
6. download the key pem.txt

wait for 15 mins

7. click on View Instances on the right down corner
8. change the name and click on Connect
9. In Terminal:
$ deactivate
$ cd
$ ls -al
10. if there is no .ssh folder create  one, then move pem file inside
$ cd .ssh
$ mv ../Downloads/ming_bali.pem .
11. change security owner read only: $ chmod 400 ming_bali.pem
12. when you are in .ssh folder, connect to server, based on DNS(domain name server) or server info given by AWS
$ ssh -i “ming_bali.pem” ubuntu@ec2-34-213-211-97.us-west-2.compute.amazonaws.com
13. when asked, type: yes
14. now we are at ubuntu@ip-172-31-24-209:~$
15. security group -> inbound -> edit inbound rules -> click on My IP: it will change to a new IP
16. install python, nginx sql curl etc here:
$ sudo apt-get update
$ sudo apt-get install python3-pip
$ sudo apt-get install python3-dev
$ sudo apt-get install nginx
$ sudo apt-get install curl
$ sudo apt-get install libmysqlclient-dev
$ sudo apt-get install python3-venv
(sudo = superuser do, which you can only install in superuser level)

STEP 3.
create directory in server: ubuntu@ip-172-31-24-209:~$ mkdir twitter_proj
$ cd twitter_proj/
$ git clone https://github.com/mingyyy/django-twitter-clone
$ cd django-twitter-clone/
create virtual environment: $ python3 -m venv env
activate virtual environment: $ source env/bin/activate
clone from github: $ git clone https://github.com/martin-martin/django-twitter-clone.git
$ cd django-twitter-clone
recursive install: $ pip install -r requirements.txt
$ pip install gunicorn
Go to setting.py file, change:
1. DEBUG=False
2. add one more item in ALLOWED_HOSTS, copy from public IP into this list.
make migrations for app djeet: $ python manage.py makemigrations djeet
make migrations for app djeeterprofile: $ python manage.py makemigrations djeeterprofile
migrate the DB: $ python manage.py migrate
runserver here command: python manage.py runserver 0.0.0.0:8000
goto brower find the public ip and add 8000:
http://34.213.211.97:8000
Now it’s running....

Then, we close the session: ctrl+c, web is not working after this.
Next we test gunicorn to run our server when we are on the session: $ gunicorn --bind 0.0.0.0:8000 djitter.wsgi
Again, the web app is running...
mingyyy/django-twitter-clone
Language
Python
Last updated
2 hours ago
mingyyy/django-twitter-cloneToday at 9:57 AMAdded by GitHub
Note for today, so far… still long way to go according to Caden

# Monday 8

RDS database is a server just for a database
lsof -i tcp

1. connect local project to local postgress
2.create new RDS
3. connect local proj to remote RDS
4. EC2 connect to RDS

problems with path:
which psql
ls/applications/postgress.app/content/verison/latest/bin

vim ~/.bash_profile  put the path
:${PATH} append existing path at the end, have to do it to keep all commands
when problem zsh, do source ~/.bash_profile   
which psql  tells you which one
