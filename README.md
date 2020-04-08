# NEWD Current point: 
NEWD website repository.

NEWD is the blog of Luis G.
------------------------------------------------------------------------------------------------------------------------------

NEWD was designed using the Python3 tool Flask: https://flask.palletsprojects.com/en/1.1.x/

## How to clone and run locally:

### Create a project folder and a venv folder within OR clone this project.
$git clone https://github.com/lgago/NoEasyWayDown.git

$cd NEWD

$ python3 -m venv venv

### Activate the virtual enviornment. 
$ . venv/bin/activate

### Install Flask in you Venv.
$ pip install flask

OR if you have a setup.py file:

$ pip install -e .

### Set the enviornment variables.
$ export FLASK_APP=NEWD

$ export FLASK_ENV=development

$ flask init-db

### Run the flask app.
$ flask run

### Navigate to the local URL.
http://127.0.0.1:5000/

### Test
$ pip install '.[test]'

$ pytest

#### Run with coverage report:

$ coverage run -m pytest

$ coverage report

$ coverage html  # open htmlcov/index.html in a browser
