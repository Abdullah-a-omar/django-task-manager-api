# Task Management API 📝

A RESTful API built with Django and Django REST Framework for managing tasks, featuring full CRUD operations, search and filtering capabilities, and Swagger documentation.

## 🚀 Features

- **Full CRUD Operations**: Create, read, update, and delete tasks.
- **Search & Filtering**: Search tasks by title/description and filter by completion status.
- **Interactive Documentation**: Integrated Swagger UI and OpenAPI schema with `drf-spectacular`.

## 🛠 Tech Stack

- **Backend**: Python, Django, Django REST Framework
- **Filtering**: `django-filter`
- **Documentation**: `drf-spectacular` (Swagger UI)

## 📌 API Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/api/tasks/` | Retrieve a list of all tasks (Supports search & filter) |
| `POST` | `/api/tasks/` | Create a new task |
| `GET` | `/api/tasks/{id}/` | Retrieve a specific task by ID |
| `PUT` | `/api/tasks/{id}/` | Update all fields of a task |
| `PATCH` | `/api/tasks/{id}/` | Partially update a task |
| `DELETE` | `/api/tasks/{id}/` | Delete a task |
| `GET` | `/api/docs/` | Interactive Swagger UI Documentation |
| `GET` | `/api/schema/` | OpenAPI 3.0 Schema file |

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Abdullah-a-omar/django-task-manager-api.git
   cd django-task-manager-api

2. **Create and activate a virtual environment:**
   python -m venv venv
   # Windows:
   venv\Scripts\activate
   # Linux/macOS:
   source venv/bin/activate

3. **Install dependencies:**
   pip install -r requirements.txt

4. **Apply database migrations:**
   python manage.py migrate

5. **Run the development server:**
  python manage.py runserver

6. **Access Documentation:**
  Open http://127.0.0.1:8000/api/docs/ in your browser