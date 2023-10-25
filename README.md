# Arpi Tool API

## REST API with CRUD for E-commerce Operations

This is a REST API designed to facilitate e-commerce operations with CRUD (Create, Read, Update, Delete) functionality.

## Installation

To run this application on your local environment, follow these steps:

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Install the required dependencies: `composer install`.
4. Configure your database connection in the `.env` file.
5. Run migrations: `php artisan migrate`.
6. Install Laravel Passport: `php artisan passport:install`.
7. Start the application: `php artisan serve`.

## API Documentation

### Endpoints:

- User Registration: `/api/register`
- User Login: `/api/login`
- User Logout: `/api/logout`

#### Products:

- List All Products: `/api/products`
- List Products by Category: `/api/products/{category_id}`
- Get a Single Product: `/api/single-product/{id}`

#### Categories:

- List All Categories: `/api/categories`
- Get a Single Category by ID: `/categories/{id}`

#### Create, Update, and Delete:

- Add a New Product: `/api/add-product`
- Add Multiple Products: `/api/add-products`
- Update a Product: `/api/update-product/{id}`
- Delete a Product: `/api/delete-product/{id}`
- Add a Category: `/api/add-category`
- Update a Category: `/api/update-category/{id}`
- Delete a Category: `/api/delete-category/{id}`

### JSON Data Format

When making requests to these endpoints, ensure that your data is in JSON format.

#### User Registration:

```json
{
    "name": "John Doe",
    "email": "john@doe.com",
    "password": "password",
    "c_password": "password",
    "role": "admin"
}
