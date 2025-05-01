# Airbnb CLONE PROJECT

## Project Overview

### 🛫 Project Objectives

The _Airbnb Clone Project_ is a comprehensive, real-world application designed to simulate the development of a robust booking platform like Airbnb.
It involves a deep dive into full-stack development, focusing on backend systems, database design, API development, and application security.
This project enables learners to understand complex architectures, workflows, and collaborative team dynamics while building a scalable web application.

### 🏆 Project Goals
	- User Management - Implement a secure system for user registration, authentication, and profile management.
	- Property Management - Develop features for property listing creation, updates, and retrieval.
	- Booking System - Create a booking mechanism for users to reserve properties and manage booking details.
	- Payment Processing - Integrate a payment system to handle transactions and record payment details.
	- Review System - Allow users to leave reviews and ratings for properties.
	- Data Optimization - Ensure efficient data retrieval and storage through database optimizations.

## 👥 Team Roles
	1. Software Developer: Engineers and stabilizers the product - Backend and Frontend engineers.
	2. Database Administrator: Manages database design, indexing, and optimizations.
	3. DevOps Engineer: Handles deployment, monitoring, and scaling of the backend services.
	4. QA Engineer: Ensures the backend functionalities are thoroughly tested and meet quality standards.
	5. Business Analyst: They translate an abstract product idea into a set of tangible requirements.
	6. Product Owner: Owns responsibility for product vision and evolution
	7. Product Manager: Ensures a product is delivered with the set time and budget
	8. UI/UX Designer: Transforms a product into a user friendly design
	9. Software Architecture: Develops the software architecture, select appropriate tools and platforms for implementation
	10. Quality Assurance Engineer: Ensures an application works according to requerements and sports the defects in the App
	11. Test Automation Engineer: Designs a test automation system

##   Project Tech Stack
        1. Django: A high-level Python web framework used for building the RESTful API.
        2. Django REST Framework: Provides tools for creating and managing RESTful APIs.
        3. PostgreSQL: A powerful relational database used for data storage.
        4. GraphQL: Allows for flexible and efficient querying of data.
        5. Celery: For handling asynchronous tasks such as sending notifications or processing payments.
        6. Redis: Used for caching and session management.
        7. Docker: Containerization tool for consistent development and deployment environments.
        8. CI/CD Pipelines: Automated pipelines for testing and deploying code changes.

## 🌵 Database Design

The key entities required for this project include:

- Users
  - Authentication: Authenticate and manage user profiles
  - Property: user having multiple properties
  - Bookings: user having multiple bookings in a single property
  - Payment: User payment to a single booking or property
  - Review: User's review of every bookings made

- Property
  - Bookings: All bookings in a single property
  - Payments: All the payments done a single booked property over a period of time
  - Reviews: All the review of the property

- Bookings
  - Payments: All the payments made for the booking
  - Reviews: All the reviews done for the booking

- Payments: All the payments made.

- Reviews: All the reviews made

## 🪶 Feature Breakdown

- User Management: Register new user, authenticate and manage user's profile

- Property Management: Create, update, retrieve, delete property listings

- Booking Systems: Make, update, and manage bookings including check-ins and check-outs details

- Payment Processing: Handle payment trasactions related to booking

- Review Systems: Post and manage reviews for properties

- Database Optimization
   - Indexing: Implement indexing for faster retrivals of frequently accesed data
   - Cache: Use caching stategies to reduce database load and improve perfomance

- API Documentation
   - OpenAPI Standards: The backend APIs are documented using OpenAPI to ensure clarity and ease of intergration
   - Django REST Framework: Provides a RESTful API for handling CRUD operations on users and property data
   - GraphQL: Offers a flexible and efficient query mechanism to interact with backend

## 🔐 API Security
The security measures that will be implemented includes

- Authentication - Verify the identity of the user or system trying to access the API
    - For registration of new users
    - Ensures access to the required user
    - Managing user profiles

- Authorization - Granting or denying access to resources based on users roles or scopes after authentication
    - User has access to certain properties or bookings
    - User has access to his browsing history

- Rate limit - Controlling the number of API requests a user or client can make within a certain period of time
    - Prevents abuse or Denial of Service (DoS) attacks
    - Ensures fair usage among clients.

- Data Encrypription - Encrypt sensitive data at rest and at transit
    - Protect payment details

- Input Validation - Prevents injection attacks (SQL, commands etc)

- HTTPS - Ensure TSL is used for data in transit.

## 🪈 CI/CD Pipeline
CI/CD pipelines (Continuous Integration and Continuous Deployment/Delivery) are automated workflows used to build, test, and deploy code changes in software projects.

 - Continuos Integration
   Automatically integrates code changes from multiple developers into a shared repository several times a day.
     - Runs automated tests
     - Bulds the project
     - Catches bugs up early
     - Ensures code quality

 - Continous Development
   Automatically deploys tested code to production (Deployment) or staging (Delivery).
     - Reduces deployment risks
     - Ensures faster delivery of features
     - Improves team productivity

The following are the importance of CI/CD Pipeline
 1. Faster feedback loop for developers.
 2. Improved code quality through automated testing.
 3. Reliable deployments with minimal human error.
 4. Streamlined collaboration in teams.

The most commont tools used in this pipeline includes:
 1. Github Actions
 2. GitLab CI
 3. Jenkins
 4. Docker 
