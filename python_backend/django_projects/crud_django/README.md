# Django REST API Documentation

This repository contains the documentation for the Django REST API. This REST API make an example of a CRUD basic operations to create, get, update and delete tasks. It provides detailed information about available endpoints, required parameters, expected responses, and usage examples.

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
#### Get all tasks
```bash
GET /tasks/api/v1/tasks/
```
This endpoint retrieves all the registered tasks in the system.

#### Create a new task
```bash
POST /tasks/api/v1/tasks/
```
Allows creating a new task in the system. The following parameters must be provided in the request body:

- `title`: (string) The title of the task.
- `description`: (string) The description of the task.
- `done`: (boolean) The status of the task.

#### Get a task by ID
```bash
GET /tasks/api/v1/tasks/{id}/
```
Returns the details of a specific task identified by their ID.

#### Update one task
```bash
PUT /tasks/api/v1/tasks/{id}/
```
Allows update a task in the system. The following parameters must be provided in the request body:

- `title`: (string) The title of the task.
- `description`: (string) The description of the task.
- `done`: (boolean) The status of the task.

#### Delete one task
```bash
DELETE /tasks/api/v1/tasks/{id}/
```
Allows delete a task in the system.

And so on!

Contributions