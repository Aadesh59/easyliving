-- Create the database if it doesn't exist: 
CREATE DATABASE IF NOT EXISTS easy_living;

-- Use the created database: 
USE easy_living;

-- Create the users table with the role column: 
CREATE TABLE IF NOT EXISTS users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    full_name VARCHAR(255) NOT NULL,
    email VARCHAR(255) UNIQUE NOT NULL,
    password VARCHAR(255) NOT NULL,
    role ENUM('admin', 'customer') DEFAULT 'customer',  -- Role column with default 'customer'
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
