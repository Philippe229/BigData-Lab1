# Big Data Introduction

## Cheat Sheets
- [Git sheet](https://rogerdudler.github.io/git-guide)
- [Git sheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf)
- [Pyspark sheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/PySpark_Cheat_Sheet_Python.pdf)
- [Python sheet](https://perso.limsi.fr/pointal/_media/python:cours:mementopython3-english.pdf)
- [Another Python sheet](https://programmingwithmosh.com/python/python-3-cheat-sheet/)

## Git Introduction
[Git Guide](https://rogerdudler.github.io/git-guide)

### Create GitHub account
You can create your GitHub account [here](https://github.com/join).
### Get the repository
The repository for this lab is located [here](https://github.com/azazel7/BigData-Lab1)
#### Fork the repository
#### Clone the repository
`git clone`
### Workflow
#### In a perfect world
`git add <filename>`
`git commit`
`git commit --amend`
`git push`
#### Bug Hunting
`git checkout`
### Pull Request

## Python Introduction
(Python CheatSheet)[]
### Required
- Python 3.5

### Motivations for Python
- Python is very popular in science and engineering: check [SciPy](https://scipy.org), [scikit-learn](http://scikit-learn.org).
- Python is free software (as in freedom)
- Python is portable, available for all major operating systems
- Python is a versatile language, "the second best language for everything"
- Python has a lively online community, active on [Stackoverflow](https://stackoverflow.com) and many other forums

### Other notes
- Python is an object-oriented language
- Python is an interpreted language
- [Google](google.com) and [Stackoverflow](https://stackoverflow.com) are your best friends!

### Hello World
```python
print("Hello world")
print('Hello world')
```
### Variables
Python is dynamically typed.
In this first example, `otter` is set as an integer and its value equal 3.
```python
otter = 3
```
Right after assigning 3 to `otter` you can change your mind and assign a string ...
```python
otter = "Otters will rule the world."
otter = 'Otters will rule the world.'
```
... or a list.
```python
otter = ["Otters", "will", "rule", "Mars", "in", "2037"]
otter = [67, 51, 17, 101, 48]
```

Complex numbers also work:
```python
otter = 3 + 2j
```
### Basic operations
Python is able to do all basic operations.
```python
a = 10
b = 3
```
```python
a + b
Output: 13
a - b
Output: 7
a / b
Output: 3.33
a * b
Output: 30
a % b
Output: 1
```
### Containers
#### Tuples
A tuple is an immutable serie of variables.
```python
parrot = (1, True, "otter")
print(parrot[1])
Output: True
```
You cannot modify a tuple.
```python
parrot[2] = 7 #This won't work
parrot[2].append('a') #Works because a string act like a reference.
parrot[2] = parrot[2] + "platypus" # Won't work because your are reassigning the tuple
```

Note: RDDs in Spark usually work with tuples.

#### Lists
A list is a mutable serie of variables.
```python
turtle = ["whale", 1, True] #Instanciate a new list with three values.
```

You can re-assigne the values and modify the list.
```python
turtle[0] = "fish" # assignes the string "fish" to the first element of the list
print(turtle)
["fish", 1, True]

turtle.append(72) # will append the value 72
print(turtle)
["fish", 1, True, 72]
```

#### Dictionaries
A dictionary is a mutable collection of key-value pairs. The idea is to access
values with indexes made of object rather than integers.
```python
otter = {"names" : ["Mike", "Ali"],
		 4 : True, 
		 "animals" : 78}
```
You can access the value of each index just like that:
```python
otter["names"]   # output ["Mike", "Ali"]
otter[4] 	     # output True
otter["animals"] # output 78
```

### Control Statements
#### If/Elif/Then statements
#### While statements
#### For statements
#### Containers in one line
