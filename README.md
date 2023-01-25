# **[Django Admin Argon PRO](https://appseed.us/product/argon-dashboard-pro/django/)**

**Django** starter styled with **[Django Admin Argon PRO](https://appseed.us/product/argon-dashboard-pro/django/)**, a premium `Bootstrap` design from [Creative-Tim](https://bit.ly/3fKQZaL).
The product is designed to deliver the best possible user experience with highly customizable feature-rich pages. 

> 👉 **NOTE**: This product `requires a License` in order to access the theme:

**Private REPO**: `git+https://github.com/app-generator/priv-django-admin-argon-pro`

<br />

## Features: 

- **UI Kit**: Argon Dashboard PRO `v1.2.1` by Creative-Tim
- [Django Argon PRO](https://github.com/app-generator/django-argon-dashboard-pro) - `sample project`
- **Sections Covered**: 
  - `Admin Section`, reserved for `superusers`
  - `All pages` managed by `Django.contrib.AUTH`
  - `Registration` page
  - `Misc pages`: colors, icons, typography, blank-page 

<br />

![Django Argon PRO - Premium Seed project powered by Flask.](https://user-images.githubusercontent.com/51070104/213974264-fe9250ff-7035-427b-b63f-bf69790f5a73.png)

<br />

## Why `Django Admin Argon PRO`

- Modern [Bootstrap](https://www.admin-dashboards.com/bootstrap-5-templates/) Design
- `Responsive Interface`
- `Minimal Template` overriding
- `Easy integration`

Designed for those who like bold elements and beautiful websites. Made of hundred of elements, designed blocks, and fully coded pages, **Soft UI Dashboard PRO** is ready to help you create stunning websites and web apps.

<br />

## How to use it

<br />

> **Install the package** via `PIP` 

```bash
$ pip install git+https://github.com/app-generator/priv-django-admin-argon-pro.git
```

<br />

> Add `admin_argon_pro` application to the `INSTALLED_APPS` setting of your Django project `settings.py` file (note it should be before `django.contrib.admin`):

```python
    INSTALLED_APPS = (
        ...
        'admin_argon_pro.apps.AdminArgonProConfig',
        'django.contrib.admin',
    )
```

<br />

> Add `LOGIN_REDIRECT_URL` and `EMAIL_BACKEND` of your Django project `settings.py` file:

```python
    LOGIN_REDIRECT_URL = '/'
    # EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
    EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
```

<br />

> Add `admin_argon_pro` urls in your Django Project `urls.py` file

```python
    from django.urls import path, include

    urlpatterns = [
        ...
        path('', include('admin_argon_pro.urls')),
    ]
```

<br />

> **Collect static** if you are in `production environment`:

```bash
$ python manage.py collectstatic
```

<br />

> **Start the app**

```bash
$ # Set up the database
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Create the superuser
$ python manage.py createsuperuser
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
```

Access the `admin` section in the browser: `http://127.0.0.1:8000/`

<br />

---
**[Django Admin Argon PRO](https://appseed.us/product/argon-dashboard-pro/django/)** - Modern Admin Interface provided by **[AppSeed](https://appseed.us/)**
