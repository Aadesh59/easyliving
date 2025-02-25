-- Create the easy_living database:
CREATE DATABASE IF NOT EXISTS easy_living;

 -- Use the easy_living database:
 USE easy_living; 
 
-- Create the users table:
CREATE TABLE IF NOT EXISTS users ( id INT AUTO_INCREMENT PRIMARY KEY, full_name VARCHAR(255) NOT NULL, email VARCHAR(255) UNIQUE NOT NULL, password VARCHAR(255) NOT NULL, created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP );
