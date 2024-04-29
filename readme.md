# Message Board App

Welcome to the Message Board App! This is a simple yet powerful application built on Django, allowing users to post and read short messages on a message board. With the built-in SQLite database and Django's admin interface, managing your message board has never been easier.

## Features

- **User Authentication:** Users can sign up, log in, and log out securely.
- **Post Messages:** Registered users can post short messages to the message board.
- **Read Messages:** Users can browse and read messages posted by other users.
- **Admin Interface:** Easily manage users and messages through Django's built-in admin interface.

## Database Model

The database model for the Message Board App consists of two main entities:

1. **User:** Represents a registered user of the application.
   - Fields:
     - Username
     - Email
     - Password

2. **Message:** Represents a short message posted by a user.
   - Fields:
     - Author (Foreign key to User)
     - Content
     - Timestamp

## Setup Instructions

To set up the Message Board App locally, follow these steps:

1. Clone the repository:


2. Navigate to the project directory:


3. Create a virtual environment:


4. Activate the virtual environment:

- On Windows:

  ```
  .\env\Scripts\activate
  ```

- On macOS and Linux:

  ```
  source env/bin/activate
  ```

5. Install dependencies:


6. Run migrations to create the database:


7. Create a superuser to access the admin interface:


8. Start the development server:


9. Access the admin interface at `http://127.0.0.1:8000/admin/` and log in with the superuser credentials created in step 7.

10. You're ready to use the Message Board App! Visit `http://127.0.0.1:8000/` to start posting and reading messages.

## Technologies Used

- Django: A high-level Python web framework for rapid development and clean, pragmatic design.
- SQLite: A lightweight, serverless, relational database management system.
- HTML/CSS: For the front-end structure and styling.