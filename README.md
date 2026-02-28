# Treinamento Hospedagem

A Laravel-based training project for managing departments, members, and tools. This repository contains the application source, database migrations, seeders, and frontend assets used during the training exercises.

## Features

- Departments, Members and Tools management
- Association between members and tools
- Authentication scaffolded by Laravel
- Database migrations and seeders for quick setup

## Requirements

- PHP 7.4+ (or the version supported by the project)
- Composer
- Node.js and npm (for frontend assets)
- A database supported by Laravel (e.g., MySQL, MariaDB, SQLite, PostgreSQL)

## Installation

1. Clone the repository:

   git clone https://your-repo-url.git
   cd treinamento-hospedagem

2. Install PHP dependencies with Composer:

   composer install

3. Install Node dependencies and build assets (optional for development):

   npm install
   npm run dev

4. Copy the example environment file and generate an application key:

   cp .env.example .env
   php artisan key:generate

5. Configure your database settings in the `.env` file.

6. Run migrations and seed the database:

   php artisan migrate --seed

## Running the application

- Serve locally with the built-in PHP server:

  php artisan serve

- Or use the included `server.php` for a quick local entry point (useful for some hosting setups):

  php -S localhost:8000 server.php

## Tests

Run the test suite with PHPUnit:

./vendor/bin/phpunit

## Database

This project includes migrations in `database/migrations` and a `DatabaseSeeder` in `database/seeds` to populate sample data for development and testing.

## Project structure (high level)

- `app/` — Eloquent models, controllers, middleware, and providers
- `config/` — Configuration files
- `database/` — Migrations, factories and seeders
- `public/` — Public entry point and compiled assets
- `resources/` — Views, front-end assets, language files
- `routes/` — Route definitions (`web.php`, `api.php`, etc.)

## Contributing

Feel free to open issues or submit pull requests. For larger changes, open an issue first to discuss the proposed work.

## License

This project is licensed under the terms found in the `LICENSE` file.
