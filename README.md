**To-Do List App**
This is a simple To-Do List web application built with Node.js and PostgreSQL, where users can add, edit, and delete tasks. The app uses Express as the web framework, EJS for templating, and integrates PostgreSQL as the database.

**Features**
Add New Tasks: Easily add tasks to the list with the add button.
Edit Tasks: Update tasks on the list by providing the new content.
Delete Tasks: Remove tasks from the list to keep it organized.
Persistent Storage: All tasks are stored in a PostgreSQL database to maintain data across sessions.
User-Friendly Interface: Simple and intuitive UI with dynamic rendering using EJS.


**Installation**
_Clone the repository:_
bash

git clone https://github.com/your-username/todo-list-app.git
cd todo-list-app


**Install dependencies:**

bash
Copy code
npm install


**Set up PostgreSQL database:**

Create a PostgreSQL database named permalist, then create an items table with the following schema:

sql
Copy code
CREATE TABLE items (
  id SERIAL PRIMARY KEY,
  title VARCHAR(255) NOT NULL
);


_Configure the database connection:_ Update your database credentials in app.js as needed.

**Start the server:**

bash
Copy code
node app.js


_Access the app:_ Open your browser and go to http://localhost:3000 to view and use the To-Do List app.

**Usage**
The main functionalities of the app include:

_Add Tasks_: Enter a task in the input field and submit to add it to the list.
_Edit Tasks_: Update any task in the list by editing the text and saving.
_Delete Tasks_: Click the delete button next to a task to remove it from the list.
All operations are handled dynamically with Express and EJS, and the data is managed in PostgreSQL.


**Code Overview**
The primary components of the app include:

_Express_: Manages the server, routing, and static file serving.
_Body-Parser_: Parses incoming request bodies, making it easier to access form data.
_(pg module)_: Provides the database connection and data management.
_EJS_: Renders the frontend dynamically with embedded JavaScript.
