=============================
Service-Communicator
=============================

.. image:: https://badge.fury.io/py/service_communicator.svg
    :target: https://badge.fury.io/py/service_communicator

.. image:: https://travis-ci.org/eshafik/service_communicator.svg?branch=master
    :target: https://travis-ci.org/eshafik/service_communicator

.. image:: https://codecov.io/gh/eshafik/service_communicator/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/eshafik/service_communicator

Service Communicator for internal services

Documentation
-------------

The full documentation is at https://service_communicator.readthedocs.io.

Quickstart
----------

Install Service-Communicator::

    pip install service_communicator

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'service_communicator.apps.service_communicator',
        ...
    )

Add Service-Communicator's URL patterns:

.. code-block:: python

    from service_communicator import urls as service_communicator_urls


    urlpatterns = [
        ...
        url(r'^', include(service_communicator_urls)),
        ...
    ]

Features
--------

* TODO

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox

Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
