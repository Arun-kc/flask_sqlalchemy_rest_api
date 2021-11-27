# A simple Product RESTful API

A simple API build using Flask for educational purpose.

## Installation

You should be having python installed in your system. If not go ahead and [install python](https://www.python.org/downloads/)

Now install `pipenv`

```python
pip install pipenv
```

You can activate your virtual env with the cmd

```python
pipenv shell
```

You can install all the dependencies as follows

```python
 pipenv install flask flask-sqlalchemy flask-marshmallow marshmallow-sqlalchemy
 ```

## Product

Product schema is as follows
```
Product {

        id: Integer (Primary Key)
        name: String
        description: String
        price: Float
        qty: Integer
}
```

## Creating DB

Get into `python shell` and run the following commands

```
from app import db
db.create_all()
```