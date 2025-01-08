# Go Course Management API

This project is a simple RESTful API for managing course information, built using Go and the Gorilla Mux package for routing. It provides basic CRUD (Create, Read, Update, Delete) operations for course data.

## Features

*   **Create Course:** Add new courses with details like name, ID, price, and author information.
*   **Get All Courses:** Retrieve a list of all courses.
*   **Get One Course:** Fetch a specific course by its ID.
*   **Update Course:** Modify an existing course's details.
*   **Delete Course:** Remove a course by its ID.
*   **Data Format:** Uses JSON for requests and responses.
*   **In-Memory Storage:** Course data is stored in memory (no external database is used in this version).

## Technology Stack

*   **Go:** Programming language.
*   **Gorilla Mux:** Powerful HTTP router and dispatcher.
*   **Standard Library:** `net/http`, `encoding/json`

## Prerequisites

*   **Go:** Make sure you have Go installed on your system. You can download it from [https://go.dev/](https://go.dev/). Verify installation with:

    ```bash
    go version
    ```

## Getting Started

1. **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd <repository-name>
    ```

    (Replace `<repository-url>` and `<repository-name>` with your repository's URL and name)

2. **Download dependencies:**

    ```bash
    go mod download
    ```

3. **Build the project (optional, but good for testing):**

    ```bash
    go build
    ```

4. **Run the API:**

    ```bash
    go run main.go
    ```


## API Endpoints

| Method | Endpoint         | Description                               |
| :----- | :--------------- | :---------------------------------------- |
| GET    | `/`              | Serves a welcome message.                 |
| GET    | `/courses`       | Retrieves all courses.                    |
| GET    | `/course/{id}`   | Retrieves a course by ID.                 |
| POST   | `/course`       | Creates a new course.                      |
| PUT    | `/course/{id}`   | Updates an existing course by ID.         |
| DELETE | `/course/{id}`   | Deletes a course by ID.                  |
