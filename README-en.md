# Sunsky-SQL Judge System

## Overview

The SQL Judge System is an interactive online platform designed to enhance the learning and practice of SQL through a variety of exercises and challenges. It enables users to submit SQL queries, execute them in a secure environment, and receive immediate feedback on their solutions. The system supports multiple question types, including fill-in-the-blank and practical scenario-based questions.

## Key Features

- **User Authentication**: Secure user registration, login, and permission management to ensure data security and isolation.
- **Question Management**: Ability to create, store, edit, and delete questions, including question types (fill-in-the-blank, practical) and content.
- **Practice and Answering**: Users can practice SQL statements online, submit answers, and receive feedback.
- **Question Submission**: Users can submit new SQL questions, including question name, description, example code, and judging requirements.
- **Judging Engine**: Core functionality to parse and execute SQL statements and verify results based on question requirements.
- **Frontend Interface**: User-friendly interface for question display, answering, and new question submission.
- **Database Design**: Design of database models to store user information, question information, and question results.
- **Security**: Ensure the security of the SQL execution environment to prevent SQL injection and other security threats.
- **Feedback Mechanism**: Provide detailed feedback to help users understand mistakes and improve.

## Technical Stack

- **Backend**: Python with the Flask framework for API development.
- **ORM**: SQLAlchemy for database interactions and dynamic model generation.
- **Frontend**: HTML, CSS, JavaScript, and optionally React or Vue.js for a dynamic user interface.
- **SQL Editor**: Ace Editor for a feature-rich SQL coding experience.
- **Authentication**: Flask-Login for handling user sessions.
- **Form Handling**: Flask-WTF for form validation and handling.
- **Admin Interface**: Flask-Admin for database CRUD operations.
- **Security**: Flask-Sandbox for secure SQL statement execution.
- **Asynchronous Tasks**: Celery for handling background tasks (optional).
- **Database**: PostgreSQL, MySQL, or SQLite.
- **Deployment**: Docker for containerization and ensuring environment consistency.

## Directory Structure

```plaintext
sql-judge-system/
│
├── api/                 # API interface files
│   ├── __init__.py
│   ├── routes.py        # Route definitions
│   └── models.py        # Data model definitions
│
├── core/                 # Core logic files
│   ├── __init__.py
│   ├── executor.py      # SQL statement executor
│   ├── parser.py        # SQL statement parser
│   └── comparator.py    # Result comparator
│
├── utils/                # Utility files
│   ├── __init__.py
│   ├── database.py      # Database connection utilities
│   └── security.py      # Security utilities
│
├── templates/            # Frontend template files (if using)
│   ├── index.html
│   └── ...
│
├── static/               # Frontend static files (if using)
│   ├── css/
│   ├── js/
│   └── ...
│
├── config/               # Configuration files
│   ├── config.py        # Configuration class
│   └── secrets.py       # Sensitive information configuration
│
├── main.py                # Project entry file
├── requirements.txt      # Python dependency packages
└── README.md             # Project documentation
```

## Getting Started

To get started with the SQL Judge System, follow these steps:

1. **Environment Setup**: Set up a Python environment and install the required packages using `pip install -r requirements.txt`.
2. **Database Configuration**: Configure the database connection in the `config.py` file.
3. **Running the System**: Run the Flask application using `python main.py`.
4. **Accessing the Interface**: Access the user interface through the browser at the specified host and port.

## Contribution

For contribution guidelines and details on how to set up the development environment, please refer to the [Contribution Guidelines](https://github.com/your-username/sql-judge-system/blob/main/CONTRIBUTING.md).

## License

The SQL Judge System is open-source software licensed under the [MIT License](https://opensource.org/licenses/MIT).

---