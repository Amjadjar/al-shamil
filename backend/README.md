# Backend API for الشامل

FastAPI backend server providing REST API endpoints for the mobile application.

## Features

- Chat messaging
- Emergency tips and guidance
- Dashboard statistics
- Feature management
- CORS enabled for mobile clients

## Installation

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## Running the Server

```bash
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

The API will be available at: http://localhost:8000

Swagger UI documentation: http://localhost:8000/docs

## API Endpoints

### Health Check
- `GET /health` - Check if server is running
- `GET /` - Root endpoint

### Dashboard
- `GET /dashboard` - Get application statistics

### Chat
- `POST /chat` - Send chat message and receive reply

### Emergency
- `GET /emergency/{topic}` - Get emergency tips for a topic

### Features
- `GET /features` - List all available features
