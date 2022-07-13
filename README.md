# Python: Getting Started

A barebones Django app, which can easily be deployed to Heroku.

This application supports the [Getting Started with Python on Heroku](https://devcenter.heroku.com/articles/getting-started-with-python) article - check it out for instructions on how to deploy this app to Heroku and also run it locally.

Alternatively, you can deploy it using this Heroku Button:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

For more information about using Python on Heroku, see these Dev Center articles:

- [Python on Heroku](https://devcenter.heroku.com/categories/python)

# Procfile
web: gunicorn gettingstarted.wsgi
web: sh setup.sh && streamlit run streamlit_app.py

# Heroku
heroku restart
git push heroku master
heroku local

# Configure database
 https://stackoverflow.com/questions/47446480/how-to-use-google-api-credentials-json-on-heroku