# Exam Management System

## Overview
This project is an **Exam Management System** built using **Flask** for web application development, **Celery** for background task processing, and **Redis** as the message broker. The system allows **admins** to create exams by uploading files (PDF, PPTX, MD), while **students** can take exams and view their results. The project utilizes the **OpenAI API** to generate multiple-choice questions from the uploaded files and store them in an **SQLite database**.

## Features
- **Admin Panel**: Admins can create exams by uploading files, which are processed in the background using Celery and Redis.
- **File Processing**: Supports **PDF**, **PPTX**, and **Markdown** files for extracting exam content.
- **Question Generation**: Uses the **OpenAI API** to generate questions and store them in the database.
- **Student Portal**: Students can take exams and view their scores.
- **Role-Based Authentication**: Separate login systems for **admins** and **students** with role-based access control.
- **SQLite Database**: Stores exam data, questions, student records, and results.
- **Asynchronous Processing**: Tasks like file parsing and question generation are handled asynchronously to enhance performance.

## Technologies Used
- **Flask**: Web framework for building the web app.
- **Celery**: Task queue for background processing.
- **Redis**: Message broker for Celery tasks.
- **SQLite**: Database to manage exam-related data.
- **OpenAI API**: To generate multiple-choice questions from file content.
- **Bootstrap**: For responsive front-end design.

## Setup and Installation

1. Clone the repository using `git clone https://github.com/yourusername/exam-management-system.git`.
2. Install the required packages by running `pip install -r requirements.txt`.
3. Start the Redis server with `redis-server`.
4. Run the Celery worker by executing `celery -A celery_config.celery worker --loglevel=info`.
5. Finally, start the Flask application by running `flask run`.

## Outcomes
- Improved skills in asynchronous processing with **Celery** and **Redis**.
- Gained experience integrating **OpenAI API** for question generation.
- Enhanced understanding of full-stack development with **Flask** and **Bootstrap**.
- Implemented role-based authentication and database design with **SQLite**.
