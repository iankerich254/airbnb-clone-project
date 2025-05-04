This is the AirBnB Clone project.

## Team Roles

Software Developer - codes an application.
Software Architect - designs a high-level software architecture and makes executive software design decisions on behalf of an app development team.
UI/UX Designer - transforms a product vision into user-friendly designs.
Project Manager - makes sure a product or its part is delivered on time and within budget.
Product Owner - is responsible for a product vision and evolution.
Business Analyst - translates an abstract product idea into a set of tangible requirements.
Quality Assurance Engineer - verifies whether an application meets the requirements.
Test automation engineer - designs a test automation ecosystem, writes and maintains test scripts for automated testing.
Devops Engineer - facilitates cooperation between development and operation teams and builds continuous integration and continuous delivery (CI/CD) pipelines for faster delivery.

## Technology Stack

Django: A high-level Python web framework used for building the RESTful API.
Django REST Framework: Provides tools for creating and managing RESTful APIs.
PostgreSQL: A powerful relational database used for data storage.
GraphQL: Allows for flexible and efficient querying of data.
Celery: For handling asynchronous tasks such as sending notifications or processing payments.
Redis: Used for caching and session management.
Docker: Containerization tool for consistent development and deployment environments.
CI/CD Pipelines: Automated pipelines for testing and deploying code changes.

## Database Design

Entities and Key Fields

Users: id, name, email, password, role
Properties: id, host_id, title, description, location 
Bookings: id, guest_id, property_id, check_in, check_out 
Reviews: id, booking_id, rating, comment, created_at 
Payments: id, booking_id, amount, status, paid_at 
