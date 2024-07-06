# Robot Direction Control Project

## Introduction
This project allows you to control a robot's movements via a web interface. 
It involves creating an HTML interface with buttons for directional commands (Stop, Forward, Backward, Left, Right) that interact with a MySQL database (`my_robot_db`) through PHP (`save_direction.php`).

## Prerequisites
### XAMPP Installation
1. Download XAMPP from [https://www.apachefriends.org/index.html](https://www.apachefriends.org/index.html).
2. Install XAMPP on your system.

### Starting Apache and MySQL
1. Open the XAMPP Control Panel.
2. Start the Apache and MySQL services.

### Creating Database
1. Open phpMyAdmin (http://localhost/phpmyadmin).
2. Create a new database named `my_robot_db`.

### Database Table Creation
1. Within the `my_robot_db` database, execute the following SQL query to create the `directional_table`:

\`\`\`sql
CREATE TABLE directional_table (
    id INT(11) AUTO_INCREMENT PRIMARY KEY,
    direction VARCHAR(10) NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
\`\`\`

## Setting Up Project Files
### Creating Project Directory
1. Open Visual Studio Code (VS Code).
2. Navigate to the XAMPP `htdocs` folder (`C:\xampp\htdocs`).
3. Create a new folder named `example1` for your project.

### Project Structure
- `example1/`
  - `Directional.html`: HTML interface for controlling robot directions.
  - `style.css`: CSS file for styling the HTML interface.
  - `script.js`: JavaScript file for client-side functionality.
  - `save_direction.php`: PHP script to handle saving direction commands to the database.
  - `code/`: Folder to organize all project code files.

## HTML Interface
### Creating HTML File (`Directional.html`)
1. Inside `example1/`, create a new file named `Directional.html`.
2. Add HTML code for buttons to control robot directions (Stop, Forward, Backward, Left, Right). Below is a sample structure:

### CSS Styling
#### Creating CSS File (`style.css`)
1. Inside `example1/`, create a new file named `style.css`.
2. Write CSS code to style the HTML interface for better presentation and user experience.

### JavaScript Functionality
#### Creating JavaScript File (`script.js`)
1. Inside `example1/`, create a new file named `script.js`.
2. Write JavaScript code to implement client-side functionality for button interactions and AJAX requests.

## PHP Backend
### Creating PHP File (`save_direction.php`)
1. Inside `example1/`, create a new file named `save_direction.php`.
2. Write PHP code to handle saving direction commands to the database `my_robot_db`.

### Interface Screenshot
![HTML Interface](./Images/Directional_Interface.png)
*Screenshot of the HTML interface with directional buttons.*

### Database Table Screenshot
![Database Table](./Images/directional_table.png)
*Screenshot of the \directional_table\ structure in \my_robot_db\.*

## Code Folder
### Code Directory (`code/`)
- Place all project code files here, including `Directional.html`, `style.css`, `script.js`, and `save_direction.php`.

## Conclusion
This project enables you to control a robot's movements using a web interface powered by HTML, CSS, JavaScript, and PHP. Follow the steps above to set up and run the project successfully.                                                       this is what i writ in the redme file and i like it
