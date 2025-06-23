DevOps Internship Assignment

This project has:
- A Go (Golang) service
- A Python service
- An Nginx reverse proxy

All are running in Docker containers using Docker Compose.

📁 Project Structure

.
├── docker-compose.yml
├── nginx/
│ ├── Dockerfile
│ └── nginx.conf
├── service_1/  Golang service
│ ├── Dockerfile
│ ├── main.go
│ └── go.mod
├── service_2/  Python service
│ ├── Dockerfile
│ ├── app.py
│ └── requirements.txt
└── README.md

 🛠️ How to Run

1. Clone the project:
   
   git clone https://github.com/HasheemHas/Devops_Assignment_DPD.git
   cd Devops_Assignment_DPD

Start everything:

docker-compose up --build


🌐 How Routing Works
Nginx sends traffic to services like this:

URL	           Goes To     
/service1	     Go service
/service2	     Python service

Visit this in browser:
👉 http://localhost:8080

✅ Features
All services run in Docker

One command to start everything

Nginx logs each request with time and path

All apps are behind a single port: 8080

🩺 Bonus: Health Checks
Each service has a health check

Nginx only sends traffic when services are healthy

🔍 Test It
In browser or terminal:

curl http://localhost:8080/service1
curl http://localhost:8080/service2

You will see response from each service.

🧰 Tools Used

EC2 Instance
Docker
Docker Compose
Nginx
Golang (Go)
Python
