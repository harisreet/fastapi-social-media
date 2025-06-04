# 📱 Social Media API with FastAPI
---

## 🔥 Features

- 🧑 **User Management** – Register, login, and manage user profiles
- 🔐 **JWT Authentication** – Secure access with OAuth2
- 📝 **Posts** – Full CRUD support with user ownership
- 👍 **Votes** – Like/Dislike functionality (one vote per user per post)
- 🗃️ **Database** – PostgreSQL + SQLAlchemy ORM + Alembic
- 🐳 **Dockerized** – Easily run using Docker Compose
- ✅ **Testing** – Pytest-based tests for major endpoints
- ☁️ **Docker Hub** – Pull the API image directly from Docker Hub

---

## 🧰 Tech Stack

- **Framework**: FastAPI
- **Database**: PostgreSQL
- **ORM**: SQLAlchemy
- **Migrations**: Alembic
- **Auth**: JWT + OAuth2 (PasswordBearer)
- **Password Hashing**: Passlib (bcrypt)
- **Testing**: Pytest, TestClient
- **Containerization**: Docker, Docker Compose
- **Deployment**: Docker Hub

---

## 📦 Docker Hub Image

🪣 Pull the latest API image:

```bash
docker pull yourdockerhubusername/social-media-api:latest

---

## 🖥️ Local setup


### Steps

1. **Clone this repository:**

    ```bash
    git clone https://github.com/harisreet/fastapi-social-media.git
    cd fastapi-social-media
    ```
2. ** Set Environment Variables:**
 
   Create a .env file in the root directory with the following values:

   ```ini
    DATABASE_HOSTNAME=localhost
    DATABASE_PORT=5432
    DATABASE_NAME=your_database_name
    DATABASE_USERNAME=your_username
    DATABASE_PASSWORD=your_password
    SECRET_KEY=your_secret_key
    ALGORITHM=HS256
    ACCESS_TOKEN_EXPIRE_MINUTES=60
    ```

3. ** Run the API Server:**

    ```bash
    uvicorn app.main:app --reload
    ```

4. **Access the API:**

    - API docs: [http://localhost:8000/docs](http://localhost:8000/docs) 

5. ** run testing:**
   
    ```bash
    pytest -v FASTAPI/test
    ```





