# Django Project Template
![Cover Image](/assets/cover.png)
This is a template for a Django project that uses Docker Compose, a Makefile for task automation, and PostgreSQL as the
database.

## Requirements

Before using this project, make sure you have the following components installed:

- Docker
- Docker Compose
- GNU Make

## Setup

1. Clone this repository to your computer.
2. Create a `.env` file based on `.env.example` and specify the necessary environment variables.

## Running the Project

1. Open a terminal and navigate to the project's root directory.
2. Use the command `make app` to build Docker containers and start the project.
3. Open your browser and go to `http://localhost:8000/` to view the project.

## Implemented Commands

- `make app`: Start the project.
- `make app-logs`: Follow the logs in app container.
- `make app-down`: Stop application and all infrastructure.
- `make storages`: Up only storages. you should run your application locally for debugging/developing purposes
- `make storages-logs`: Follow the logs in storages containers
- `make storages-down`: Stop all infrastructure

## Most Used Django Specific Commands

- `make migrate`: Apply Django migrations to the database.
- `make migrations`: To create database migration files based on the changes you've made to your models.
- `make superuser`: Create a Django superuser.
- `make collectstatic`: To collect all necessary static files for your project.

## Making Changes

1. Make necessary changes to the Django source code as needed.
2. Run `make migrate` and `make migrations` after making changes to Django models to update the database schema.

## License

This project is distributed under the MIT License. See the `LICENSE` file for additional information.