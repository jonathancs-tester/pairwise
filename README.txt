# Pairwise technique combinations generator test


Pairwise is an open source test combinations generator written in  Python. The generator allows one to create a set of tests using "pairwise combinations" method, reducing a number of combinations of variables into a lesser set that covers most situations.

For more info on pairwise testing see http://www.pairwise.org.

## Features


  * Produces good enough dataset.
 
  * Pythonic, iterator-style enumeration interface.

  * Allows to filter out "invalid" combinations during search for the
    next combination.

  * Allows to exclude "previously tested" pairs/combinations.
    
  * Goes beyond pairs! If/when required can generate n-wise
    combinations.


## Installation


  To install Pairwise to your Python's site-packages directory, run this command from the command prompt:

   ```
    python setup.py install
   ```

  Alternatively, you can just copy the entire "pairwise" directory somewhere into your Python path.

  Ps.: Pairwise need to run with Python 3

## Troubleshooting
  If you have this problem (windows):

  1 - * ModuleNotFoundError: No module named... *

  You must run this command
  
  ```
  setx PYTHONPATH "<PythonPath>;<PythonPath>\DLLs;<PythonPath>\lib;<PythonPath>\lib\plat-win;<PythonPath>\lib\site-packages"
 ```
  Ex.:
  setx PYTHONPATH "C:\Programas\python\3.7.4;C:\Programas\python\3.7.4\DLLs;C:\Programas\python\3.7.4\lib;C:\Programas\python\3.7.4\lib\plat-win;C:\Programas\python\3.7.4\lib\site-packages"

## Execute

  ```
  python examples/example1.1.py
  ```

## Known issues


  * Not optimal - there are tools that can create smaller set covering all the pairs. However, they are missing some other important features and/or do not integrate well with Python.
  
  * Lousy written filtering function may lead to full permutation of parameters.
  
  * Version 2.0 has become slower (a side-effect of introducing ability to produce n-wise combinations).

