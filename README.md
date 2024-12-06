# INET4031 PHP Crude CRUD App  
**A basic PHP CRUD (Create, Read, Update, Delete) application with HTML and PHP, designed to interact with a MariaDB/MySQL database.**  

## Overview  
This project is part of the INET4031 coursework, providing a hands-on demonstration of CRUD operations using PHP. It includes dynamic web pages for adding, deleting, and finding employees, with secure database connections configured for both local and external databases.  

## Project Structure  

| **File/Folder**             | **Description**                                                                                  |  
|-----------------------------|--------------------------------------------------------------------------------------------------|  
| `README.md`                 | This file, containing project details and setup instructions.                                   |  
| `addemployee.html`          | HTML form for adding a new employee.                                                           |  
| `addemployee.php`           | PHP script for processing employee addition to the database.                                   |  
| `deleteemployee.html`       | HTML form for deleting an employee.                                                            |  
| `deleteemployee.php`        | PHP script for handling employee deletion requests.                                            |  
| `findemployee.html`         | HTML form for searching employee details.                                                      |  
| `dynamic.php`               | A script to dynamically interact with database entries (specific details depend on implementation). |  
| `credentials.php`           | Default database connection file (can be configured for use).                                  |  
| `credentialsexternaldb.php` | Connection settings for an external database.                                                  |  
| `credentialslocalhost.php`  | Connection settings for a localhost database.                                                  |  

## Features  
- **Add Employees:** Submit a form to add new employees to the database.  
- **Delete Employees:** Remove employee records via an interactive form.  
- **Find Employees:** Query employee details using a search form.  
- **Flexible Database Connections:** Switch between local and external databases using dedicated configuration files.  

## Requirements  
- PHP 7.4 or higher  
- MariaDB or MySQL database  
- A web server (e.g., Apache or Nginx)  

## Setup  
1. **Clone the Repository**  
   ```bash  
   git clone https://github.com/yourusername/inet4031-php-crude-crud.git  
   cd inet4031-php-crude-crud  
   ```  

2. **Configure the Database**  
   - Import the required tables and data using your own SQL setup or a provided script (if available).  
   - Modify the appropriate `credentials.php` file (or `credentialsexternaldb.php`/`credentialslocalhost.php`) with your database connection details:  
     ```php  
     <?php  
     $host = 'your_host';  
     $db = 'your_database';  
     $user = 'your_user';  
     $pass = 'your_password';  
     ?>  
     ```  

3. **Deploy on a Web Server**  
   - Copy the repository files to your web server’s document root.  
   - Open your browser and navigate to:  
     ```
     http://localhost/inet4031-php-crude-crud/  
     ```  

## Usage  
- Use the HTML forms (`addemployee.html`, `deleteemployee.html`, `findemployee.html`) to interact with the application.  
- Update the `dynamic.php` script for additional database queries as needed.  
