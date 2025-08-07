# SecureOps-Playground


# 🔐 FastAPI Secure API – Auth-Protected Endpoint Demo

This project is a practical, hands-on demonstration of building a secure API using **FastAPI**, showcasing core concepts of **API security** including:

- Token-based authentication (`OAuth2 + JWT`)
- User registration and login
- Protected route access with bearer tokens
- Swagger UI integration for testing

> ✅ Built as part of my **API Security Engineer** portfolio – demonstrating secure API practices using modern Python frameworks.

---

## 🚀 Tech Stack

- **FastAPI** – Python web framework for building APIs
- **Uvicorn** – ASGI server to run the FastAPI app
- **OAuth2PasswordBearer** – for secure token issuance
- **JWT** – for secure user sessions
- **Swagger UI** – built-in API testing
- **Python 3.12+**, `venv`

---

## 📂 Folder Structure
fastapi-secure-api/
│
├── app/
│ ├── main.py # API entry point
│ ├── auth.py # Authentication logic (token generation, verification)
│ ├── models.py # Pydantic models for request/response
│ └── db.py # (Optional) In-memory storage (dict), no database for now
│
├── requirements.txt # All dependencies
└── README.md # This file


---


🧪 How to Test


Open your browser and go to:
👉 http://127.0.0.1:8000/docs

Try these:

Register a new user via /register

Login via /login to get a token

Click the green "Authorize" button at the top right

Paste the token you received (just the JWT)

Access the /secure-data endpoint with token protection

----

## 🔧 Setup Instructions

```bash
# 1. Clone this repo
git clone https://github.com/deadlytoolsys/SecureOps-Playground.git
cd SecureOps-Playground/fastapi-secure-api

# 2. Create and activate virtual environment
python3 -m venv venv
source venv/bin/activate

# 3. Install requirements
pip install -r requirements.txt /* wait on this one*/

# 4. Run the API server
uvicorn app.main:app --reload
```



