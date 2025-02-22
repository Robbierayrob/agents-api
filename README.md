# Flask Server Setup Guide

## Prerequisites
- Python 3.7 or higher
- pip package manager

## Installation

1. Clone the repository:
```bash
git clone https://github.com/your-repo/agents-api.git
cd agents-api
```

2. Create and activate a virtual environment (recommended):
```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Running the Server

1. Set up environment variables (if needed) in a `.env` file:
```bash
# Example .env file
FLASK_APP=app.py
FLASK_ENV=development
```

2. Run the server:
```bash
flask run
```

3. The server will be available at:
```
http://localhost:5000
```

## API Endpoints

- `POST /chat` - Main chat endpoint
- `GET /static/images/<filename>` - Serves static images
- `GET /` - Serves the main HTML page

## Notes
- The server uses port 5000 by default
- Debug mode is enabled in development
- Static images are served from the `static/images` directory
