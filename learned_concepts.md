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
