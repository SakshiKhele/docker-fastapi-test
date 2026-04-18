# docker-fastapi-test
Overview
- This is a simple FastAPI application containerized using Docker and managed with docker-compose.

Features
- GET `/` → Returns hello message
- GET `/users` → Fetch all users
- POST `/users` → Add new user
- Data stored in JSON file
- Persistent storage using Docker volumes
  
How to Run
- git clone <your-repo-link>
- cd docker-fastapi-test
- docker compose up --build
- http://<public_IP>:8080
  
Data Persistence
- User data is stored in `data/users.json`
- Docker volume is used

Data remains even after container restart
Test Persistence
1. Add user via `/docs`
2. Stop container: docker-compose down
3. Restart: docker-compose up --build
   

