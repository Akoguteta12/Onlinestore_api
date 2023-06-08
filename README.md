Online Store Category Management API
-------------------------------------
This project provides a Laravel API for managing categories in an online store using the nested set model. The API allows you to create, update, delete, and retrieve categories with support for nested hierarchy.

Getting Started
---------------
These instructions will help you set up the project on your local machine for development and testing purposes. See the "Deployment" section for notes on how to deploy the project to a production environment.

Prerequisites
--------------
Make sure you have the following software installed on your machine:

PHP 7.4 or higher
Composer
Laravel 8.x
Installing
Clone the repository to your local machine.
Install project dependencies by running composer install.
Rename the .env.example file to .env and configure the necessary environment variables (database, mail, etc.).
Generate an application key by running php artisan key:generate.
Migrate the database by running php artisan migrate.
(Optional) Seed the database with sample data by running php artisan db:seed.
Usage
-----
To start the local development server, run the following command:

shell
Copy code
php artisan serve
By default, the API will be accessible at http://localhost:8000. You can modify the port number in the .env file.

The following API endpoints are available:

-GET /api/categories: Retrieve all categories.
-GET /api/categories/{id}: Retrieve a specific category.
-POST /api/categories: Create a new category.
-PUT /api/categories/{id}: Update an existing category.
-DELETE /api/categories/{id}: Delete a category and its descendants.


API Documentation
------------------
The API documentation is automatically generated and available at /api/documentation when running the project. It provides detailed information about each endpoint, request parameters, and response formats.

Running Tests
To execute the test suite, run the following command:

shell
Copy code
php artisan test
The tests are located in the tests directory and cover various scenarios to ensure the API functions correctly.

Deployment
----------
To deploy the project to a production environment, please follow these steps:

Set up a web server (Apache, Nginx, etc.) and configure it to point to the project's public directory.
Set the necessary environment variables in the production .env file.
Generate a new application key by running php artisan key:generate --env=production.
Run the necessary database migrations by running php artisan migrate --env=production.
(Optional) Seed the database with initial data by running php artisan db:seed --env=production.
Configure any additional server-specific settings (e.g., SSL certificates, caching, etc.).
Start the web server and make sure it is accessible over the internet.
Contributing
Contributions to the project are welcome! If you have any suggestions, bug reports, or improvements, please open an issue or submit a pull request.

License
--------
This project is licensed under the MIT License.

Acknowledgments
---------------
We would like to thank the Laravel community and all the open-source contributors for their fantastic work that made this project possible.

Contact
--------
If you have any questions or need further assistance, please contact umurerwaakogutetakevine@gmail.com.
