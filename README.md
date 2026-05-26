# Docker Voting App (Customized)

A simple multi-container application I used to practice Docker and Docker Compose.

I customized the UI and adapted the application to better understand how services interact in a containerized setup.

## Tech Stack
- Docker
- Docker Compose
- Python (Flask) – vote service
- Node.js – result service
- Redis – message queue
- PostgreSQL – database

## Architecture
The application consists of multiple services:
- **Vote service** → UI where users submit votes
- **Redis** → temporarily stores votes
- **Worker** → processes votes and saves them
- **PostgreSQL** → stores results
- **Result service** → displays live results

## How to Run

```bash
docker compose up --build
``