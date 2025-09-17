# Todo App

A simple and beautiful todo application built with Node.js, Express, and SQLite.

## Features

- ✅ Create new todos with title and description
- ✅ Mark todos as complete/incomplete
- ✅ Edit existing todos
- ✅ Delete todos
- ✅ Responsive design that works on mobile and desktop
- ✅ Real-time updates without page refresh
- ✅ Persistent storage with SQLite database

## Prerequisites

- Node.js (version 14 or higher)
- npm (comes with Node.js)

## Installation

1. Clone or download this project
2. Navigate to the project directory:

   ```bash
   cd sample-app
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

## Running the Application

1. Start the server:

   ```bash
   npm start
   ```

2. Open your browser and go to:
   ```
   http://localhost:3000
   ```

## API Endpoints

The application provides the following REST API endpoints:

- `GET /api/todos` - Get all todos
- `GET /api/todos/:id` - Get a specific todo
- `POST /api/todos` - Create a new todo
- `PUT /api/todos/:id` - Update a todo
- `DELETE /api/todos/:id` - Delete a todo

## Project Structure

```
sample-app/
├── server.js          # Main Express server file
├── package.json       # Node.js dependencies and scripts
├── todos.db          # SQLite database (created automatically)
├── public/
│   └── index.html    # Frontend HTML/CSS/JavaScript
└── README.md         # This file
```

## Database Schema

The SQLite database contains a single `todos` table with the following structure:

- `id` - Primary key (auto-increment)
- `title` - Todo title (required)
- `description` - Todo description (optional)
- `completed` - Boolean flag for completion status
- `created_at` - Timestamp when todo was created
- `updated_at` - Timestamp when todo was last updated

## Technologies Used

- **Backend**: Node.js, Express.js
- **Database**: SQLite3
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Styling**: Modern CSS with gradients and animations

## Development

To run in development mode:

```bash
npm run dev
```

The server will start on port 3000 by default. You can change this by setting the `PORT` environment variable.

## License

MIT
