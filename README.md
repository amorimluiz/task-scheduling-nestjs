# Task Scheduling with NestJS

## Project Overview

Task Scheduling with NestJS is a project designed to manage and schedule tasks efficiently. Built with NestJS, a progressive Node.js framework, this application provides a robust backend to handle task creation, updates, and management, leveraging modern development practices and tools.

## Technologies Used

- **NestJS**: A framework for building efficient, reliable, and scalable server-side applications using TypeScript.
- **Node.js**: JavaScript runtime for server-side programming.
- **MySQL**: Relational database for storing application data.
- **Docker**: Containerization platform for consistent development and deployment environments.
- **Adminer**: A lightweight database management tool for MySQL.

## Getting Started

### Prerequisites

- Docker and Docker Compose installed on your machine.
- `.env` file configured with necessary environment variables.

### Configuration

Create a `.env` file in the root directory of the project with the following content:

```env
APP_PORT=

DB_PASSWORD=""
DB_NAME=""
DB_PORT=

ADMINER_PORT=
```

### Running the Project with Docker

1. **Build Containers**

   To build the Docker images for the application, run:

   ```sh
   docker-compose build
   ```

2. **Run Containers**

   To start the application along with MySQL and Adminer, run:

   ```sh
   docker-compose up
   ```

3. **Accessing the Application**

   - **Application**: Open your browser and go to `http://localhost:3000` (or the port specified in your `.env` file).
   - **Adminer**: Open your browser and go to `http://localhost:8080` (or the port specified in your `.env` file) to manage the MySQL database.

### Development

For local development, you can edit the source files in the `src` directory. Docker volumes are set up to sync changes automatically, so you can see updates without rebuilding the containers.

### Running Tests

To run tests locally, execute:

```sh
npm test
```

### Linting

To ensure code quality and consistency, run:

```sh
npm run lint:fix
```

### License

This project is licensed under the [MIT License](LICENSE).
