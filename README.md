<a ><img src="https://cdn.dribbble.com/users/976984/screenshots/2387423/telescope.gif" align="right" height="240"/></a>

## Some-Useful-Python-Modules 🧨

## About :
🔸 All the modules used in these jupyter notebooks are really helpful and can really save a lot of time making large projects.<br><br>
🔹 Would really like you to have a look at it !

## Jupyter Notebooks :
1) &nbsp;&nbsp; Unzipping and Zipping Files.ipynb
2) &nbsp;&nbsp; Collections module.ipynb
3) &nbsp;&nbsp; Math and Random Modules.ipynb
4) &nbsp;&nbsp; Opening and Reading Files.ipynb
5) &nbsp;&nbsp; Overview of Regular Expressions.ipynb
6) &nbsp;&nbsp; Python Debugger.ipynb

## Modules & libraries used :
### 💨 *Unzipping and Zipping Files*
Files can be compressed to a zip format.<br>
Python can do the task with just a few simple lines of code.<br><br>
```python
import zipfile
```
##### *Using zipfile library*
The zipfile library is built in to Python, we can use it to compress folders or files. 
To compress all files in a folder, just use the os.walk() method to iterate this process
for all the files in a directory.<br><br>
```python
import shutil
```
##### *Using shutil library*
Often you don't want to extract or archive individual files from a .zip, but instead archive 
everything at once. The shutil library that is built in to python has easy to use commands for this!<br><br>
### 💨 *Collections Module---># Counter # defaultdict # namedtuple*
```python
from collections import Counter
```


## '''

##### *Common patterns when using the Counter() object:*<br>

sum(c.values())&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# total of all counts<br>
c.clear()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# reset all counts<br>
list(c)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# list unique elements<br>
set(c)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# convert to a set<br>
dict(c)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# convert to a regular dictionary<br>
c.items()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# convert to a list of (elem, cnt) pairs<br>
Counter(dict(list_of_pairs))&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# convert from a list of (elem, cnt) pairs<br>
c.most_common()[:-n-1:-1]&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# n least common elements<br>
c += Counter()&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# remove zero and negative counts<br>

## '''
```python
from collections import defaultdict
```

```python
from collections import namedtuple
```

## '''

##### *Using namedtuple :*
The standard tuple uses numerical indexes to access its members. <br><br>
   For simple use cases, this is usually enough. On the other hand, remembering which index 
   should be used for each value can lead to errors, especially if the tuple has a lot of fields 
   and is constructed far from where it is used. A namedtuple assigns names, as well as the numerical 
   index, to each member.<br>

   Each kind of namedtuple is represented by its own class, created by using the namedtuple() factory 
   function. The arguments are the name of the new class and a string containing the names of the  
   elements.
   
  ## '''

### 💨 *Useful Math Functions & Random Module*
```python
import math
```
##### *Using math Library :*

The Python Math Library provides us access to some common math functions and constants in Python, which we can use throughout our code for more complex mathematical computations. The library is a built-in Python module, therefore you don't have to do any installation to use it.<br>

```python
import random
```
##### *Using Random Module :*


The random module is a built-in module to generate the pseudo-random variables. It can be used perform some action randomly such as to get a random number, selecting a random elements from a list, shuffle elements randomly, etc.

### 💨 *Opening and Reading Files*
##### *Getting Directories*
```python
import os
```

##### *Moving Files*
```python
import shutil
```
##### *Deleting Files*
```python
import send2trash
```

## '''
NOTE: The os module provides 3 methods for deleting files:<br>

->  os.unlink(path) which deletes a file at the path your provide !<br>
->  os.rmdir(path) which deletes a folder (folder must be empty) at the path your provide !<br>
->  shutil.rmtree(path) this is the most dangerous, as it will remove all files and folders 
    contained in the path. All of these methods can not be reversed! Which means if you make 
    a mistake you won't be able to recover the file. <br>
   
->  Instead using the send2trash module is a safer alternative that sends deleted files to the 
    trash bin instead of permanent removal.
    
## '''
### 💨 *Regular Expressions ---> #re.search #re.findall #re.compile*

## '''
Regular Expressions (sometimes called regex for short) allows a user to search for strings 
   using almost any sort of rule they can come up. For example, finding all capital letters in a 
   string, or finding a phone number in a document.

   Regular expressions are notorious for their seemingly strange syntax. This strange syntax is a
   byproduct of their flexibility. Regular expressions have to be able to filter out any string 
   pattern you can imagine, which is why they have a complex string pattern format.
  ##  '''
  
  ```python
import re
```
## '''
📌 **re.search()** will take the pattern, scan the text, and then returns a Match object.<br>
   If no pattern is found, a None is returned (in Jupyter Notebook this just means that 
   nothing is output below the cell).<br><br>
📌 **re.findall** returns all non-overlapping matches of pattern in string, as a list of strings. The string is scanned left-to-right, and matches are returned in the order found. <br><br>
 📌 **re.compile** combines a regular expression pattern into pattern objects, which can be used for pattern matching. It also helps to search a pattern again without rewriting it.
##   '''

### 💨 *Python Debugger*
```python
import pdb
```
The Python debugger provides a debugging environment for Python programs. It supports setting conditional breakpoints, stepping through the source code one line at a time, stack inspection, and more.<br><br>
Kindly have a look at [Official Docs](https://docs.python.org/3/library/pdb.html) 😀!

### 💨 *Timing your code*
## '''
 Sometimes it's important to know how long your code is taking to run, or at least know if a
    particular line of code is slowing down your entire project. Python has a built-in timing module
    to do this.
##   '''


   
    


##### *Timing Start and Stop*
```python
import time
```
Try using the time module to simply calculate the elapsed time for the code. <br>
Due to the time module's precision, the code needs to take at least 0.1 seconds 
to complete.

##### *Timeit Module*

```python
import timeit
```
What if we have two blocks of code that are quite fast, the difference from the time.time() method 
may not be enough to tell which is fater. In this case, we can use the timeit module.<br>

The timeit module takes in two strings, a statement (stmt) and a setup. It then runs the setup code 
and runs the stmt code some n number of times and reports back average length of time it took.


