# Classroom Management API

Welcome to the Classroom Management API documentation. This API is designed to provide functionality for managing assignments, students, and teachers in a classroom setting. It is built with Spring Boot and provides a range of features to support the educational process.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [API Endpoints](#api-endpoints)
- [Authentication](#authentication)
- [Features](#features)
- [Examples](#examples)

## Introduction

This application is made with Spring Boot and offers a classroom management system. It allows teachers to create, update, and delete assignments, grade submissions, and send notifications to students. Students can submit their responses to assignments. The API also includes features like email notifications, caching using Redis, and more.

- Hosted URL: [https://classroom-docker-pp.onrender.com/](https://classroom-docker-pp.onrender.com/)
- Docker Image: You can pull the Docker image using `docker pull rohitchouhan35/classroom`.

## Getting Started

To get started with this API, follow these initial steps:

1. Clone the project and open it in your preferred IDE (e.g., IntelliJ IDEA).
2. Install all the project dependencies.
3. In the `application.properties` file located in `classroom/src/main/resources/`, configure your database settings and other configurations. You can choose to use a remote MySQL database and a remote Redis server or configure them for local use.
4. Choose to run the API using either the hosted URL or a local URL. When using the hosted URL, be aware that the server may close the application after a period of inactivity, resulting in initial delay.
5. Sign up as a teacher or student to access the API. Choose your role during signup and use the generated access token for API authentication.

## API Endpoints

The API provides various endpoints for managing assignments and submissions, user management, and more. Here are some of the key endpoints:

1. **Signup**: Register as a user (teacher or student).
2. **Login**: Obtain a JWT token for authentication.
3. **Create Assignment**: Allows teachers to create new assignments.
4. **Update Assignment**: Allows teachers to update existing assignments.
5. **Delete Assignment**: Allows teachers to delete existing assignments by ID.
6. **Submit Assignment Answer**: Allows students to submit responses to assignments.
7. **Get All Assignments**: Fetch a list of all assignments.
8. **Student Who Submitted Assignment**: Allows teachers to see a list of students who have submitted a particular assignment.
9. **Get Assignment by ID**: Retrieve a single assignment by its ID.
10. **Student Report**: Allows teachers to view students' submissions.
11. **All Submissions**: Get a list of all student submissions.
12. **Grade Submission**: Allows teachers to grade students' submissions.
13. **Get User**: Get a list of all registered users.
14. **Save User**: Save a user to the database.

For detailed usage and examples of these endpoints, please refer to the [API Documentation](https://schema.getpostman.com/json/collection/v2.1.0/collection.json).

## Authentication

All API requests require authentication using a JWT token. To obtain a token, use the login endpoint with your username and password. Then, include the token in the `Bearer` authorization header of your requests.

## Features

- Automatic reminders to students for assignments with a due date within 2 days.
- User registration as teachers or students.
- User-based access control for all API endpoints.
- Teacher actions: create, update, delete, and grade assignments.
- Student actions: submit responses to assignments.
- Email notifications for new assignments and graded submissions.
- Caching using Redis to reduce API latency for some endpoints.
- MySQL database for data storage.
- Docker containerization support.

## Examples

Here are some examples of common API use cases:

- Creating a new assignment as a teacher.
- Updating an existing assignment as a teacher.
- Deleting an assignment as a teacher.
- Submitting a response to an assignment as a student.
- Viewing a list of all assignments.
- Viewing a list of students who submitted a specific assignment.
- Getting a single assignment by ID.
- Viewing students' submissions as a teacher.
- Viewing all student submissions.
- Grading a student's submission as a teacher.
- Fetching a list of all registered users.
- Saving a new user to the database.

---

Contact information: rohitchouhan3512@gmail.com
