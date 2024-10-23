# Django Project: Simple Social Media App

A social media web application built with Django that allows users to create accounts, join groups, and post content and many more. This project demonstrates the implementation of user authentication, groups, post features and many more. It is a cloned project from a Django bootcamp 

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Usage](#usage)

## Project Overview
SimpleSocial is a social media platform built using Django, where users can:
- Register and log in to their accounts.
- Join or leave different groups.
- Post updates that are visible to group members.
- View posts made by other users in the groups they belong to.

## Features
- User authentication (registration, login, logout).
- Group management (create, join, leave).
- Posting content to groups.
- Responsive design with Bootstrap integration.
- Debug toolbar for development assistance.

## Technologies Used
- **Django**: High-level Python web framework.
- **SQLite**: Default database for development.
- **Bootstrap**: Frontend framework for responsive design.
- **Python-decouple**: For managing environment variables.

## Installation

### Prerequisites
Ensure you have the following installed on your machine:
- Python 3.8+
- Django 3.2+
- Git

### Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Waris10/social-media-app.git
   cd simplesocial
   ```

2. **Set up a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables:**
   Create a `.env` file in the root directory and add the following (customize as needed):

   ```bash
   SECRET_KEY=your-secret-key
   DEBUG=True
   ALLOWED_HOSTS=localhost,127.0.0.1
   ```

5. **Apply the database migrations:**
   ```bash
   python manage.py migrate
   ```

6. **Create a superuser for the admin panel:**
   ```bash
   python manage.py createsuperuser
   ```

7. **Run the development server:**
   ```bash
   python manage.py runserver
   ```

8. **Access the app:**
   Open your browser and go to `http://127.0.0.1:8000`.

## Environment Variables

Ensure you have the following environment variables configured in a `.env` file:
- `SECRET_KEY`: Your Django secret key.
- `DEBUG`: Set to `True` for development and `False` for production.
- `ALLOWED_HOSTS`: List of allowed hosts (e.g., `localhost`, `127.0.0.1`).

## Usage
After starting the server, you can:
- Register a new account or log in if you already have one.
- Join existing groups or create new ones.
- Post content in the groups you're part of.
- View and manage your posts.
