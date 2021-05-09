### Setting up a virtual environment in python

A **virtual environment** is a **Python environment** such that the **Python** interpreter, libraries and scripts installed into it are isolated from those installed in other **virtual environments**, and (by default) any libraries installed in a "system" **Python**, i.e., one which is installed as part of your operating system. I regularly use virtual environment for all my python projects however I always forget the commands for setting it up. This post is mostly for my own convenience and if it helps you setup an environment, even better !

#### To install virtualenv

```
pip install virtualenv
```

Go inside the directory of the project for which you want the environment.

```
cd my-project/
```

#### Create virtualenv using Python3

```
virtualenv -p python3 myenv
```

or

```
python3 -m venv myenv
```

#### Active your virtual environment:

```
source myenv/bin/activate
```

#### To deactivate:

`deactivate`

### Generating a requirements.txt file

"Requirements files" are files containing a list of items to be installed using [pip install](https://pip.pypa.io/en/stable/reference/pip_install/#pip-install) .

#### Activate virtual environment.

`source myenv/bin/activate`

#### Freeze the environment.

`pip freeze > requirements.txt`

#### For installing the requirements.txt on some other virtual env.

Create a virtual environment and activate it.

Then,

`pip install -r requirements.txt`
