# Todo List Backend

This is the backend API for the Todo List application built with Express.js.

## Setup

1. Install dependencies:
   ```
   npm install
   ```

2. Start the server:
   ```
   npm start
   ```
   
   For development with auto-restart:
   ```
   npm run dev
   ```

## API Endpoints

- `GET /api/todos` - Get all todos
- `GET /api/todos/:id` - Get a specific todo
- `POST /api/todos` - Create a new todo
- `PUT /api/todos/:id` - Update a todo
- `DELETE /api/todos/:id` - Delete a todo

## Request & Response Examples

### Create Todo

**Request:**
```json
POST /api/todos
Content-Type: application/json

{
  "text": "Buy groceries"
}
```

**Response:**
```json
{
  "id": "1629384756",
  "text": "Buy groceries",
  "completed": false,
  "createdAt": "2023-08-15T12:34:56.789Z"
}
```