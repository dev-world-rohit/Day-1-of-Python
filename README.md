# Python: Day 1
-created by Guido Van Rossum, 1989
-Python 2.0 released in 2000 and last release is Python 2.7(end of life of Python 2 April 2020)
**- Python is a language**
  -there are many implementations of python
      1. Cpython
      2. PyPy
  -even compilers that 'translate' Python code to other languages
      1. IronPython -> .NET
      2. Tython -> Java
      3. Cython -> C/C++
  - the "reference" Python implementation is CPython(most widely used)

### CPython
CPython is just a collection of bunch of files that are located in some directory.

### Py
The py launcher or just py for short is a shortcut to all the installed versions of Python on your system.
```
py <<python-version>> <<command>>
```

## Virtual Environment
In python a virtual environment performs 2 import tasks
1. Make copy of python installation.
2. provides scripts to activate and deactivate the enviroment.
    -unset the old path and set the new path
**Creating Virtual Environment**
```
py <<python-version>> -m venv <<environment-name>>
```

**Activating the Virtual Environment**
Activating the virtual environment means removing the old path from environment variables and setting the new path.
```
<path-to-environment\Scripts\activate.bat
```
**Deactivating the Virtual Environment**
Deativating the virtual environment means removing the newly set path from environment variables and setting the old path.
```
deactivate
```

## pip(Python Package Manager)
- pip is an another app/software installed alongside Python.
- it can easily install, update or remove the packages
- it uses the Python Package Index (https://pypi.org)

**Installing a Package**
```
pip install package-name
```
Some Variations in Command
1. pip install package-name==version (install package of that version)
2. pip install package-name<=1.2 (install package less than or lower than 1.2)
3. pip install package-name>2.0 (install package higher than 2.0)

**Uninstalling a Package**
```
pip uninstall package-name
```
### requirement.txt
- It is a file created alongside the code, to keep track of he required packages and versions used.
- requirement.txt is a widely accepted convention. A coder can name a file anything.

**Creating requirement.txt**
```
pip freeze > requirement.txt
```

**Installing packages inside requirement.txt**
```
pip install -r requirement.txt
```

## Python Complier/Interpreter
Python is considered as both compiiler(it compiles the code to bytecode) and interpreter(Virtual Machine OS/Platform) runs the required code line by line.

### How do we run Python
Python is a compiler/interpreter
  - reads chunk of code
  - compiles and runs it
  - output is sent

### Python can do this in two ways
**1. Interactive Mode**
  - it follows REPL(Read -> Evaluate -> Print -> Loop
  - first it reads a code then evaluate the code, then print the output and at last again repeat these things
  -  Python interactive shell

**Script Mode**
  - in this mode programmers can code the whole software and then run it.
  - python script mode
