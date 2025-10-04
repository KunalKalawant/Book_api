Book Review API

A Node.js application to manage a book store where users can view books, search by ISBN, author, or title, and manage book reviews. Registered users can add, modify, or delete reviews securely using JWT authentication.

Project Overview:

This project provides a RESTful API for a small book store. Users can view book lists, search for books, and manage reviews. Registered users can add or modify reviews, and all protected routes require JWT authentication.

Features:

View all books
Search books by ISBN, author, or title
View book reviews
Register and login as a user
Add, update, or delete reviews (registered users only)
Async operations using callbacks and Promises

Technologies Used

Node.js
Express.js
Axios
JSON Web Tokens (JWT)

API Endpoints:

User Endpoints:
POST /register: Register a new user
POST /login: Authenticate and get JWT

Book Endpoints:

GET / : Get all books

GET /isbn/:isbn : Get book details by ISBN

GET /author/:author : Get books by author

GET /title/:title : Get books by title

GET /review/:isbn : Get book reviews

Protected Endpoints (JWT required):

PUT /auth/review/:isbn : Add or modify a book review

DELETE /auth/review/:isbn : Delete your book review
