# Greenlight Movie API

Greenlight is a JSON API for retrieving and managing information about movies. The API supports basic CRUD operations for movies and user management functionalities. The core functionality is similar to the Open Movie Database API.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Endpoints](#endpoints)

## Introduction

Greenlight is a JSON API built with Go, designed to handle movie information, user registration, authentication, and more. This project follows advanced patterns for building APIs and web applications in Go.

## Features

- Retrieve movie details
- Create, update, and delete movies
- User registration and activation
- User authentication and password management
- Structured logging and error handling
- Rate limiting
- Graceful shutdown
- Cross-origin requests (CORS)
- Metrics and monitoring

## Prerequisites

- Go 1.17 or later
- PostgreSQL

## Endpoints

1. **Health Check**
    - GET /v1/healthcheck: Show application health and version information.

2. **Movies**
    - GET /v1/movies: Show details of all movies.
    - POST /v1/movies: Create a new movie.
    - GET /v1/movies/:id: Show details of a specific movie.
    - PATCH /v1/movies/:id: Update details of a specific movie.
    - DELETE /v1/movies/:id: Delete a specific movie.

3. **Users**
    - POST /v1/users: Register a new user.
    - PUT /v1/users/activated: Activate a specific user.
    - PUT /v1/users/password: Update the password for a specific user.

4. **Tokens**
    - POST /v1/tokens/authentication: Generate a new authentication token.
    - POST /v1/tokens/password-reset: Generate a new password-reset token.

5. **Metrics**
    - GET /debug/vars: Display application metrics.
