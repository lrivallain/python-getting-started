# python-getting-started

A barebones Python app, which can easily be deployed to Heroku.

## Deploying to Heroku

```sh
# get the sample app
$ git clone https://github.com/lrivallain/python-getting-started.git
$ cd python-getting-started

# create app
$ heroku login
$ heroku create

# deploy to heroku
$ git push heroku master
$ heroku open
```

## Running Locally

Make sure you have Python [installed properly](http://install.python-guide.org). 

Also, install the [Heroku Toolbelt](https://toolbelt.heroku.com/) and [Postgres](https://devcenter.heroku.com/articles/heroku-postgresql#local-setup).

```sh
# get the sample app
$ git clone https://github.com/lrivallain/python-getting-started.git
$ cd python-getting-started

# Install python requirements
$ pip install -r requirements.txt

# Install python requirements
$ createdb python_getting_started
$ python manage.py migrate
$ python manage.py collectstatic

# Run the app
$ heroku local
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

## Documentation

For more information about using Python on Heroku, see these Dev Center articles:

- [Python on Heroku](https://devcenter.heroku.com/categories/python)
