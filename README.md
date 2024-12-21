# Django Event Management App

Welcome to the **Event Management App** repository! This application is designed to manage events, attendees, and tasks associated with events.

---

## Prerequisites

Ensure you have the following installed on your system:

1. **Python** (3.8 or later)
2. **Pip** (Python package manager)
3. **Virtualenv** (optional but recommended)
4. **Git**
5. **SQLite** (default database for Django)

---

## Getting Started

Follow these instructions to set up and run the project locally.

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/event-management.git
cd event-management
```

### 2. Create and Activate a Virtual Environment

#### On Windows:
```bash
python -m venv env
env\Scripts\activate
```

#### On macOS/Linux:
```bash
python3 -m venv env
source env/bin/activate
```

### 3. Install Dependencies

Install the required Python packages:
```bash
pip install -r requirements.txt
```

### 4. Apply Migrations

Run the following commands to set up the database:
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Create a Superuser

Create an admin user to access the Django admin panel:
```bash
python manage.py createsuperuser
```
Follow the prompts to set up your superuser credentials.

### 6. Run the Development Server

Start the Django development server:
```bash
python manage.py runserver
```

Visit `http://127.0.0.1:8000` in your web browser to view the application.

---

## Usage

### Access the Admin Panel
- Navigate to `http://127.0.0.1:8000/admin`.
- Log in using the superuser credentials you created earlier.

### Add Events, Attendees, and Tasks
1. Go to the admin panel.
2. Use the **Event**, **Attendee**, and **Task** sections to add and manage entries.

---

## Deployment

To deploy this project in a production environment:
1. Set `DEBUG = False` in `settings.py`.
2. Use a production-ready database like PostgreSQL.
3. Configure a web server like **Gunicorn** or **uWSGI** with **Nginx**.
4. Set up static files by running:
   ```bash
   python manage.py collectstatic
   ```
5. Use environment variables to manage sensitive information.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contributing

Feel free to fork this repository, make improvements, and submit a pull request! We welcome contributions.

---

## Support

If you encounter any issues, please open an [issue](https://github.com/<your-username>/event-management/issues) or contact the maintainer.

---

Thank you for using the Event Management App!

