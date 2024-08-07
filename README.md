# Task Manager

A simple task management application built with Laravel.

## Prerequisites

Before you begin, ensure you have met the following requirements:

-   You have installed PHP (7.3 or higher)
-   You have installed Composer
-   You have installed MySQL

## Setting up the Task Manager

To set up the Task Manager, follow these steps:

1. Clone the forked repository

    ```
    git clone https://github.com/your-username/task-manager.git
    cd task-manager
    ```

2. Install the project dependencies

    ```
    composer install
    ```

3. Create a copy of the .env file

    ```
    cp .env.example .env
    ```

4. Generate an application key

    ```
    php artisan key:generate
    ```

5. Configure the database in the .env file

    ```
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=task_manager
    DB_USERNAME=your_mysql_username
    DB_PASSWORD=your_mysql_password
    ```

    Replace `your_mysql_username` and `your_mysql_password` with your actual MySQL credentials.

6. Create the database

    ```
    mysql -u root -p
    ```

    ```sql
    CREATE DATABASE task_manager;
    exit;
    ```

7. Run the database migrations

    ```
    php artisan migrate
    ```

8. Start the development server

    ```
    php artisan serve
    ```

9. Visit `http://localhost:8000` in your web browser to use the application.

## Contributing to Task Manager

To contribute to Task Manager, follow these steps:

1. Fork this repository.
2. Create a branch: `git checkout -b <branch_name>`.
3. Make your changes and commit them: `git commit -m '<commit_message>'`
4. Push to the original branch: `git push origin <project_name>/<location>`
5. Create the pull request.
