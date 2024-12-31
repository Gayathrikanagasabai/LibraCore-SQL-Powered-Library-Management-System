# LibraCore-SQL-Powered-Library-Management-System
A SQL-based Library Management System for managing books, members, and transactions with features like tracking availability and analyzing borrowing trends.


## Features
- Book inventory management (add, update, delete books).
- Member management.
- Borrowing and returning books.
- Track availability and borrowing history.
- Analyze most borrowed books and top members.

## Database Structure
### Tables:
- **Books**: Stores book details like title, author, publication year, and availability.
- **Members**: Contains member details like name, email, and phone.
- **Transactions**: Tracks book issue and return dates linked to members.

## SQL Queries Overview
- Add, update, and delete books.
- Check book availability.
- List and manage members.
- Track borrowed books and return updates.
- Analyze most borrowed books and active members.

## Usage
1. **Database Setup**: Run the provided SQL script to create the `LibraryDB` database and populate it with sample data.
2. **Execute Queries**: Use the SQL queries to interact with the database.
3. **Analyze Data**: Retrieve statistics like borrowing trends and member activity.

## Getting Started
### Prerequisites
- SQL database (e.g., MySQL).
- SQL client for executing queries.

### Steps
1. Clone or download this repository.
2. Set up the database by running the SQL script.
3. Use a SQL client to execute queries and interact with the system.

## Sample Queries
- **Check Book Availability**:
  ```sql
  SELECT title, availability FROM Books WHERE book_id = 1;
  ```
- **Add a New Member**:
  ```sql
  INSERT INTO Members (name, email, phone) VALUES ('John Doe', 'john.doe@example.com', '1234567890');
  ```
- **Record a Transaction**:
  ```sql
  INSERT INTO Transactions (book_id, member_id, issue_date) VALUES (1, 1, '2024-12-22');
  ```

## Contributions
Contributions are welcome! Feel free to fork and submit pull requests.

## License
This project is licensed under the MIT License.
