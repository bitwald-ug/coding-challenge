# bitwald Coding Challenge

## Context

##### Imagine you're working as a programmer for bitwald. The data team has just created an advanced model for flagging suspicious transactions. This model is still in the early stages, so they want to pass the transactions on for manual review. The challenge is to create a small full stack application for the fraud team that consists of a server and a web based UI in order to manage reported transactions.

## Requirements

### 1. Backend (Node.js + TypeScript)
- Create a Node.js server that serves as the backend for the application.
- Use Express.js to set up your server.

Implement the following REST-Endpoints
- GET /transactions: Retrieve a list of suspicious transactions including the comments, ordered from newest to oldest.
- POST /transactions/:id/flag: Flag a transaction as suspicious.
- POST /transactions/:id/allow: Allow a transaction.
- POST /transactions/:id/comment: Comment on a transaction.

Use a local, text-based datastore to store and update transaction data. Ensure that flagged, allowed, and commented transactions are persisted between server restarts.

### 2. Frontend (React)
- Create a React-based web application for the fraud team to manage reported transactions.
- Build a dashboard that displays a list of suspicious transactions, ordered from newest to oldest.
- Each transaction in the list should show its details, including the transaction amount, description, comments and date
- Provide buttons to allow, flag, and comment on transactions. Clicking on these buttons should send the respective API requests to the backend.
- Implement a transaction detail view that displays additional information about the selected transaction, including any comments made by users.
- Add a comment section to the transaction detail view, allowing users to leave comments about the transaction.
- Ensure that the user's actions, such as flagging, allowing, and commenting, are immediately reflected in the UI without requiring a page refresh.
- The web application should be 100% responsive (smartphone, tablets etc.)

### 3. Bonus Points
- Use TypeScript for both the frontend and backend.
- Add pagination to the list of transactions, allowing the user to load more transactions as needed.
- Dockerize your application for easy deployment.
- Write unit tests for critical parts of your application.

### Submission
Please provide the source code of your solution in a private code repository (e.g., GitHub, GitLab) and share access with us. Include clear instructions in a README.md on how to run your application locally.

### What we're looking for

1. High code quality (you should favor quality over quantity)
2. Develop with regard to clean code principles
2. Pragmatic technical choices
3. A runnable full-stack application with clear instructions how to run it
