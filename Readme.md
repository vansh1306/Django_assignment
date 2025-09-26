# Healthcare Backend API - WhatBytes Assignment

This is a backend system for a healthcare application built with Django and Django REST Framework. It allows for secure user registration and management of patient and doctor records.

---

## Tech Stack

- Python
- Django & Django REST Framework
- PostgreSQL
- JWT (djangorestframework-simplejwt) for Authentication

---

## How to Set Up and Run the Project

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/vansh1306/Django_assignment](https://github.com/vansh1306/Django_assignment)
    cd Django_assignment
    ```

2.  **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    # On Windows
    venv\Scripts\activate
    # On Mac/Linux
    source venv/bin/activate
    ```

3.  **Install all dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up your `.env` file:**
    Create a `.env` file in the main project folder. Add your database credentials and a secret key like this:
    ```
    SECRET_KEY='a-new-secret-key'
    DEBUG=True
    DB_NAME='healthcare_db'
    DB_USER='postgres'
    DB_PASSWORD='your-postgres-password'
    DB_HOST='localhost'
    DB_PORT='5432'
    ```

5.  **Run database migrations:**
    ```bash
    python manage.py migrate
    ```

6.  **Run the server:**
    ```bash
    python manage.py runserver
    ```
    The API will be running at `http://127.0.0.1:8000/`.

---

## API Endpoints

A few key endpoints to test:

- `POST /api/auth/register/`
- `POST /api/auth/login/`
- `GET /api/patients/` (Requires authentication)
- `POST /api/patients/` (Requires authentication)
