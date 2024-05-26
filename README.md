<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

# User Rest API

This is a Laravel project for building a RESTful API for managing users.

## Requirements

- PHP (>= 7.4)
- Composer
- MySQL or any other compatible database

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Mahmudul-Hasan-870/User-Rest-API.git
    ```

2. Navigate to the project directory:

    ```bash
    cd User-Rest-API
    ```

3. Install dependencies:

    ```bash
    composer install
    ```

4. Copy the `.env.example` file to `.env`:

    ```bash
    cp .env.example .env
    ```

5. Generate the application key:

    ```bash
    php artisan key:generate
    ```

6. Configure your `.env` file with your database details.

7. Migrate the database:

    ```bash
    php artisan migrate
    ```

8. Start the development server:

    ```bash
    php artisan serve
    ```

The API will be available at `http://localhost:8000/api/users`.

## API Routes

- `GET /api/users`: Get all users.
- `GET /api/users/{id}`: Get a user by ID.
- `POST /api/users`: Create a new user.
- `PUT /api/users/{id}`: Update a user by ID.
- `DELETE /api/users/{id}`: Delete a user by ID.

## Usage

You can test the API using tools like Postman or cURL.

Example cURL command to create a new user:

```bash
curl -X POST http://localhost:8000/api/users \
    -H "Content-Type: application/json" \
    -d '{"name": "John Doe", "email": "john@example.com", "phone": "1234567890", "password": "secret"}'
```

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
