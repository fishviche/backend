# Django REST API Documentation

This repository contains the documentation for the Django REST API. It provides detailed information about available endpoints, required parameters, expected responses, and usage examples.

## Installation

1. Clone this repository and navigate to the specific directory

```shell
# Clone this repository to your local machine:
git clone https://github.com/fishviche/backend.git
# Navigate to the cloned directory:
cd python_backend/django_projects/crud_django
```

2. Set up a Python environment:
```shell
# Linux and MacOS
source env/bin/activate
# Install the required dependencies:
pip install -r requirements.txt
```

## Database Migrations
Before running the API, perform the following database migrations:
```shell
python manage.py migrate
```
This command will create the necessary tables and schema in the database.

## Creating a Superuser
To create a superuser (admin) account for accessing the API, run the following command:
```shell
python manage.py createsuperuser
```
Follow the prompts to enter the username, email (optional), and password for the superuser.

## Running the Django Server
To start the Django development server, execute the following command:
```shell
python manage.py runserver
```
The server will start running on http://localhost:8000/.

## Endpoints
The following endpoints are available in the API:

### Tasks
Get all tasks
```bash
GET /api/users/
```
This endpoint retrieves all the registered tasks in the system.

Create a new task
```bash
POST /api/users/
```
This endpoint retrieves all the registered tasks in the system.