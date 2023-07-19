# Expense Tracker Documentation

The Expense Tracker application is designed to help users track and manage their expenses. It provides features to record, categorize, and analyze expenses, allowing users to gain insights into their spending habits and make informed financial decisions.

## Functionality
The Expense Tracker application offers the following functionality:

- **Add Expense**: Users can add new expenses by providing a description, category, amount, and date. This allows them to record their spending details accurately.

- **View Expenses**: Users can view a list of all expenses recorded in the system. The list provides information about the description, category, amount, and date of each expense.

- **Filter Expenses**: Users can filter expenses based on specific criteria such as category or date. This helps them narrow down the list and focus on specific expenses of interest.

- **Update Expense**: Users have the ability to update existing expenses. They can modify the description, category, amount, or date of an expense, providing flexibility and ensuring accurate expense records.

- **Delete Expense**: Users can delete expenses that are no longer relevant or need to be removed from the system.
## Dependencies

The Expense Tracker application is built using the following dependencies:

- Java
- Spring Boot
- Spring Data JPA
- MySQL Connector/J
- HTML/CSS/JavaScript (Front-end)

## Endpoints

The Expense Tracker application provides the following endpoints:

### Add Expense

- **Endpoint**: `/api/expenses/add`
- **Method**: POST
- **Description**: Adds a new expense to the system.
- **Request Body**:
    - `description` (string): Description of the expense.
    - `category` (string): Category of the expense.
    - `amount` (number): Amount spent for the expense.
    - `date` (string): Date of the expense in the format "YYYY-MM-DD".

### Get All Expenses

- **Endpoint**: `/api/expenses`
- **Method**: GET
- **Description**: Retrieves all expenses from the system.

### Get Expense by ID

- **Endpoint**: `/api/expenses/{id}`
- **Method**: GET
- **Description**: Retrieves a specific expense by its ID.

### Update Expense

- **Endpoint**: `/api/expenses/{id}`
- **Method**: PUT
- **Description**: Updates an existing expense with the given ID.
- **Request Body**:
    - `description` (string): Updated description of the expense.
    - `category` (string): Updated category of the expense.
    - `amount` (number): Updated amount spent for the expense.
    - `date` (string): Updated date of the expense in the format "YYYY-MM-DD".

### Delete Expense

- **Endpoint**: `/api/expenses/{id}`
- **Method**: DELETE
- **Description**: Deletes an expense with the given ID.

## Usage

To use the Expense Tracker application, follow these steps:

1. Install the required dependencies (Java, Spring Boot, MySQL Connector/J).
2. Set up a MySQL database to store the expenses.
3. Configure the database connection in the `application.properties` file.
4. Build and run the application using Spring Boot.
5. Access the application through the provided endpoints using a tool like Postman or a web browser.

