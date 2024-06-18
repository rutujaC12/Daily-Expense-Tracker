# Daily-Expense-Tracker


## Introduction
The Daily Expense Tracker is a web-based application designed to help you manage your daily expenses efficiently. With features to add, remove, and track expenses, this application is a perfect tool to stay on top of your financial activities.

## Features
- **User Authentication**: Secure login and registration system.
- **Add Expense**: Record new expenses with details such as amount, category, and date.
- **Remove Expense**: Delete an expense entry from your records.
- **Total Spend**: View the total amount spent over a specified period.
- **Expense List**: View a list of all recorded expenses.
- **Expense Categories**: Organize expenses into categories for better tracking and analysis.

## Installation

### Prerequisites
- Web server (e.g., Apache, Nginx)
- PHP 7.0 or higher
- MySQL or any other database system
- Composer (for PHP dependency management)

### Steps
1. **Clone the repository**:
    ```bash
    git clone https://github.com/rutujaC12/daily-expense-tracker.git
    ```
2. **Navigate to the project directory**:
    ```bash
    cd daily-expense-tracker
    ```
3. **Set up the database**:
    - Create a database named `dailyexpense`.
    - Import the provided SQL file to set up the necessary tables:
      ```sql
      source path/to/dailyexpense.sql;
      ```
4. **Configure the database connection**:
    - Edit the `config.php` file to include your database credentials:
      ```php
      <?php
      $con = mysqli_connect("localhost:3307","root","","dailyexpense");
      if (mysqli_connect_errno())
      {
        echo "Failed to connect to MySQL: " . mysqli_connect_error() .";
      }
      ?>
      ```
5. **Install dependencies**:
    ```bash
    composer install
    ```
6. **Deploy the application**:
    - Move the project directory to your web server's root directory (e.g., `/var/www/html/`).
    - Ensure that the web server has the necessary permissions to read/write to the project directory.
  
## Screenshot
- **Dashboard**
![Screenshot 2024-04-27 132345](https://github.com/rutujaC12/Daily-Expense-Tracker/assets/130744778/b6c9bfd8-cfe6-4b1b-a96d-4a00e3aabecb)

- **Add Expenses**
![Screenshot 2024-06-18 131543](https://github.com/rutujaC12/Daily-Expense-Tracker/assets/130744778/d42f866a-d8de-489c-9349-3ac3c1c4170f)

- **Manage Expenses**
![Screenshot 2024-05-10 100902](https://github.com/rutujaC12/Daily-Expense-Tracker/assets/130744778/d5e8962f-4345-4670-9e24-14626fa4476a)


## Usage
1. **Access the application**:
    - Open a web browser and navigate to `http://yourdomain.com/daily-expense-tracker`.

2. **Register/Login**:
    - Register a new account or log in using your credentials.

3. **Add an Expense**:
    - Navigate to the "Add Expense" section and fill out the form with the necessary details.

4. **Remove an Expense**:
    - Go to the "Expenses" section, find the expense you want to remove, and click the delete button.

5. **List All Expenses**:
    - Navigate to the "Expenses" section to view all recorded expenses.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
