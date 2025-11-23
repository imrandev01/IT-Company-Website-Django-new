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


Here are the exact PowerShell commands to run the project from the repo root (IT-Company-Website-Django). Paste them into a PowerShell terminal.

If you haven't created the virtualenv yet (one-time):
cd path where projet
python -m venv .venv

Activate the virtualenv (PowerShell):
cd path where project
.\.venv\Scripts\Activate.ps1

Install project dependencies (once or when requirements change):
.\.venv\Scripts\python -m pip install --upgrade pip setuptools wheel
.\.venv\Scripts\python -m pip install -r requirements.txt

Apply migrations and start the dev server (bind to localhost):
.\.venv\Scripts\python manage.py migrate
.\.venv\Scripts\python manage.py runserver 127.0.0.1:8000
Open the site in your browser:

http://127.0.0.1:8000/

If you need the server to be reachable from other devices on your network:
.\.venv\Scripts\python manage.py runserver 0.0.0.0:8000

To stop the dev server in PowerShell: press CTRL+BREAK (or CTRL+C if configured).

Notes:

If PowerShell blocks running the activation script, run this once in an elevated (admin) PowerShell to allow scripts:
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
If you see missing static files in the browser, verify STATICFILES_DIRS and that static/ exists; the dev server serves static/ and media/ automatically for development.


----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Short answer: run these PowerShell commands from the project folder. Paste them one-by-one into the prompt that shows:
`PS C:\Users\imd38\OneDrive\Desktop\eee\gitclone\IT-Company-Website-Django>`

**Steps (copy & paste each line)**

1) Change to the project directory (if you’re not already there)
```powershell
cd 'C:\Users\imd38\OneDrive\Desktop\eee\gitclone\IT-Company-Website-Django'
```

2) (One-time) create a virtual environment
```powershell
python -m venv .venv
```

3) Activate the virtual environment (PowerShell)
```powershell
.\.venv\Scripts\Activate.ps1
```
If PowerShell blocks script execution, run (once, as admin or current user):
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

4) Install dependencies
```powershell
python -m pip install --upgrade pip setuptools wheel
python -m pip install -r requirements.txt
```
If you don’t have `requirements.txt`, run:
```powershell
python -m pip install Django Pillow
```

5) Apply database migrations
```powershell
python manage.py migrate
```

6) Start the development server
```powershell
python manage.py runserver 127.0.0.1:8000
```

Open the site in your browser:
- http://127.0.0.1:8000/

Stop the server: press CTRL+C (or CTRL+BREAK in PowerShell).

