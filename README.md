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

## Feature Breakdown

User Management
Allows users to register, log in, and manage their profiles. Hosts and guests have role-specific dashboards to view and edit personal details, track listings or reservations, and update security settings.

Property Management
Enables hosts to create, edit, and remove listings with photos, descriptions, amenities, and pricing. Includes availability calendars and location mapping to ensure accurate booking information and attract guests.

Booking System
Lets guests search for properties by date, location, and filters, then reserve stays with real-time availability checks. Hosts receive booking requests for approval (if required), and both parties get notifications and booking summaries.

Reviews & Ratings
After a completed stay, guests can leave ratings and written feedback for properties; hosts can respond to reviews. Aggregated scores inform future guests and help maintain quality across the platform.

Payments & Transactions
Handles secure payment processing, supporting deposits, final balances, and refunds. Tracks transaction statuses and receipts, providing transparency and financial records for both guests and hosts.

Search & Filters
Offers keyword search and advanced filters (price range, property type, amenities, ratings) to help guests find suitable listings quickly. Integrates map view and sort options (e.g., price low-to-high) for intuitive discovery.

Notifications & Messaging
Facilitates in-app messaging between hosts and guests for inquiries and stay details. Sends automated email and push notifications for booking confirmations, reminders, and review prompts.

## API Security

Authentication (OAuth 2.0, JWT tokens): Ensures only verified users or services can access endpoints, preventing unauthorized entry 

Authorization (RBAC, scope checks): Enforces fine-grained permissions so authenticated clients can only perform allowed actions 

Rate Limiting & Throttling: Caps request rates per client to thwart brute-force attacks and denial-of-service attempts 

Encryption (TLS/HTTPS): Protects data in transit against eavesdropping and man-in-the-middle attacks 

Input Validation & Sanitization: Blocks injection attacks (e.g., SQL, script) by verifying and cleaning all incoming payloads 

### Why It Matters

Protecting User Data: Keeps personal and sensitive information safe from unauthorized access or leaks 

Securing Payments: Ensures transaction integrity and compliance with financial regulations by guarding payment endpoints 

Ensuring Availability: Maintains service uptime by mitigating abusive or malicious traffic patterns

## CI/CD Pipeline

A CI/CD pipeline automates the flow from code commits through building, testing, and deployment, reducing manual steps and ensuring consistent, reliable releases. It’s vital for our Airbnb-clone because it speeds up feedback loops, catches bugs early in development, and enables frequent, dependable feature rollouts. Common tools include GitHub Actions or GitLab CI for workflow orchestration, Docker for reproducible build environments, and Kubernetes or Terraform for deployment automation.
