Planner App

## Getting Started

First, run the development server:

```bash
npm install
# then
npm run dev
# or
yarn dev
# or
pnpm dev
```

---

## About

The Planner App is designed to help you manage your time effectively. It offers features like timeblocking, task management with both list and Kanban board views, and a customizable Pomodoro timer to boost your productivity.

This is the basic functionality; let's look at each section in more detail.

---

## Features

### Time Blocks

Plan your day by scheduling tasks with full CRUD (Create, Read, Update, Delete) operations.
Dynamic Task Sizing: Task elements automatically adjust their size based on the duration of the task.
Drag and Drop: Easily rearrange your schedule by dragging and dropping tasks.

### Tasks Management

List and Kanban Views: View your tasks in either a traditional list or a Kanban board for better visualization.
Interactive Drag and Drop: Move tasks between different statuses or dates; the task's date updates automatically when moved.
Efficient Organization: Categorize and prioritize tasks to enhance productivity.

### Pomodoro Timer

Customizable Sessions: Set custom rounds and session lengths to fit your work style.
Productivity Booster: Utilize the Pomodoro Technique to maintain focus and manage breaks effectively.
User-Friendly Interface: Easy-to-use timer controls for starting, pausing, and resetting sessions.

---

## Technology Stack

The main infrastructure of the application is built using modern technologies for both frontend and backend development.

A complete list of the entire technology stack is given below:

## Backend

- **[NestJS](https://docs.nestjs.com/)**
- **[Prisma](https://www.prisma.io/docs/getting-started)**
- **[PostgreSQL](https://www.postgresql.org/docs/)**

# Frontend

- **[NextJS 14](https://nextjs.org/docs)**
- **[TanStack Query (React Query)](https://tanstack.com/query/v5/docs/react/overview)**
- **[React Hook Form](https://react-hook-form.com/get-started)**
- **[Tailwind CSS](https://tailwindcss.com/docs/installation)**

---

## ORM

Prisma is used as the ORM (Object-Relational Mapping) technology for database querying.

In conjunction with the VS Code extension, it allows you to conveniently compose models, generate a database object, and provides a convenient API for working with the database.

Prisma also provides a handy Prisma Studio (npx prisma studio) that allows direct interaction with the database and supports all CRUD operations.

## Database

A PostgreSQL database is used to store all the application information.

## Working with Data

The application works with data using React Query for efficient data fetching and caching, and React Hook Form for form state management and validation.

---

## Environment

The application infrastructure is built based on the requirements of the Next.js framework, utilizing the app directory introduced in Next.js 14 for routing and server components.

Navigation and working with backend endpoints are done through the folder and file structure.

app Directory: Contains all the routes and pages of the application. Each route is represented by a folder containing a page.tsx or page.js file.

Services Folder: For each feature, there is a file in services folder inside the frontend project. This structure facilitates easy interaction with the backend by organizing API calls and business logic related to each feature.

The hooks folder contains custom hooks to automate and simplify the interaction with libraries.

The components folder contains all the components of the application. Where possible, they have been divided into appropriate categories to summarize the functionality.

The UI components are styled using Tailwind CSS for rapid UI development.

---

## Working with Forms

Although the application is not large, it contains a few forms. During development, React Hook Form was used to simplify form state management and validation.

---

## State Management and Data Fetching

React Query: Manages server state, caching, and data synchronization.

React Hook Form: Simplifies form state management and validation.

---

## Styling

Tailwind CSS: A utility-first CSS framework for quickly building custom designs.

---

## Environment Variables

To run this project, you will need to add the following environment variables to your .env file:

```js
DATABASE_URL= /* URL for connection to database, ex: DATABASE_URL="postgresql://USER:PASSWORD@localhost:5432/DB_NAME?schema=public" */
JWT_SECRET = /* Token that is used authorization, ex:  JWT_SECRET="WoklJpTfu392VUqLIG0OyJpkaKrs7UB4" */

```

---

## Notes

The application is designed with scalability and maintainability in mind.
The use of the app directory in Next.js 14 enhances the routing capabilities and simplifies server component integration.
The inclusion of a services folder which contains files for each feature in the frontend project facilitates modular and organized interaction with the backend services.
