Laravel Project Setup Guide (Git Testing)
===========================

Prerequisites
-------------

Make sure you have the following installed on your system:

*   PHP (>= 8.0)
    
*   Composer https://getcomposer.org/download/
    
*   Laravel Installer (optional but recommended)
    
*   Node.js and NPM (for frontend dependencies, if applicable) (not required for Laravel API but required for React app)
    
*   MySQL
    
*   Git (https://git-scm.com/downloads)
    

Setup Instructions
------------------

### 1\. Clone the Repository

`git clone https://github.com/Hendrickhz/git_testing_app.git  ` 

`cd ./git_testing_app/  ` 

### 2\. Install PHP Dependencies

`   composer install   `

### 3\. Create and Configure .env File

`   cp .env.example .env   `

Open the .env file and update the following details according to your local setup:

`APP_NAME=Laravel   `   

`APP_ENV=local  `   

`APP_KEY=  `    

`APP_DEBUG=true`   

`APP_URL=http://localhost `  

`DB_CONNECTION=mysql`   

`DB_HOST=127.0.0.1`  

`DB_PORT=3306`   

`DB_DATABASE=git_testing_app`  

`DB_USERNAME=root`   

`DB_PASSWORD=   `  

### 4\. Generate Application Key

`   php artisan key:generate   `

### 5\. Run Database Migrations

`   php artisan migrate   `


### 6\. Start the Development Server

`   php artisan serve   `

By default, your application will be available at:

`   http://127.0.0.1:8000   `

### 6\. Check the test route

`   http://127.0.0.1:8000/test   `

Check if the word "Hello World!" appears in the screen.
