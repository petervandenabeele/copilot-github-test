# Mergington High School Activities

A comprehensive web application built with FastAPI and MongoDB that allows students to view and sign up for extracurricular activities, with teacher authentication and management features.

## Tech Stack

- **Backend**: FastAPI (Python web framework)
- **Database**: MongoDB for data storage
- **Frontend**: Static HTML, CSS, and JavaScript
- **Authentication**: Secure password hashing with Argon2
- **Server**: Uvicorn ASGI server

## Features

### Student Features
- View all available extracurricular activities
- Sign up for activities with participant limits
- Filter activities by day of the week
- Filter activities by time (start/end times)
- View detailed activity information (description, schedule, max participants)

### Teacher Features  
- Secure login system with hashed passwords
- Teacher authentication and session management
- Activity management capabilities

### System Features
- RESTful API endpoints for activities and authentication
- Real-time activity filtering and search
- Responsive web interface
- Database initialization with sample data
- Static file serving for frontend assets

## Setup and Installation

### Prerequisites
- Python 3.7+
- MongoDB server running on localhost:27017
- pip package manager

### Installation Steps

1. **Install Python dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Start MongoDB server:**
   Make sure MongoDB is running on `mongodb://localhost:27017/`

3. **Run the application:**
   ```bash
   uvicorn app:app --reload
   ```

4. **Access the application:**
   Open your browser to `http://localhost:8000`

### Database Setup
The application automatically initializes the MongoDB database with sample activities and teacher accounts on first run.

## API Endpoints

- `GET /` - Redirects to the main application
- `GET /activities/` - Get all activities (with optional filtering)
- `POST /auth/login` - Teacher login
- `GET /static/` - Static file serving

## Development Guide

For detailed setup and development instructions, please refer to our [Development Guide](../docs/how-to-develop.md).
