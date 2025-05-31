# Real Estate Dashboard API

Django REST API backend with JWT authentication for the real estate dashboard.

## Features

- **User Registration** - Register with name, email, password (bcrypt hashed)
- **User Login** - Login with email/password, returns JWT token
- **Protected Dashboard** - Welcome page accessible only when logged in
- **Logout** - Secure logout functionality

## Installation

1. **Clone and setup**
```bash
git clone https://github.com/your-username/real-estate-api.git
cd real-estate-api
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

2. **Install and run**
```bash
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

3. **API available at:** `http://localhost:8000/api/`

## Live API

**Deployed at:** https://posinnove.onrender.com

## API Endpoints

- `POST /api/users/register/` - Register user
- `POST /api/users/login/` - Login user  
POST /api/users/register/
 {
       
        "first_name": "Queen",
        "last_name": "Bella",
        "phone_number": "0788786755",
        "email": "queen345@gmail.com",
        "password": "queen345",
        "role": "Estate_Associate"
    }

- `POST /api/users/login/` - Login user  

 {
       
        "email": "queen345@gmail.com",
        "password": "queen345"
    }
## Tech Stack

Django, Django REST Framework, JWT, Bcrypt

---

Built with Python & Django
