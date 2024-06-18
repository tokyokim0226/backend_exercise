# Course 5 - Django Web Framework

In many web applications, the data is stored in a database and this data can be accessed on the seb server by a programming language such as Python. Once the data is retrieved, it can then be sent to teh end users inside web pages using HTML.

**Django**
An open source web framework written in Python that is used to build large scale back end web applications

**What is HTTP**

**Project**
- In Django, a project represents the entire web application
- Django provides a set of commands that auto generates a project structure that contains the configuration and setting related to the entire web application
- project structure - way to organize your Python files and folders 

**App**
- An app is a submodule of a project
- typically used to implement functionality foro some specific purpose
- can be self contained, which means they do not rely on other apps to function - can be reused/used in other projects as well (Don't Repeat Yourself - DRY principle)

```zsh
(djenv) C:\djenv>django-admin startproject demoproject 
```

Once the ```startproject``` command from django-admin is used, it will create the following:
- **manage.py** -  the manage.py script can perform everything that the django-admin utility does
  - ```python manage.py <command>```
  - ```python manage.py startapp <name of app>```
- A folder of the same name of the project that contains the following:
  - **settings.py** - django configures specific parameters with their default values and puts them in this file
  - **urls.py** - used to define URL patterns for your project
    - maps URL path to views
    - tells Django which view to load for a given URL
    - central routing configuration for your project
  - **asgi.py** - ASGI stands for asynchronous server gateway interface
  - used to configure the ASGI application, which is useful for handling asynchronous web requests in django.
  - **wsgi.py** - Web Server Gateway Interface - used to configure teh WSGI application, which serves as the entry point for WSGI-compatible web servers to serve your project
  - **__init__.py** - an empty file that indicates to Python that the `demoproject` directory should be treated as a Python package - allows you to import the module and its submodules in Python code.

In Django, when a user navigates to a URL, the URL is routed to something called a view or a controller
- For now you can just think of view as Python functions that generate the content that makes up the webpage
- Views can receive a request and return a response
- because this request and response will take place over the web, it'll use two objects called HTTP request and HTTP response

Later, you need to map the view function to a URL
- The URL you will use in your Django project are stored as a URL configuration in a file called urls.py - url config
  - acts like a mapping chart that Django uses to determine which view functions are associated with a specific URL 