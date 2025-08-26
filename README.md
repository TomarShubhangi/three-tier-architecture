🐳 Three-Tier Architecture using Docker Compose

This project demonstrates a basic Three-Tier Web Application using Docker Compose:

- Frontend: Static HTML page served via a Node.js HTTP server
  
- Backend: Golang API
  
- Database: PostgreSQL with an initialization SQL script



🧱 Architecture

 Client → Frontend (8081) → Backend API (8080) → PostgreSQL DB (5432)



📁 Folder Structure

three-tier-architecture/
│
├── docker-compose.yml
├── .gitignore
├── README.md
│
├── Frontend/
│   ├── Dockerfile
│   └── index.html
│
├── Backend/
│   ├── Dockerfile
│   ├── main.go
│   └── go.mod
│
└── DB/
    └── init.sql

    

🚀 How to Run

1. Clone the Repository:
   
       git clone https://github.com/TomarShubhangi/three-tier-architecture.git
   
       cd three-tier-architecture
   
2. Build and Start the Containers:

       docker-compose up --build

3. Access the Services:
   
     Frontend: http://<your-public-ip>:8081
   
     Backend API: http://<your-public-ip>:8080
   


⚙️ Environment Variables

   Credentials and configurations should be moved into a .env file and included in .gitignore to avoid accidental exposure.



✅ To-Do for Production

 - Add volumes: for PostgreSQL persistence
   
 - Use .env for sensitive data
   
 - Add healthcheck: to service.
   
 - Set up nginx or traefik reverse proxy (optional)



📌 Stop the container

    docker-compose down



📌 What this does:

  - Stops all running containers started by docker-compose up
    
  - Removes the containers and default network

  - Does not remove images or named volumes



📌 Why This Project Matters:

This project showcases containerized application deployment using Docker Compose. It reflects core DevOps and cloud concepts:

- Microservices-style architecture (frontend, backend, DB separation)

- Infrastructure as code (docker-compose)

- Stateless design and container isolation

- Scalable foundation for CI/CD, monitoring, and cloud hosting



📸 Screenshots:

FRONT-END UI
![Frontend UI](https://github.com/TomarShubhangi/three-tier-architecture/blob/master/screenshots/frontend.png?raw=true)


BACK-END OUTPUT
![Backend Output](https://github.com/TomarShubhangi/three-tier-architecture/blob/master/screenshots/backend.png?raw=true)


Database (PostgreSQL)
![Database Screenshot](https://github.com/TomarShubhangi/three-tier-architecture/blob/master/screenshots/database.png?raw=true)

