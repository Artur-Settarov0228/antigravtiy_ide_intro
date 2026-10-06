# Smart Home Backend API 🏠

This project is a backend API designed to manage a **Smart Home** system. It allows controlling smart home devices such as lights, temperature, door locks, and other IoT devices.

---

## 🛠 Tech Stack
The project uses the following modern and fast libraries:
- **FastAPI** — Main framework for building the API (extremely fast and convenient).
- **Uvicorn** — Lightning-fast ASGI server to run the FastAPI application.
- **SQLAlchemy** — Object Relational Mapper (ORM) for database interactions.
- **Pydantic** — Data validation and settings management using Python type hints.
- **Python-dotenv** — Reads key-value pairs from a `.env` file for secret configurations.

---

## 📁 Project Layout
```text
smart_home_api/
├── src/                  # Main source code
│   ├── main.py           # Application entry point (API routers)
│   ├── database.py       # Database connection setup
│   ├── models.py         # SQLAlchemy database models
│   └── schemas.py        # Pydantic schemas for data validation
├── tests/                # Automated tests
├── .env.example          # Environment variables template
├── requirements.txt      # Project dependencies
└── README.md             # Project documentation
```

---

## 🚀 Quick Start

### 1. Create and activate a virtual environment
```bash
python3 -m venv venv
source venv/bin/activate  # For Mac/Linux
# venv\Scripts\activate   # For Windows
```

### 2. Install dependencies
Install all required libraries by running:
```bash
pip install -r requirements.txt
```

### 3. Run the application
To start the API server, run:
```bash
uvicorn src.main:app --reload
```
Once the server is running, open `http://127.0.0.1:8000/docs` in your browser to access the interactive API documentation (Swagger UI).
