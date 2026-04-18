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
3. Stop container: docker-compose down
4. Restart: docker-compose up --build



 <img width="1910" height="948" alt="Screenshot 2026-04-18 123914" src="https://github.com/user-attachments/assets/22997921-98bb-4afd-a2de-0bc0688f9b76" />
<img width="1919" height="1015" alt="Screenshot 2026-04-18 123855" src="https://github.com/user-attachments/assets/a775d8ee-0cf1-423b-b0ce-097e67670111" />

   

