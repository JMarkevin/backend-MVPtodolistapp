# TodoList Backend API

A RESTful API for managing todo items, built with Express.js and TypeScript.

## Features

- ✅ CRUD operations for todos
- 📝 Swagger API documentation
- 🔒 API key authentication
- 🌐 CORS enabled for frontend integration
- 📊 Health check endpoint
- 🚀 Production ready

## API Endpoints

### Todos

- `GET /todos` - Get all todos (with pagination and filtering)
- `POST /todos` - Create a new todo
- `PUT /todos/:id` - Update a todo
- `DELETE /todos/:id` - Delete a todo

### Health Check

- `GET /health` - API health status

### Documentation

- `GET /api-docs` - Swagger UI documentation

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository

```bash
git clone <repository-url>
cd todolist-backend
```

2. Install dependencies

```bash
npm install
```

3. Create environment file

```bash
cp .env.example .env.local
```

4. Update environment variables in `.env.local`

### Development

```bash
npm run dev
```

The server will start on `http://localhost:8080`

### Production

```bash
npm run build
npm start
```

## Environment Variables

| Variable       | Description            | Default                 |
| -------------- | ---------------------- | ----------------------- |
| `NODE_ENV`     | Environment mode       | `development`           |
| `PORT`         | Server port            | `8080`                  |
| `API_KEY`      | API authentication key | Required                |
| `FRONTEND_URL` | Frontend URL for CORS  | `http://localhost:5173` |

## API Documentation

Once the server is running, visit `http://localhost:8080/api-docs` to view the interactive Swagger documentation.

## Deployment

This application is configured for deployment on Render. The `render.yaml` file contains the deployment configuration.

### Render Deployment Steps

1. Connect your GitHub repository to Render
2. Render will automatically detect the `render.yaml` configuration
3. Set the environment variables in Render dashboard
4. Deploy!

## License

ISC
