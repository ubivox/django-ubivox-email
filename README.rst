=============================
Ubivox: Django e-mail backend
=============================

This is an e-mail backend for Django to route your outgoing e-mail 
through your Ubivox account.

Enabling this will route calls to ``django.core.mail.send_mail``
trough Ubivox.

Setup
=====

To install the backend::

    pip install django-ubivox-email

Then add the configuration parameters to your settings::

    UBIVOX_API_USERNAME = "sample"
    UBIVOX_API_PASSWORD = "sample"
    UBIVOX_API_URL = "https://sample.clients.ubivox.com/xmlrpc/"

    EMAIL_BACKEND = "django_ubivox_email.backend.UbivoxEmailBackend"
