# Book Store Management System

## Overview
The Book Store Management System is a Spring Boot application that provides functionality to manage books and maintain a custom list of favorite books. Users can:

- Add, edit, and delete books in the main catalog.
- Maintain a personal list of favorite books.

## Features
1. **Book Management**:
   - Add new books to the catalog.
   - Edit existing book details.
   - Delete books from the catalog.
   - View a list of all available books.

2. **My Book List**:
   - Add books to a personalized list.
   - Remove books from the personalized list.
   - View the personalized list of books.

## Technologies Used
- **Spring Boot**: For backend development.
- **Spring Data JPA**: For ORM and database interaction.
- **Thymeleaf**: For frontend template rendering.
- **H2 Database**: In-memory database for development and testing.

## Project Structure
### Controllers
1. **BookController**:
   - Manages book-related operations such as adding, editing, and deleting books.
   - Routes:
     - `/book_register`: Displays the book registration form.
     - `/available_books`: Displays the list of all available books.
     - `/mylist/{id}`: Adds a book to the personalized list.
     - `/editBook/{id}`: Edits an existing book.
     - `/deleteBook/{id}`: Deletes a book by ID.

2. **MyBookListController**:
   - Manages the personalized book list.
   - Routes:
     - `/deleteMyList/{id}`: Removes a book from the personalized list.

### Entities
1. **Book**:
   - Represents a book in the main catalog.
   - Fields: `id`, `name`, `author`, `price`.

2. **MyBookList**:
   - Represents a book in the personalized list.
   - Fields: `id`, `name`, `author`, `price`.

### Repositories
- **BookRepository**: Extends `JpaRepository` for `Book` entity.
- **MyBookRepository**: Extends `JpaRepository` for `MyBookList` entity.

### Services
1. **BookService**:
   - Handles business logic for book-related operations.
   - Methods: `save`, `getAllBook`, `getBookById`, `deleteById`.

2. **MyBookListService**:
   - Handles business logic for the personalized book list.
   - Methods: `saveMyBooks`, `getAllMyBooks`, `deleteById`.

## How to Run
1. Clone the repository:
    ```bash
    git clone https://github.com/Mostafa-Hisham0/OOAD-Project.git
    cd bookstore-management
    ```

2. Build and run the application:
    ```bash
    mvn spring-boot:run
    ```

3. Access the application:
    - Home Page: `http://localhost:1001/`

## Sample Routes
- **Book Registration**: `http://localhost:1001/book_register`
- **Available Books**: `http://localhost:1001/available_books`
- **My Books List**: `http://localhost:1001/my_books`

## Database Schema
- **Book** Table:
  - `id`: Primary key
  - `name`: Book name
  - `author`: Author name
  - `price`: Book price
- **MyBooks** Table:
  - `id`: Primary key
  - `name`: Book name
  - `author`: Author name
  - `price`: Book price


## License
This project is open-source and available under the MIT License.
