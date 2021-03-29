date: 2021-03-29
title: "Task-B"
linkTitle: "Task-B"
author: Sacha Wharton
---

*Contributed by Sacha Wharton* 

@sachajw

<div>
<img src="./images/ufo-abduct-cow.jpg" alt="task-c" height="192px" width="192x" />
</div>
<p></p>

# task-B

## Setup
* Language [Python3](https://www.python.org/)
* OS [Ubuntu 20.04](https://ubuntu.com/)
* IDE [Microsoft VS Code](https://code.visualstudio.com/)

## Requirements
* Using a simple micro web framework, expose the functionality of the bubble sort algorithm using HTTP and JSON.
* Write a script to automate your tests and static code analysis tools checks, that can run before starting up your development server on localhost.
* If there is any failure, your server should not start up.

## Bubble Sort
Lets describe the Python file bubble-sort.py.

* I use the ```bash``` terminal in ```Ubuntu 20.04```.
* I used the [Flask Framework](https://flask.palletsprojects.com/en/1.1.x/) to present the bubble sort algorithm as json in the browser.
* In order to run the development server change into the ```app``` directory and run ```python3 bubble-sort.py``` in your terminal.
* Access the web page in your browser here http://localhost:5000

## Test & Static Code Analyzer
After comparing [Tox](https://tox.readthedocs.io/en/latest/index.html) and [Nox](https://nox.thea.codes/en/stable/).
I choose Nox because it uses the Python language to configure its tests. You can find the cmd line [here](https://nox.thea.codes/en/stable/usage.html)
I created ```noxfile.py``` with two sessions, one for testing/code coverage using [Pytest](https://docs.pytest.org/en/stable/contents.html) abd one for linting using [Flake8](https://flake8.pycqa.org/en/latest/). 
I created a ```requirements.txt``` file for all the neccessary dependencies to be installed for the [Python](https://www.python.org/) application ```bubble-sort.py```,
and for all the neccessary plugins to be installed for [Pytest](https://docs.pytest.org/en/stable/contents.html).

In order to run the tests, just type ```nox``` in the route and it will go through the ```test``` session and the ```linting``` session.
Nox uses ```noxfile.py``` for all its session and confiugration. You will see to sections one for test and one for linting.

## Phone a friend!
* Write a script to automate your tests and static code analysis tools checks, that can run before starting up your development server on localhost.
* If there is any failure, your server should not start up.

**:heartpulse:LoveYourCodies**