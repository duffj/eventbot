eventbot
========

A Slack bot written in Python providing useful integration with Eventbrite.

[![CircleCI](https://circleci.com/gh/duffj/eventbot.svg?style=svg)](https://circleci.com/gh/duffj/eventbot)


Prerequisities
--------------

* Python >=2.7 with pip and virtualenv
* If you want to make use of Heroku's convenient local development environment, install Heroku Toolbelt.
* GNU make, for installing stuff


Build and run
-------------

The app runs in Heroku, and is also built on commit by CircleCI.

To view status:

    heroku login
    heroku status

For local dev:

    make heroku-local

To deploy to Heroku:

    heroku login
    make deploy

To run the tests:

    . .venv/bin/activate
    make test


Features
--------

* Runs in Heroku
* `@eventbot help`
* `@eventbot events` - list currently live events

### Backlog

1. Logging via `python eventbot.py`.
1. Logging via `flask run`
1. Display stats from Eventbrite.
1. Post ticket sales into a channel once per day.
1. Add a basic web interface.


References
----------

* [Eventbrite APIv3 Developer Documentation](https://www.eventbrite.com/developer/v3/)
* https://www.fullstackpython.com/blog/build-first-slack-bot-python.html
* https://blog.heroku.com/how-to-deploy-your-slack-bots-to-heroku
* http://flask.pocoo.org/docs/0.11/quickstart/
* http://flask.pocoo.org/docs/0.11/deploying/wsgi-standalone/
* https://devcenter.heroku.com/articles/python-gunicorn
