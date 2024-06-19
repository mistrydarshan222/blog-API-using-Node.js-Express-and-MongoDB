## Created By Darshan Mistry

-----------------------------------------------------------------------------------------------------
# Blog API
This is a simple Node.js application using Express and MongoDB to manage a collection of blog posts.
-----------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------
## Project Setup

### Steps to Set Up the Project Locally

1. Clone the repository:
    git clone https://github.com/mistrydarshan222/blog-API-using-Node.js-Express-and-MongoDB
    Run this command in command prompt

2. Install dependencies:    npm install

3. Create a `.env` file in the root directory and add MongoDB URI (Database String):
    MONGO_URI=mongodb+srv://Dmistry:skUSlpiUY6yjKIpm@midterm-api.jdevfqd.mongodb.net/?retryWrites=true&w=majority&appName=Midterm-Api
    This given string is mine, you can use your own string to show data in MongoDB
-----------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------
### Commands to Run the Project and Tests

1. Start the server:   npm start

2. The server will run at `http://localhost:3000`.

### Endpoints

- **POST /items**: Add a new blog post.
- **GET /items**: Retrieve all blog posts.
- **GET /items/:id**: Retrieve a single blog post by ID.
- **PUT /items/:id**: Update a blog post by ID.
- **DELETE /items/:id**: Delete a blog post by ID.
-----------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------
## Testing the API

You can test the endpoints using Thunder Client or any other API client. I've used Thunder Client, and here's an example for each endpoint:

### POST /items

- URL: `http://localhost:3000/items`
- Method: POST
- Body (raw JSON):
    --json--
    {
      "title": "My First Blog",
      "description": "This is the description of my first blog post.",
      "author": "Darshan",
      "publishedDate": "2023-06-18"
    }
    

### GET /items - Get all the blogs list

- URL: `http://localhost:3000/items`
- Method: GET

### GET /items/:id - Get the Single blog from its ID

- URL: `http://localhost:3000/items/<id>`
- Method: GET

### PUT /items/:id - Update the Single blog from its ID

- URL: `http://localhost:3000/items/<id>`
- Method: PUT
- Body (raw JSON):
    ```json
    {
      "title": "Updated Blog",
      "description": "This is the updated description.",
      "author": "Darshan Mistry",
      "publishedDate": "2024-06-18"
    }
    ```

### DELETE /items/:id - Delete the blog item with its ID

- URL: `http://localhost:3000/items/<id>`
- Method: DELETE
-----------------------------------------------------------------------------------------------------


