
#### root_directory = where this file lives.

## Installation

To install this app as a package in your python env:

`pip install -e .`


## Do not use pip freeze directly

Pip freeze is causing an issue for this package that
is installed locally through `pip install -e`

Hence everytime you do `pip freeze > requirements.txt`,
edit the file manually and change the line that starts with `-e`
to `-e .`


## Running

`export FLASK_APP=hedgehog` **from root_directory**

`flask run`

`heroku local`


## Migration

`flask db init` **from root_directory**

`flask db migrate`

the migration folder should exist OUTSIDE of hedgehog/hedgehog


## Testing

`python -m unittest discover testing`  **from root_directory**

