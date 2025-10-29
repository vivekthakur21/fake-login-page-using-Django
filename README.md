FB Clone - Django example (signup + login with secure hashing)
-----------------------------------------------------------

What's included:
- A minimal Django project named `fb_clone`
- An app `accounts` with signup/login/profile using Django's auth system
- SQLite (default) as the database

Quick start:
1. create and activate a virtualenv (recommended)
   python -m venv .venv
   source .venv/bin/activate   # mac/linux
   .venv\Scripts\activate    # windows (powershell)

2. Install requirements:
   pip install -r requirements.txt

3. Run migrations and start server:
   python manage.py migrate
   python manage.py runserver

4. Visit http://127.0.0.1:8000/ to view the app (login).

Notes:
- DEBUG=True in settings.py for development only. Replace SECRET_KEY before production.
- This project uses Django's create_user / authenticate which handle salted password hashing.
