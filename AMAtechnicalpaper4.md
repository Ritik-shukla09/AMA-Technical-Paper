

## 1. What is Django and why is it used?
Django is a high-level Python web framework used to develop secure, scalable, and maintainable web applications quickly. It follows the DRY (Don’t Repeat Yourself) principle and provides built-in features like authentication, admin panel, ORM, and protection against security threats such as SQL Injection, CSRF, and XSS.

---

## 2. What is `settings.py` in Django?
`settings.py` is the main configuration file of a Django project. It contains project-wide settings such as database configuration, installed applications, middleware, templates, static and media files, security keys, and debug options.

---

## 3. What is a Model in Django?
A Model in Django represents the database structure. Each model maps to a database table, and each field represents a column. Models are defined as Python classes and managed using Django ORM.

---

## 4. How to stop the Django server?
To stop the Django development server, press:

CTRL + C

## 5. What is WSGI in Django?

WSGI (Web Server Gateway Interface) is a standard interface that allows Django applications to communicate with web servers like Apache or Gunicorn. It acts as a bridge between the web server and the Django application and is mainly used for production deployment.

## 6. What is the MTV architecture in Django?

Django follows the MTV (Model–Template–View) architecture:

Model: Handles database logic

Template: Handles presentation/UI

View: Handles business logic

Request flow:
User → URL → View → Model → View → Template → User

## 7. Difference between Django and Flask?

Django is a full-stack framework with built-in features like ORM, authentication, and admin panel, making it suitable for large applications. Flask is a micro-framework with minimal built-in features, offering more flexibility and better suited for small applications and APIs.

## 8. What is INSTALLED_APPS?

INSTALLED_APPS is a list in settings.py that contains all enabled applications in a Django project, including default Django apps, custom apps, and third-party apps. Django loads app-related functionality based on this list.

## 9. What is manage.py?

manage.py is a command-line utility used to interact with a Django project. It is used to run the development server, create apps, apply migrations, open the Django shell, and perform administrative tasks.

## 10. What is a Django Project vs a Django App?

A Django Project is the complete website configuration containing settings and URLs, while a Django App is a modular component that performs a specific functionality. A single project can contain multiple apps.

## 11. What is ORM and why do we use it?

ORM (Object Relational Mapping) allows developers to interact with the database using Python objects instead of writing raw SQL queries. It improves readability, enhances security, ensures database independence, and helps prevent SQL injection.
```bash
