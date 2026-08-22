# 📱 Social Media Web Application

A **Django-based Social Media Web Application** built with Python and SQLite. This project provides the foundation for a social media platform with user authentication and a structured Django backend.

## 🚀 Features

* 🔐 User authentication
* 👤 User account management
* 🗄️ SQLite database
* 🎨 Static files support
* 📄 Django templates
* ⚙️ Django admin panel
* 🧩 Modular Django app structure
* 🛠️ Easy local development setup

## 🛠️ Tech Stack

* **Python 3.12+**
* **Django**
* **SQLite3**
* **HTML / CSS**
* **JavaScript**
* **Django Templates**
* **Virtual Environment (venv)**

## 📂 Project Structure

```text
socialmedia/
│
├── manage.py
├── db.sqlite3
│
├── socialmedia/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── userauth/
│   ├── migrations/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
│
├── static/
├── template/
└── venv/
```

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
cd socialmedia
```

### 2. Create a virtual environment

Windows:

```powershell
python -m venv venv
```

### 3. Activate the virtual environment

Windows PowerShell:

```powershell
venv\Scripts\Activate.ps1
```

If activation is successful, you should see:

```text
(venv)
```

### 4. Install dependencies

If the project contains `requirements.txt`:

```powershell
pip install -r requirements.txt
```

Otherwise, install Django:

```powershell
pip install django
```

### 5. Apply database migrations

Make sure you are in the directory containing `manage.py`:

```powershell
python manage.py migrate
```

### 6. Create a superuser

```powershell
python manage.py createsuperuser
```

Follow the prompts to create your Django admin account.

### 7. Start the development server

```powershell
python manage.py runserver
```

The application will be available at:

```text
http://127.0.0.1:8000/
```

## 🖥️ Django Admin

After creating a superuser, open:

```text
http://127.0.0.1:8000/admin/
```

You can use the Django admin panel to manage registered application data.

## 🔄 Development Workflow

After making changes to models, create migrations:

```powershell
python manage.py makemigrations
```

Apply them:

```powershell
python manage.py migrate
```

Run the server:

```powershell
python manage.py runserver
```

## 🔒 Environment & Security

For development, this project can use Django's default configuration. Before deploying to production:

* Set `DEBUG = False`
* Configure `ALLOWED_HOSTS`
* Use a secure `SECRET_KEY`
* Configure a production database
* Configure static and media files
* Use HTTPS
* Never commit passwords, API keys, or other secrets

## 📌 Important

Always run Django commands from the folder containing `manage.py`.

Correct:

```text
D:\PythonFullstack\socialmedia>
```

Incorrect:

```text
D:\PythonFullstack\socialmedia\socialmedia>
```

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature/new-feature
```

3. Make your changes
4. Commit your changes

```bash
git commit -m "Add new feature"
```

5. Push the branch

```bash
git push origin feature/new-feature
```

6. Open a Pull Request

## 📄 License

This project is available for learning and development purposes. Add your preferred open-source license before distributing it publicly.

---

⭐ **If you found this project useful, consider giving it a star on GitHub!**
