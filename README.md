# 🐳 Three-Tier Docker Architecture

This is a simple demonstration of a **Three-Tier Architecture** using **Docker Compose**:

### 💡 Tiers:
- **Frontend**: Static HTML served via `http-server` (Node)
- **Backend**: Golang API that connects to PostgreSQL
- **DB**: PostgreSQL with init script

### 🚀 Run the Project:

```bash
docker-compose up --build

