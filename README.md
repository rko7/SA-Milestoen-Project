# SA-Milestone-Project : IGottaBook

## Overview
**`IGottaBook`** is an application that helps users explore and manage their book collections. It integrates with the **`Google Books API`** to fetch book data and uses an **`Azure SQL Database`** to store and manage this data. Users can search for books, view details, add favorites, and manage their book lists

## Features
- **Search for Books:** Look up books by title, author, or other keywords using the Google Books API.
- **Book Management:** Store and retrieve book data in the Azure SQL Database.
- **Favorite Management:** Add books to a personal favorites list.
- **Data Cleanup:** Remove test data from the database.

## Prerequisites
1. **Python 3.8+** installed on your computer.
2. Install the required Python libraries:
```
   pip install pyodbc requests
```
3. Database Configuration:
- Set up your Azure SQL Database with the necessary credentials.
- Ensure your database connection credentials (server, username, password, etc.) are stored securely as environment variables or in a private configuration file.

## Setup Instructions
1. Clone the repository.
2. Configure Environment Variables:
- Set up the following environment variables for your database:
```
  export DB_SERVER="your_server_name"
  export DB_NAME="your_database_name"
  export DB_USER="your_username"
  export DB_PASS="your_password"
```
3. Run the Application.

## Functionality Overview
- **Table Setup:** Automatically creates a `Books` table in the database if it does not exist.
- **Google Books API:** Fetches book data based on search queries.
- **Data Insertion:** Inserts book data from the Google Books API into the database.
- **Data Retrieval:** Retrieves and displays book records from the database.
- **Data Cleanup:** Deletes test data for maintenance.

## Testing the Application
1. Run Tests:
- The application includes a test function to validate its core functionality.
2. Expected Output:
- Successful creation of the `Books` table.
- Successful fetching, insertion, and retrieval of book data.
- Deletion of test data.


## License
This project is licensed under the MIT License.
