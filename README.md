# Wellness Tracker

## Overview
The Wellness Tracker is a Django-based web application designed to help users monitor and improve their overall well-being. It allows users to log daily activities such as water intake, exercise, sleep, and mood, and provides insightful reports and dashboards to track progress over time.

## Features
- **User Authentication**: Secure user registration, login, and logout functionality.
- **Profile Management**: Users can update their profile details, including weight, calorie goals, and reminders.
- **Daily Logs**: Track daily water intake, exercise, sleep hours, and mood.
- **Calorie Burn Calculator**: Calculate calories burned based on exercise type and duration.
- **Dashboard**: View recent logs and progress charts.
- **Summary Reports**: Generate weekly or monthly reports with averages and mood analysis.
- **Responsive Design**: User-friendly interface optimized for various devices.

## Installation

### Prerequisites
- Python 3.8+
- Django 5.2.3
- SQLite (default database)

### Steps
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd wellness-tracker
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Apply migrations:
   ```bash
   python manage.py migrate
   ```
5. Create a superuser for admin access:
   ```bash
   python manage.py createsuperuser
   ```
6. Start the development server:
   ```bash
   python manage.py runserver
   ```
7. Open the application in your browser at `http://127.0.0.1:8000`.

## Usage

### Logging In
- Navigate to the login page and enter your credentials.
- New users can register via the registration page.

### Adding Logs
- Use the "Add Log" feature to record daily activities.
- Update or delete logs as needed.

### Viewing Reports
- Access the dashboard for recent activity summaries.
- Generate detailed weekly or monthly reports from the "Summary Report" section.

## Project Structure
- **Project1/**: Contains project-level settings and configurations.
- **WellnessApp/**: Main application with models, views, templates, and static files.
  - `models.py`: Defines the `UserProfile` and `WellnessLog` models.
  - `views.py`: Contains views for user authentication, logging, and reporting.
  - `templates/WellnessApp/`: HTML templates for the application.
  - `static/`: Static files (CSS, JavaScript, images).

## Key Dependencies
- Django 5.2.3
- django-crontab (for scheduled tasks)
- django-widget-tweaks (for form customization)
- SQLite (default database)

## Contributing
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- Django Documentation: [https://docs.djangoproject.com/](https://docs.djangoproject.com/)
- Bootstrap for responsive design.

---
Start tracking your wellness journey today!