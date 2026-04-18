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
   
# docker-fastapi-test
