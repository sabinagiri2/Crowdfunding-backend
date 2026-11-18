# Crowdfunding Backend

Backend application for the Crowdfunding Platform, developed using Python, Django and Django REST Framework.

## Technology Stack

- Python
- Django
- Django REST Framework
- Django REST Framework Simple JWT
- Django CORS Headers
- Pillow
- python-dotenv
- SQLite (planned initial development database)

## Project Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/Crowdfunding-backend.git
cd Crowdfunding-backend
```

Replace `YOUR-USERNAME` with your actual GitHub username.

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the virtual environment

Windows PowerShell:

```powershell
.\venv\Scripts\Activate.ps1
```

### 4. Install dependencies

```bash
pip install django djangorestframework django-cors-headers djangorestframework-simplejwt pillow python-dotenv
```

### 5. Save dependencies

```bash
pip freeze > requirements.txt
```

### 6. Create the Django project

```bash
django-admin startproject config .
```

### 7. Create Django applications

```bash
python manage.py startapp accounts
python manage.py startapp campaigns
python manage.py startapp donations
python manage.py startapp payments
python manage.py startapp organizations
python manage.py startapp payouts
```

### 8. Run the development server

After initializing the Django project and applying database migrations:

```bash
python manage.py runserver
```

The backend will run locally at:

http://127.0.0.1:8000/

## Project Structure

The planned backend structure is:

```text
Crowdfunding-backend/
│
├── config/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── accounts/
├── campaigns/
├── donations/
├── payments/
├── organizations/
├── payouts/
│
├── manage.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

## Current Progress

- Python virtual environment created.
- Required Python packages installed.
- Python dependencies saved in requirements.txt.

## Planned Backend Modules

- **Accounts and Authentication:** User registration, login and role-based access.
- **Campaign Management:** Create, update and manage fundraising campaigns.
- **Organisation Verification:** Organisation registration and admin approval.
- **Donations:** Manage donor contributions.
- **Payments:** Handle payment transactions.
- **Payout Management:** Manage withdrawal and payout requests.
- **Admin Management:** Review applications, campaigns, payouts and audit logs.



