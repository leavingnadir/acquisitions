## ⚙️Tech Stack

This project uses a modern, production-ready stack including Node.js and Express.js for backend development, Neon PostgreSQL with Drizzle ORM for database management, and Zod for runtime data validation. Security is enhanced with Arcjet, while Docker and Kubernetes enable containerization and scalable deployments. Developer productivity is supported through tools like Warp Terminal, ESLint, Prettier, and Jest.

## 🔋 Features

- JWT-based authentication and role-based access control
- Business listings and deal management system
- PostgreSQL database with migrations using Drizzle ORM
- Input validation using Zod
- API protection with Arcjet
- Structured logging with Winston
- Health monitoring endpoint
- Dockerized development and production environments
- Hot reload for faster development
- Automated testing with Jest and Supertest
- Clean code architecture with absolute imports

## 🚀 Production API Setup Guide

This guide helps you clone the repository, install dependencies, and set up the database for your production-ready API project.

## 📦 Install Required Dependencies

1️⃣ Core Server & Environment Setup

- express → Web framework for building APIs
- dotenv → Loads environment variables from .env file

```
npm install express dotenv
```

2️⃣ Code Quality & Formatting Tools (Development Only)

- eslint → Finds and fixes code issues
- prettier → Formats your code automatically
- eslint-config-prettier → Prevents ESLint and Prettier conflicts
- eslint-plugin-prettier → Runs Prettier inside ESLint
- -D → Installs as development dependency

```
npm install eslint @eslint/js prettier eslint-config-prettier eslint-plugin-prettier -D
```

3️⃣ Database ORM & Serverless Support

- @neondatabase/serverless → Connects to Neon PostgreSQL serverless database
- drizzle-orm → Type-safe ORM for database operations

```
npm install @neondatabase/serverless drizzle-orm
```

4️⃣ Database Migration Tool (Dev Only)

- drizzle-kit → CLI tool for generating and running database migrations

```
npm install -D drizzle-kit
```

5️⃣ Generate Database Schema

Generates migration files based on your Drizzle ORM schema

```
npm run db:generate
```

6️⃣ Apply Database Migrations

```
npm run db:migrate
```

7️⃣ Logging & Security Middleware

- winston → Advanced logging system
- helmet → Adds security headers to protect your API
- morgan → HTTP request logger for debugging and monitoring

```
npm i winston
```

```
npm i helmet
```

```
npm install morgan
```

```
npm install cors cookie-parser
```

8️⃣ Authentication & Validation

- jsonwebtoken → Creates and verifies JWT tokens
- bcrypt → Hashes passwords securely
- zod → Schema validation for inputs and responses

```
npm i jsonwebtoken
```

```
npm install zod
```

```
npm install bcrypt
```

9️⃣ API Protection & Security Monitoring

- @arcjet/node → API protection, rate limiting, and abuse detection
- @arcjet/inspect → Debug and inspect Arcjet decisions

```
npm i @arcjet/node @arcjet/inspect
```

🔟 Testing Setup (Development Only)

- Jest → JavaScript testing framework
- Supertest → HTTP assertions for API testing
- cross-env → Cross-platform environment variable support (Windows/macOS/Linux)

```
npm install --save-dev jest
```

```
npm install -D cross-env
```

```
npm install supertest --save-dev
```

```
npm init jest@latest
```
