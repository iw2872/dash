# [Volt Dashboard Django](https://appseed.us/product/volt-dashboard/django/)

Open-source **Django Dashboard** generated by `AppSeed` on top of a modern design. **[Volt Dashboard](https://appseed.us/product/volt-dashboard/django/)** is a free and open source `Bootstrap 5` Admin Dashboard featuring over 100 components, 11 example pages and 3 plugins with Vanilla JS. There are more than 100 free Bootstrap 5 components included some of them being buttons, alerts, modals, datepickers and so on.

- 👉 [Volt Dashboard Django](https://appseed.us/product/volt-dashboard/django/) - Product page
- 👉 [Volt Dashboard Django](https://django-volt-dashboard.appseed-srv1.com/) - LIVE Demo
- 👉 [Complete documentation](https://docs.appseed.us/products/django-dashboards/volt) - `Learn how to use and update the product`

<br /> 

> 🚀 Built with [App Generator](https://appseed.us/generator/), Timestamp: `2022-09-18 07:49`

- ✅ `Up-to-date dependencies`
- ✅ Database: `sqlite`
- ✅ UI-Ready app, Django Native ORM
- ✅ `Authentication`, Session Based, `OAuth` via **Github**
- ✅ [Volt Design](https://github.com/app-generator/django-admin-volt) - Theme for `admin` section

<br />

![Volt Dashboard - Full-Stack Starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/168843604-b026fd94-5969-4be7-81ac-5887cf0958e5.png)

<br /> 

## ✨ Start the app in `Docker`

> 👉 **Step 1** - Download the code from the GH repository (using `GIT`) 

```bash
$ git clone https://github.com/app-generator/django-volt-dashboard.git
$ cd django-volt-dashboard
```

<br />

> 👉 **Step 2** - Start the APP in `Docker`

```bash
$ docker-compose up --build 
```

Visit `http://localhost:5085` in your browser. The app should be up & running.

<br />

## ✨ Create a new `.env` file using sample `env.sample`

The meaning of each variable can be found below: 

- `DEBUG`: if `True` the app runs in develoment mode
  - For production value `False` should be used
- `ASSETS_ROOT`: used in assets management
  - default value: `/static/assets`
- `OAuth` via Github
  - `GITHUB_ID`=<GITHUB_ID_HERE>
  - `GITHUB_SECRET`=<GITHUB_SECRET_HERE> 

<br />

## ✨ How to use it

> Download the code 

```bash
$ git clone https://github.com/app-generator/django-volt-dashboard.git
$ cd django-volt-dashboard
```

<br />

### 👉 Set Up for `Unix`, `MacOS` 

> Install modules via `VENV`  

```bash
$ virtualenv env
$ source env/bin/activate
$ pip3 install -r requirements.txt
```

<br />

> `Set Up Database`

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> `Start the app`

```bash
$ python manage.py runserver
// OR with https
$ python manage.py runsslserver 
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

### 👉 Set Up for `Windows` 

> Install modules via `VENV` (windows) 

```
$ virtualenv env
$ .\env\Scripts\activate
$ pip3 install -r requirements.txt
```

<br />

> `Set Up Database`

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> `Start the app`

```bash
$ python manage.py runserver
// OR with https
$ python manage.py runsslserver 
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

### 👉 Create Users

By default, the app redirects guest users to authenticate. In order to access the private pages, follow this set up: 

- Start the app via `python manage.py runserver`
- Access the `registration` page and create a new user:
  - `http://127.0.0.1:8000/register/`
- Access the `sign in` page and authenticate
  - `http://127.0.0.1:8000/login/`

<br />

## ✨ Code-base structure

The project is coded using a simple and intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- core/                               # Implements app configuration
   |    |-- settings.py                    # Defines Global Settings
   |    |-- wsgi.py                        # Start the app in production
   |    |-- urls.py                        # Define URLs served by all apps/nodes
   |
   |-- apps/
   |    |
   |    |-- home/                          # A simple app that serve HTML files
   |    |    |-- views.py                  # Serve HTML pages for authenticated users
   |    |    |-- urls.py                   # Define some super simple routes  
   |    |
   |    |-- authentication/                # Handles auth routes (login and register)
   |    |    |-- urls.py                   # Define authentication routes  
   |    |    |-- views.py                  # Handles login and registration  
   |    |    |-- forms.py                  # Define auth forms (login and register) 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>         # CSS files, Javascripts files
   |    |
   |    |-- templates/                     # Templates used to render pages
   |         |-- includes/                 # HTML chunks and components
   |         |    |-- navigation.html      # Top menu component
   |         |    |-- sidebar.html         # Sidebar component
   |         |    |-- footer.html          # App Footer
   |         |    |-- scripts.html         # Scripts common to all pages
   |         |
   |         |-- layouts/                   # Master pages
   |         |    |-- base-fullscreen.html  # Used by Authentication pages
   |         |    |-- base.html             # Used by common pages
   |         |
   |         |-- accounts/                  # Authentication pages
   |         |    |-- login.html            # Login page
   |         |    |-- register.html         # Register page
   |         |
   |         |-- home/                      # UI Kit Pages
   |              |-- index.html            # Index page
   |              |-- 404-page.html         # 404 page
   |              |-- *.html                # All other pages
   |
   |-- requirements.txt                     # Development modules - SQLite storage
   |
   |-- .env                                 # Inject Configuration via Environment
   |-- manage.py                            # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />

## PRO Version

> For more components, pages and priority on support, feel free to take a look at this amazing starter:

Volt Pro is a premium Bootstrap 5 Admin Dashboard featuring over 800 components, 20 example pages and 10 fully customized plugin written in Vanilla Javascript. 

- 👉 [Django Volt PRO](https://appseed.us/product/volt-dashboard-pro/django/) - product page
  - ✅ `Enhanced UI` - more pages and components
  - ✅ `Priority` on support
  - ✅ `OAuth` via Github & Twitter
  - ✅ `Extended User profile`
  - ✅ `Improved Authentication`
  - ✅ `Tasks` Module: create, assign and edit
  - ✅ `Transaction` Module: full management

<br >

![Volt Dashboard PRO - Starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/172672843-8c40a801-3438-4e9c-86db-38a34191fbdf.png)

<br />

---
[Volt Dashboard Django](https://appseed.us/product/volt-dashboard/django/) - Open-source starter generated by **[AppSeed Generator](https://appseed.us/generator/)**.
