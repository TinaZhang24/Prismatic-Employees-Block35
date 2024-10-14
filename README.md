# Prismatic Employees

You've done a great job building an employee-management API with placeholder data. Now you can be trusted to build the API with a real database!

## Prisma

In this first section, you'll be setting up the database with Prisma.

1. Create a new PostgreSQL database named `prismatic-employees`.
2. Initialize Prisma in this repo and connect it to that PostgreSQL database.
3. Define the `Employee` model in the schema with the following fields:
   - `id`: int, primary key, auto increment
   - `name`: string
4. Seed the database with 10 initial employees.

## Express

Now that your database is up and running, build an Express app that serves the following routes. Make sure to use the appropriate body-parsing and error-handling middleware!

- `GET /` sends the message "Welcome to the Prismatic Employees API."
- `GET /employees` sends array of all employees
- `POST /employees` adds a new employee with the provided name
  - Send 400 if name is not correctly provided
  - Send the newly created employee with status 201
- `GET /employees/:id` sends employee with specified ID
  - Send 404 if employee does not exist
- `PUT /employees/:id` updates employee with specified ID with provided data
  - Send 400 if name is not correctly provided
  - Send 404 if employee does not exist
  - Send the updated employee with status 200
- `DELETE /employees/:id` deletes employee with specified ID
  - Send 404 if employee does not exist
  - Send just the status 204

## Submission

Submit the link to your public GitHub repository.
