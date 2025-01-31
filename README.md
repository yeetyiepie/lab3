# Working with External APIs and JSON Processing

## Objectives
- Familiarize and identify JSON as a primary data format for API development
- Parse JSON strings and traverse data in the JSON string using Python
- Convert Python data structures into a valid JSON format
- Utilize external APIs and manipulate data accordingly

## Instructions
1. Create an API that interacts with an external API and processes the retrieved data.
2. Implement the following endpoints:
   - `GET /posts/` - Retrieve all posts from an external API.
   - `GET /posts/{postId}` - Retrieve a specific post by ID.
   - `GET /comments/` - Retrieve all comments from an external API.
   - `GET /comments/{postId}` - Retrieve comments for a specific post.
   - `GET /formatted_posts/{userID}` - Retrieve posts for a specific user and format the data.
   - `GET /formatted_comment/{postID}` - Retrieve comments for a post and format the data.
   - `GET /detailed_post/{userID}` - Retrieve all posts for a user along with comments for each post.

3. Return values should be properly structured JSON objects.
4. Implement proper error handling and validation.

## Features
- Fetch and process data from an external API.
- Format JSON data to a more structured format.
- Use FastAPI for efficient API development.
- Implement proper validation and error handling.

## Requirements
- Python 3.7+
- FastAPI
- Uvicorn
- Requests

## Installation

1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/external-api-project.git
   cd external-api-project
   ```

2. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. Install dependencies:
   ```sh
   pip install fastapi uvicorn requests
   ```

## Running the API
Start the FastAPI server using Uvicorn:
```sh
uvicorn main:app --reload
```

## Usage
### Endpoints and Example Requests

#### Get All Posts
```sh
GET http://127.0.0.1:8000/posts/
```

#### Get a Specific Post
```sh
GET http://127.0.0.1:8000/posts/1
```

#### Get All Comments
```sh
GET http://127.0.0.1:8000/comments/
```

#### Get Comments for a Specific Post
```sh
GET http://127.0.0.1:8000/comments/1
```

#### Get Formatted Posts for a User
```sh
GET http://127.0.0.1:8000/formatted_posts/1
```

#### Get Formatted Comments for a Post
```sh
GET http://127.0.0.1:8000/formatted_comment/1
```

#### Get Detailed Posts with Comments for a User
```sh
GET http://127.0.0.1:8000/detailed_post/1
```

## API Documentation
Once the server is running, you can view the interactive API documentation at:
- Swagger UI: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
- ReDoc: [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)

## License
