The project “IT Company Website” is a responsive website made using HTML, CSS, Bootstrap and JavaScript and Django.
As it is responsive, it works well on all devices. The website includes modules like About, Services, Portfolio, Team, Career, Contact and Blog.
Whenever anyone submits the contact form or career form, an email is sent on company’s email id so that they get notified about it and can communicate with that person soon.
The website contains all the modules that meet the project requirement and is doing all the work accurately.

Quick start
-----------

1. Create and activate a virtual environment (Windows PowerShell):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Install dependencies:

```powershell
.\.venv\Scripts\python -m pip install --upgrade pip setuptools wheel
.\.venv\Scripts\python -m pip install -r requirements.txt
```

3. Apply migrations and run the development server:

```powershell
.\.venv\Scripts\python manage.py migrate
.\.venv\Scripts\python manage.py runserver
```

Notes
-----
- I added `requirements.txt` (generated from the project's virtualenv) to make setup reproducible.
- I fixed duplicate/missing local script includes in `templates/header.html` — the footer already includes the required JS and using both caused 404s. If you see missing static files, run `collectstatic` (for production) or ensure `STATICFILES_DIRS` / `STATIC_ROOT` settings are configured correctly.

Youtube demo link: https://www.youtube.com/watch?v=qqVmGFLJ0_c
