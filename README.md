# Books API

A simple RESTful API for managing books built with Express.js. This API provides CRUD operations for a book collection with in-memory storage.

## Features

- **CRUD Operations**:
  - Create, Read, Update, and Delete books
- **Validation**:
  - Input validation for required fields
- **Error Handling**:
  - Proper HTTP status codes and error messages
- **In-Memory Storage**:
  - Simple data persistence (resets on server restart)

## API Endpoints

| Method | Endpoint       | Description                          | Required Fields           |
|--------|----------------|--------------------------------------|---------------------------|
| GET    | `/books`       | Get all books                        | None                      |
| POST   | `/books`       | Add a new book                       | `title`, `author`         |
| PUT    | `/books/:id`   | Update a book by ID                  | At least one: `title` or `author` |
| DELETE | `/books/:id`   | Delete a book by ID                  | None                      |

## Request and Response Examples

### Get All Books
**Request:**
```http
GET /books
