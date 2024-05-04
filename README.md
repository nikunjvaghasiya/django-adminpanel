# Django REST API CRUD Application

This is a Django-based REST API application that provides CRUD (Create, Read, Update, Delete) functionality for managing products and categories in an e-commerce platform.

## Features

- User authentication with register and login functionality
- CRUD operations for products
- CRUD operations for categories
- Token-based authentication (using Django's built-in session authentication)

## Getting Started

### Prerequisites

- Python 3.x
- Django 5.0.4
- Django REST Framework

### Installation

1. Clone the repository: 
https://github.com/nikunjvaghasiya/django-adminpanel.git
2. Navigate to the project directory: 
cd ecommerce-api
3. Create and activate a virtual environment (optional but recommended):
python -m venv env
source env/bin/activate  # On Windows, use env\Scripts\activate

4. Install the required packages:
pip install -r requirements.txt
5. Apply database migrations:
python manage.py migrate
6. Start the development server:
python manage.py runserver


The API should now be accessible at `http://localhost:8000/api/`.

## API Endpoints

### Authentication

- `POST /api/register/`: Register a new user
- `POST /api/login/`: Login and obtain session credentials

### Products

- `GET /api/products/`: List all products
- `POST /api/products/`: Create a new product
- `GET /api/products/<product_id>/`: Retrieve details of a product
- `PUT /api/products/<product_id>/`: Update a product
- `DELETE /api/products/<product_id>/`: Delete a product

### Categories

- `GET /api/categories/`: List all categories
- `POST /api/categories/`: Create a new category
- `GET /api/categories/<category_id>/`: Retrieve details of a category
- `PUT /api/categories/<category_id>/`: Update a category
- `DELETE /api/categories/<category_id>/`: Delete a category
