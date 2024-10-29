
# Task Management Application

A simple Task Management application built with Django as the backend and React as the frontend.
This application allows users to create, read, update, and delete tasks efficiently in a single-page interface.

![image](https://github.com/user-attachments/assets/0cbda6a4-00c7-45cf-86c0-99fa00678b8e)
![image](https://github.com/user-attachments/assets/a23feb81-527b-42de-b74e-1cb794abe7bb)



## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)

#superuser
id = admin
pass = admin
## Features

- Add new tasks with title and description.
- Edit existing tasks.
- Delete individual tasks.
- Responsive design for mobile and desktop views.
- User-friendly interface using Bootstrap for styling.

## Technologies Used

- **Frontend**: 
  - React
  - Bootstrap
- **Backend**: 
  - Django
  - Django REST Framework
- **Database**: 
  - SQLite (default)

## Installation

### Prerequisites

Ensure you have the following installed on your machine:

- Python 3.x
- Node.js and npm
- Django
- Django REST Framework

### Backend Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/DnyaneshwarChavan1232/task-management-app.git
   cd task-management-app/server
Create a virtual environment:

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Run migrations:

bash
Copy code
python manage.py migrate
Start the Django server:

bash
Copy code
python manage.py runserver
Frontend Setup
Navigate to the frontend directory:

bash
Copy code
cd ../frontend
Install the required npm packages:

bash
Copy code
npm install
Start the React development server:

bash
Copy code
npm start
The application should now be running on http://localhost:3000 for React and http://localhost:8000 for Django.

Usage
Open your browser and go to http://localhost:3000.
You can add a new task by filling out the form on the left.
Existing tasks will be displayed on the right with options to edit or delete each task.

API Endpoints
Here are the API endpoints available in the Django backend:

GET /api/tasks/: Retrieve all tasks.
POST /api/tasks/: Create a new task.
PUT /api/tasks/<id>/: Update an existing task by ID.
DELETE /api/tasks/<id>/: Delete a task by ID.

## API Reference

#### Get all items

```http
  GET /api/items
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |

#### Get item

```http
  GET /api/items/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |
