# 📚 Books REST API (Node.js + Express)

A simple REST API to manage a list of books.  
Data is stored **in-memory** (resets when the server restarts).  

## 🚀 Features
- Get all books
- Get a book by ID
- Add a new book
- Update a book
- Delete a book

---

## 🛠️ Setup & Installation

1. Clone this repo or create a new folder:
   ```bash
   mkdir books-api && cd books-api
Initialize project:

bash
Copy code
npm init -y
Install dependencies:

bash
Copy code
npm install express
Create server.js and add the code from this project.

Run the server:

bash
Copy code
node server.js
Server will run at:

arduino
Copy code
http://localhost:3000

API Endpoints
1. Get all books
GET /books

2. Get a single book by ID
GET /books/:id


Example: /books/1

3. Add a new book
POST /books


Body (JSON):

{
  "title": "To Kill a Mockingbird",
  "author": "Harper Lee"
}

4. Update a book
PUT /books/:id


Body (JSON):

{
  "title": "Nineteen Eighty-Four",
  "author": "George Orwell"
}

5. Delete a book
DELETE /books/:id

🧪 Testing

Use Postman
 or curl to test the endpoints.

Example using curl:

curl -X GET http://localhost:3000/books

📌 Example Response (GET /books)
[
  {
    "id": 1,
    "title": "1984",
    "author": "George Orwell"
  },
  {
    "id": 2,
    "title": "The Great Gatsby",
    "author": "F. Scott Fitzgerald"
  }
]
