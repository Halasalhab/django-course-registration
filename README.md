# Django Course Registration App

This is a Django-based course registration application.

## Requirements

- Python 3.7
- PostgreSQL
- pipenv

## Setup Instructions

### 1. Clone the Repository

```bash
git clone <your-repo-url>
cd <your-repo-directory>
```

### 2. Set Up Python Environment
- pip install pipenv
- pipenv install
- pipenv shell

### 3. Configure PostgreSQL

```bash
- CREATE DATABASE courseRegDB;
```

### 4. Update Django Settings
Update the DATABASES setting in settings.py:
```bash
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'courseRegDB',
        'USER': 'postgres',
        'PASSWORD': 'pgAdmin',  # Use your PostgreSQL password here
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
```

### 5. Generate Secret Key
Add a .env file in the root directory and include your Django secret key:
```bash
SECRET_KEY=your_secret_key
```

### 6. Run Migrations
Apply database migrations:
```bash
python manage.py migrate
```

### 7. Run the Development Server
Start the Django development server:
```bash
python manage.py runserver
```

### 9. Access the Application
Open a web browser and go to http://127.0.0.1:8000 to access your Django application.# django-course-registration
