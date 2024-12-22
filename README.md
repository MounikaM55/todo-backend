# API Endpoints
This frontend connects to the backend API at http://localhost:4000. Make sure the backend is running before starting the frontend.

This is the backend API for the Todo List App, built with Express.js, Prisma, and MySQL. The API provides CRUD operations for managing tasks.

## Features

- Create a new task.
- Fetch all tasks.
- Update an existing task (title, color, or completion status).
- Delete a task.
- Handles basic validation and error responses.

## Technologies Used

- **Express.js**
- **TypeScript**
- **Prisma ORM**
- **MySQL**

## Setup Instructions

1. Clone this repository:
   ```bash
   git clone <backend-repo-url>
   cd todo-backend
2. Install Dependencies
   ```bash
   npm install
3. setup database
   update .env file,  DATABASE_URL="mysql://username:password@localhost:3306/database_name"
   run prisma : npx prisma migrate dev
4. start backend server
   npm run dev
5. The API will be available at: http://localhost:4000


# API Endpoints
Base URL: http://localhost:4000

Method	Endpoint	Description	Example Payload

GET	/tasks	Fetch all tasks	

POST	/tasks	Create a new task	{ "title": "Task", "color": "red", "completed": false }

PUT	/tasks/:id	Update a task	{ "title": "New Task", "completed": true }

DELETE	/tasks/:id	Delete a task	-


