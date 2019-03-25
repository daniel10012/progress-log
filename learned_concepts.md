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
.gitignore(venv idea secrets) and secrets.py
gitinit
python manage.py migrate
add sqlite database to gitignore
python manage.py runserver
python manage.py createsuperuser (to create an admin)
git add .    
git commit -m "inital setup"
python manage.py startapp appname  (creates app file on top of management app we have)
in models.py -> put db models as class (singular in django)
class inherits from models.Model
add our new app logs in setting.py in our management app (dont forget "," at the end can mess up django)
python manage.py makemigrations (creates initial.py in the migrations file of our app)
python manage.py sqlmigrate logs 0001   (show what SQL does)      


