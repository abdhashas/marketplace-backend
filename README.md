# 🛒 E-commerce Marketplace Backend API (Laravel & MySQL)

A scalable, secure, and optimized RESTful backend API engineered for an e-commerce marketplace platform ("Souq"). This repository manages the entire core business logic, relational database schemas, and API endpoints required to power client-side applications.

## 📂 Project Structure & Laravel Core

The repository follows the standard production-ready Laravel architecture, cleanly separating business workflows from data mapping layers:
- **`app/Http/Controllers/`**: Houses the RESTful API controllers routing logic for user authentication, product listings, and cart management.
- **`app/Models/`**: Contains the Eloquent Object-Relational Mapping (ORM) models defining system entities and relational foreign key constraints.
- **`database/migrations/`**: Relational MySQL database blueprints, tables setup, and structured schema evolution migration files.
- **`routes/api.php`**: Standardized endpoint routing rules exposed securely for frontend or mobile client integrations.
- **`config/`**: Central application setting modules managing database connections, encryptions, and security packages.

## 🚀 Key System Features

- **Robust Authentication**: Implements secure user and vendor authentication workflows and session tracking.
- **Product Catalog Management**: Handles multi-vendor product listings, categorical trees, stock levels, and inventory management.
- **Shopping Cart & Order Workflows**: Controls relational operations for tracking active user shopping carts, placing orders, and processing transactional data.
- **Relational Database Architecture**: Structured MySQL database design optimized to eliminate data redundancy and handle concurrent system operations.

## 🛠️ Tech Stack & Dependencies

- **Backend Framework**: Laravel (PHP)
- **Database Management System**: MySQL
- **Architectural Pattern**: MVC / RESTful API Design
- **Package Managers**: Composer (PHP dependency manager)

## ⚙️ Setup and Installation

1. Clone this repository to your local system:
   ```bash
   git clone https://github.com
   ```
2. Install the application PHP development dependencies:
   ```bash
   composer install
   ```
3. Create and configure your local server environment file:
   ```bash
   cp .env.example .env
   ```
   *(Be sure to adjust your `DB_DATABASE`, `DB_USERNAME`, and `DB_PASSWORD` parameters inside the new `.env` file to match your MySQL database server).*
4. Generate the application secure encryption key:
   ```bash
   php artisan key:generate
   ```
5. Run the structural database migrations to seed your local database:
   ```bash
   php artisan migrate
   ```
6. Fire up the local development server:
   ```bash
   php artisan serve
   ```
