**TextSpace — Cloud-Deployed Messaging Platform**
TextSpace is a full-stack messaging platform designed for simplified, intentional communication. It integrates Angular frontend components with a TypeScript-based Express backend, MongoDB Atlas database, Google SSO authentication, and Azure cloud deployment.

**Architecture Overview**

TextSpace follows a modular client–server architecture:
**Frontend:**
Angular application with modular components
Angular routing with parameterized routes
Angular service layer to consume REST APIs
**Backend:**
Node.js + Express (TypeScript)
RESTful API endpoints
Mongoose ODM for MongoDB interaction
Google OAuth 2.0 SSO integration
**Database:**
MongoDB Atlas (cloud-hosted NoSQL database)
**Mongoose models:**
User
Message
Group
Notification
**Authentication:**
Google OAuth 2.0 using Passport strategy
Secure session handling
**Cloud Deployment:**
Deployed to Microsoft Azure Web App
Deployment logs monitored for release validation
**Testing:**
Mocha-based API tests
Single Object endpoint test
List Object endpoint test
Tests target deployed host and route paths
**System Flow**
Angular Component → Angular Service → Express Route → Controller Logic → MongoDB Atlas → Response → Angular Render
**Authentication Flow:**
User → Google SSO → Backend Passport Strategy → Session Established → Protected Routes Access

**Key Engineering Features**
TypeScript-based backend for type safety
Modular model structure for scalability
SSO integration with external identity provider
Cloud-hosted database
Deployed production endpoint validation via Mocha
Parameterized routes in Angular
REST API contract testing
**Project Structure (Backend)**
**src/**
Server.ts
dbConnect.ts
**models/**
User.ts
Message.ts
Group.ts
Notification.ts
**sso/**
GooglePassport.ts
googleOAuth2.ts
**createDB/**
**What This Project Demonstrates**

Full-stack integration (Angular + Express)
Secure authentication boundary design
Cloud database integration
Production deployment workflow (Azure)
API contract testing
System modularity and separation of concerns
