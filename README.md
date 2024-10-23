## Planner Application

The Planner Application is a full-stack task management system designed to enhance productivity through an intuitive user interface and robust backend service. It includes a frontend built with Next.js for dynamic task management and a backend powered by NestJS for secure user authentication and efficient task handling. The application utilizes PostgreSQL for data storage and implements features like task categorization, Pomodoro timer, drag-and-drop scheduling, and much more.

---

## Features

### User Authentication (Backend)

- Secure login and registration using JSON Web Tokens (JWT).

### Task Management

- Create, Read, Update, Delete (CRUD) tasks.

- List view and Kanban view for task organization.

- Categorize and prioritize tasks.

### Time Blocks and Scheduling

- Dynamic task sizing for better visual clarity based on duration.

- Drag-and-drop functionality for easy task rearrangement.

- Task management through list or Kanban views with interactive updates.

### Pomodoro Timer

- Customizable work and break sessions for enhanced focus.

- Simple user interface for managing Pomodoro cycles.

---

## Technology Stack

### Backend

- **[NestJS](https://docs.nestjs.com/)**: A progressive Node.js framework for building efficient server-side applications.

- **[TypeScript](https://www.typescriptlang.org/docs/)**: A strongly typed programming language that builds on JavaScript.

- **[Prisma](https://www.prisma.io/docs/getting-started)**: Next-generation ORM for Node.js and TypeScript.

- **[PostgreSQL](https://www.postgresql.org/docs/)**: An advanced open-source relational database.

- **[NestJS JWT](https://docs.nestjs.com/security/authentication)**: An open standard for secure data transmission.

### Frontend

- **[Next.js](https://nextjs.org/docs)**: Next.js is a powerful web development framework that simplifies the process of building fast, interactive applications.

- **[TypeScript](https://www.typescriptlang.org/docs/)**: A strongly typed programming language that builds on JavaScript.

- **[TanStack React Query](https://tanstack.com/query/v5/docs/react/overview)**: A powerful data-fetching and state management library for managing server-state in React applications, improving performance and developer experience.

- **[React Hook Form](https://react-hook-form.com/get-started)**: A library for building and managing forms, providing easy validation and high-performance handling of form inputs.

- **[Tailwind CSS](https://tailwindcss.com/docs/installation)**: A utility-first CSS framework for rapidly building custom, responsive designs with minimal effort.

---

## Prerequisites

Before you begin, ensure you have the following installed:

- Node.js (v14 or higher)
- npm or yarn
- PostgreSQL: v12 or higher

---

## Installation and Setup

### Backend

1. Clone the backend repository

```bash
   git clone https://github.com/vitalii-hrymalyuk/planner-backend.git
```

2. Navigate to the project directory

```bash
   cd planner-backend
```

3. Install dependencies:

```bash
   # Using npm
   npm install

   # Or using yarn
   yarn install
```

4. Create an .env file in root folder
5. Set up environment variables by adding the following to your `.env` file:

   ```env
   DATABASE_URL="postgresql://USER:PASSWORD@HOST:PORT/DATABASE"
   JWT_SECRET="your_jwt_secret"

   ```

6. Run database migrations:

```bash
   npx prisma migrate dev --name init
```

7. Start the backend server:

```bash
   npm run start:dev
```

The backend server will be running at http://localhost:4200.

### Frontend

1. Clone the frontend repository

```bash
   git clone https://github.com/vitalii-hrymalyuk/planner-frontend.git
```

2. Navigate to the project directory

```bash
   cd planner-frontend
```

3. Install dependencies:

```bash
   # Using npm
   npm install

   # Or using yarn
   yarn install
```

4. Start the frontend development server:

```bash
   npm run dev

```

The frontend will be accessible at http://localhost:3000.

---

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

---

## License

This project is licensed under the MIT License.

---

## Contact Information

- **Author**: Vitalii Hrymalyuk
- **Email**: [vitalii.hrymalyuk@gmail.com](mailto:vitalii.hrymalyuk@gmail.com)

Feel free to reach out if you have any questions or need assistance setting up the project.
