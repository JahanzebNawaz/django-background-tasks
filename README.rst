=======================
Django Background Tasks
=======================

.. image:: https://travis-ci.org/arteria/django-background-tasks.svg?branch=master
    :target: https://travis-ci.org/arteria/django-background-tasks
    :alt: Build Status
.. image:: https://coveralls.io/repos/arteria/django-background-tasks/badge.svg?branch=master
    :target: https://coveralls.io/repos/arteria/django-background-tasks/badge.svg?branch=master&service=github
    :alt: Coverage Status
.. image:: https://readthedocs.org/projects/django-background-tasks/badge/?version=latest
    :target: http://django-background-tasks.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
.. image:: https://img.shields.io/pypi/v/django-background-tasks.svg
    :target: https://pypi.python.org/pypi/django-background-tasks
    :alt: PyPI

Django Background Task is a database-backed work queue for Django, loosely based around `Ruby's DelayedJob`_ library. This project was adopted and adapted from lilspikey_ `django-background-task`.

.. _Ruby's DelayedJob: https://github.com/tobi/delayed_job
.. _lilspikey: https://github.com/lilspikey/

To avoid conflicts on PyPI we renamed it to django-background-tasks (plural). For an easy upgrade from django-background-task to django-background-tasks, the internal module structure were left untouched.

In Django Background Task, all tasks are implemented as functions (or any other callable).

There are two parts to using background tasks:

- creating the task functions and registering them with the scheduler
- setup a cron task (or long running process) to execute the tasks

Note: this version is compatible with django >=4.0 as the the providing_arg were removed from django 4.0 onwards

Installation:

  pip install   git+https://github.com/JahanzebNawaz/django-background-tasks.git@master


Docs
====
See `Read the docs`_.

.. _Read the docs: http://django-background-tasks.readthedocs.io/en/latest/

Donations
========= 

``django-background-tasks`` is free software. If you find it useful and would like to give back, please consider to make a donation using ETH_ or Paypal_. Thank you!

.. _ETH: https://metamask.app.link/send/0x8CbA5b300E347619F3b75C1c0Dd30c707C45f9Ef@1?value=1e16
.. _PayPal: https://www.paypal.me/mrjahanzeb
