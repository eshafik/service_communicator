=====
Usage
=====

To use Service-Communicator in a project, add it to your `INSTALLED_APPS`:

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
