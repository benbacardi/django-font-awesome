django-font-awesome
===================

![Version Badge](https://img.shields.io/pypi/v/django-font-awesome.svg)
![Downloads Badge](https://img.shields.io/pypi/dw/django-font-awesome.svg)
![Wheel Status Badge](https://img.shields.io/pypi/wheel/django-font-awesome.svg)
![License Badge](https://img.shields.io/pypi/l/django-font-awesome.svg)

[Font Awesome](https://fortawesome.github.io/Font-Awesome/) packaged in a django app to speed up new applications and deployment.

Installation
------------

Install using `pip`:

    pip install django-font-awesome
    
Add to `font_awesome` to your `INSTALLED_APPS` in `settings.py`:

    INSTALLED_APPS = (
        ...
        'font_awesome',
        ...
    )
    
Run `collectstatic` to bring in the Font Awesome static files.
    
Usage
-----

In the template where you require Font Awesome, load Django's `static` template tag library:

    {% load static %}
    
Then use the `static` template tag to load the Font Awesome CSS:

    <link rel='stylesheet' type='text/css' href='{% static 'css/font-awesome.css' %}' />
