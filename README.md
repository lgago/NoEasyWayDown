# NEWD Current point: 
NEWD website repository. This website is hosted on PythonAnywhere at http://noeasywaydown.pythonanywhere.com/

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

#### TO DO:

1. A detail view to show a single post. Click a post’s title to go to its page. [DONE-Edit1]

2. Make NoEasyWayDown at the top of each page clickable, and have it return you to the home screen. [Done-Edit2]

3. Add error logging for various scenarios. [Done-Edit2]

4. Create two user types. Admin user (myself) and read/comment only user (anyone that isn't me that logs into my blog). [Edit3]

5. Like / unlike a post. 

6. Comments.

7. Tags. Clicking a tag shows all the posts with that tag.

8. A search box that filters the index page by name.

9. Paged display. Only show 5 posts per page.

10. Upload an image to go along with a post.

11. Format posts using Markdown.

12. An RSS feed of new posts.
