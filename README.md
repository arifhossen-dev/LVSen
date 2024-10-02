# About LVSen

## Laravel + Vue 3 + Inertia.js Application

This is a full-stack web application built using **Laravel** as the backend framework, **Vue 3** as the frontend
framework, and **Inertia.js** to bridge the two. The project uses **Vite** as the build tool for the frontend, *
*TailwindCSS** for styling, and **TypeScript** to improve type safety in the frontend code.

## Table of Contents

- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Features

- Laravel 11 for the backend
- Vue 3 for the frontend
- TypeScript support for the frontend code
- TailwindCSS for easy and responsive UI design
- Inertia.js for SPA (Single Page Application) functionality without the need for an API
- Ziggy for managing routes between Laravel and Vue
- Sanctum for authentication
- Vite for fast development builds

## Technologies

This project uses the following technologies:

### Backend

- **[Laravel](https://laravel.com/)**: A PHP framework for modern web applications.
- **[Inertia.js](https://inertiajs.com/)**: Provides a modern monolithic approach to SPAs without APIs.
- **[Laravel Sanctum](https://laravel.com/docs/sanctum)**: A simple package for API token authentication.
- **[Laravel Breeze](https://laravel.com/docs/11.x/starter-kits#laravel-breeze)**: A starter kit for authentication
  scaffolding.

### Frontend

- **[Vue 3](https://vuejs.org/)**: The progressive JavaScript framework.
- **[TailwindCSS](https://tailwindcss.com/)**: A utility-first CSS framework for styling.
- **[Vite](https://vitejs.dev/)**: A frontend build tool with fast development and optimized builds.
- **[TypeScript](https://www.typescriptlang.org/)**: For type-safe JavaScript development.

## Installation

Follow these steps to get the project up and running locally.

### Prerequisites

Make sure you have the following installed on your system:

- [PHP 8.2+](https://www.php.net/)
- [Composer](https://getcomposer.org/)
- [Node.js](https://nodejs.org/) (v16+)
- [NPM](https://www.npmjs.com/) or [Yarn](https://yarnpkg.com/)

### Clone the Repository

```bash
git clone https://github.com/arifhossen-dev/LVSen.git
cd LVSen
```

### Backend Setup (Laravel)

1. Install PHP dependencies:
    ```bash
    composer install
    ```

2. Copy the example `.env` file and update environment variables:
    ```bash
    cp .env.example .env
    ```

3. Generate the application key:
    ```bash
    php artisan key:generate
    ```

4. Run the migrations to set up the database:
    ```bash
    php artisan migrate
    ```

### Frontend Setup (Vue 3 + Inertia.js)

1. Install Node.js dependencies:
    ```bash
    npm install
    ```

2. Build the frontend assets:
    ```bash
    npm run dev
    ```

## Running the Application

After completing the installation steps, you can start the local development server with:

```bash
php artisan serve
```

And in another terminal window, run the Vite development server:

```bash
npm run dev
```

The application should now be available at `http://localhost:8000`.

## Project Structure

Here is a high-level overview of the project's structure:

```
├── app/                    # Laravel backend logic
├── resources/
│   ├── js/                 # Vue.js components and pages
│   ├── views/              # Blade templates for Inertia.js
│   └── css/                # TailwindCSS configuration and styles
├── routes/
│   └── web.php             # Laravel routes
├── composer.json           # PHP dependencies
├── package.json            # Node.js dependencies
└── vite.config.ts          # Vite configuration
```
