# dbms
-- Create the database (if it doesn't exist)
CREATE DATABASE IF NOT EXISTS todo_list;

-- Use the newly created database
USE todo_list;

-- Create the 'tasks' table
CREATE TABLE IF NOT EXISTS tasks (
  task_id INT AUTO_INCREMENT PRIMARY KEY,
  task_name VARCHAR(255) NOT NULL,
  description TEXT,
  is_completed BOOLEAN NOT NULL DEFAULT false
);
